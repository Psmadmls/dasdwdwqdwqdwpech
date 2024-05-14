# ใช้ base image จาก Ubuntu
FROM ubuntu:latest

# ตั้งค่า environment variables
ENV DEBIAN_FRONTEND=noninteractive

# อัปเดต package list และติดตั้งแพ็คเกจพื้นฐาน
RUN apt-get update && \
    apt-get install -y \
    build-essential \
    curl \
    wget \
    vim \
    git \
    && apt-get clean

# คัดลอกไฟล์หรือไดเร็กทอรีจากเครื่อง host ไปยัง container
# COPY <source> <destination>
# ตัวอย่าง:
# COPY . /app

# เปลี่ยน directory ไปยัง /app
# WORKDIR /app

# สั่งรันคำสั่งเพิ่มเติม
# ตัวอย่าง:
# RUN make

# เปิดพอร์ตที่ต้องการ
# ตัวอย่าง:
# EXPOSE 8080

# สั่งให้ container รันคำสั่งเมื่อเริ่มต้น
# CMD ["command", "parameter1", "parameter2"]
# ตัวอย่าง:
# CMD ["./your-program"]

# หรือใช้ ENTRYPOINT แทน CMD ได้
# ENTRYPOINT ["executable", "param1", "param2"]

