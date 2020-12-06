# bulletproofs测试说明

## 1. 项目来源

- 原始地址：*https://github.com/dalek-cryptography/bulletproofs*

- 修复地址：*https://github.com/eranrund/bulletproofs/tree/uprev-deps*

- 现存地址：*https://github.com/teimusaku/bulletproofs*

## 2. Rust语言

1. 安装rustup：`curl https://sh.rustup.rs -sSf | sh`

2. 安装toolchain：`rustup install nightly`

3. 设置默认：`rustup default nightly`

4. crates.io换源：

   ```shell
   tee $HOME/.cargo/config <<-'EOF'
   [source.crates-io]
   registry = "https://github.com/rust-lang/crates.io-index"
   replace-with = 'ustc'
   [source.ustc]
   registry = "git://mirrors.ustc.edu.cn/crates.io-index"
   EOF
   ```

## 3. bulletproofs

1. 下载：`git clone https://github.com/teimusaku/bulletproofs.git`
2. 测试：`cargo test`
3. 评估：`cargo bench`
4. 查看：`firefox ~/bulletproofs/target/criterion/report/index.html`
5. 编译：`cargo build`
6. 库文件：`~/bulletproofs/target/debug/libbulletproofs.rlib`
