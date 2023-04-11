resource "aws_s3_bucket" "bucket_beyond_the_cloud" {
  bucket = "demobucketbeyondthecloud"
  force_destroy = true
}

resource "aws_s3_bucket_public_access_block" "bucket_beyond_the_cloud"{
  bucket = aws_s3_bucket.bucket_beyond_the_cloud.id

  block_public_acls       = true
  block_public_policy     = true
  ignore_public_acls      = true
  restrict_public_buckets = true
}
