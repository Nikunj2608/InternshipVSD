# 15 Unique Instructions (in Instruction Type Format)

1. **`li a4, 0`**
   - Instruction Type: `I-Type`
   - Opcode: `0010011`
   - Immediate: `0`
   - rs1: `x0`
   - funct3: `000`
   - rd: `a4`

2. **`addi t3, t3, -1`**
   - Instruction Type: `I-Type`
   - Opcode: `0010011`
   - Immediate: `-1`
   - rs1: `t3`
   - funct3: `000`
   - rd: `t3`

3. **`j 17f6c`**
   - Instruction Type: `J-Type`
   - Opcode: `1101111`
   - Immediate: Offset to `17f6c`
   - rd: `x0`

4. **`mv a1, a6`**
   - Instruction Type: `I-Type`
   - Opcode: `0010011`
   - Immediate: `0`
   - rs1: `a6`
   - funct3: `000`
   - rd: `a1`

5. **`lw a3, 0(s0)`**
   - Instruction Type: `I-Type`
   - Opcode: `0000011`
   - Immediate: `0`
   - rs1: `s0`
   - funct3: `010`
   - rd: `a3`

6. **`addi a6, a1, 4`**
   - Instruction Type: `I-Type`
   - Opcode: `0010011`
   - Immediate: `4`
   - rs1: `a1`
   - funct3: `000`
   - rd: `a6`

7. **`and a5, a3, t3`**
   - Instruction Type: `R-Type`
   - Opcode: `0110011`
   - funct7: `0000000`
   - rs2: `t3`
   - rs1: `a3`
   - funct3: `111`
   - rd: `a5`

8. **`addw a5, a5, a4`**
   - Instruction Type: `R-Type`
   - Opcode: `0111011`
   - funct7: `0000000`
   - rs2: `a4`
   - rs1: `a5`
   - funct3: `000`
   - rd: `a5`

9. **`srliw a2, a2, 0x10`**
   - Instruction Type: `I-Type`
   - Opcode: `0011011`
   - Immediate: `0x10`
   - rs1: `a2`
   - funct3: `101`
   - rd: `a2`

10. **`subw a5, a5, a4`**
    - Instruction Type: `R-Type`
    - Opcode: `0111011`
    - funct7: `0100000`
    - rs2: `a4`
    - rs1: `a5`
    - funct3: `000`
    - rd: `a5`

11. **`sraiw a3, a5, 0x10`**
    - Instruction Type: `I-Type`
    - Opcode: `0011011`
    - Immediate: `0x10`
    - rs1: `a5`
    - funct3: `101`
    - rd: `a3`

12. **`slliw a3, a4, 0x10`**
    - Instruction Type: `I-Type`
    - Opcode: `0011011`
    - Immediate: `0x10`
    - rs1: `a4`
    - funct3: `001`
    - rd: `a3`

13. **`or a5, a5, a3`**
    - Instruction Type: `R-Type`
    - Opcode: `0110011`
    - funct7: `0000000`
    - rs2: `a3`
    - rs1: `a5`
    - funct3: `110`
    - rd: `a5`

14. **`sw a5, -4(a6)`**
    - Instruction Type: `S-Type`
    - Opcode: `0100011`
    - Immediate: `-4`
    - rs2: `a5`
    - rs1: `a6`
    - funct3: `010`

15. **`bltu s1, t4, 17f68`**
    - Instruction Type: `B-Type`
    - Opcode: `1100011`
    - Immediate: Offset to `17f68`
    - rs2: `t4`
    - rs1: `s1`
    - funct3: `110`

# 32-bit Patterns for Instructions

1. **`li a4, 0`**
   - **Binary**: `000000000000 01110 000 01110 0010011`

2. **`addi t3, t3, -1`**
   - **Binary**: `111111111111 11100 000 11100 0010011`

3. **`j 17f6c`**
   - **Binary**: `000000000000 00000 000000011111 1101111`

4. **`mv a1, a6`**
   - **Binary**: `000000000000 10000 000 01011 0010011`

5. **`lw a3, 0(s0)`**
   - **Binary**: `000000000000 01000 010 01101 0000011`

6. **`addi a6, a1, 4`**
   - **Binary**: `000000000100 01011 000 10000 0010011`

7. **`and a5, a3, t3`**
   - **Binary**: `0000000 01101 11100 111 01111 0110011`

8. **`addw a5, a5, a4`**
   - **Binary**: `0000000 01110 01111 000 01111 0111011`

9. **`srliw a2, a2, 0x10`**
   - **Binary**: `0000000 10000 01100 101 01100 0011011`

10. **`subw a5, a5, a4`**
    - **Binary**: `0100000 01110 01111 000 01111 0111011`

11. **`sraiw a3, a5, 0x10`**
    - **Binary**: `0100000 10000 01111 101 01101 0011011`

12. **`slliw a3, a4, 0x10`**
    - **Binary**: `0000000 10000 01110 001 01101 0011011`

13. **`or a5, a5, a3`**
    - **Binary**: `0000000 01101 01111 110 01111 0110011`

14. **`sw a5, -4(a6)`**
    - **Binary**: `1111111 01111 10000 010 01111 0100011`

15. **`bltu s1, t4, 17f68`**
    - **Binary**: `1111101 11110 01001 110 11110 1100011`
