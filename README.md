# load_xml_to_bq

CREATE OR REPLACE EXTERNAL TABLE `bnm-experimental.bnm_test_ext_tbl.xml_test` (
  col1 STRING
)
OPTIONS (
  format = 'CSV',
  field_delimiter = '\x10',
  quote = '',
  uris = ['gs://bnm-bucket/input/xml/notes.xml']
);

