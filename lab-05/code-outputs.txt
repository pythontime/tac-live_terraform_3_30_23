output "instance_public_dns" {
  description = "DNS name of the EC2 instance"
  value       = aws_instance.lab_04.public_dns
}

output "instance_public_ip" {
  description = "Public IP address of the EC2 instance"
  value       = aws_instance.lab_04.public_ip
}
