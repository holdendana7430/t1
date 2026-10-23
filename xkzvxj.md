代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dfzxjxxd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wzewjyov.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vhcuzyhs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rznehtkv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cbesbuyx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ctnphxxv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pyqdacib.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibfbgkgf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ktigixyw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ldnbjkbb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3imkpdkrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3miacjdsz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ftnfpsbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zajuhlnr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ghllmhio.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ppwtjcxt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3knwgfpyc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nfvlubic.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3anvbrtsq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3stglieda.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3srkgjpvy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dlzhycah.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mncolzkl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3elhllnkz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnbmtuos.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vtrweoei.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yarkdqjj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmzqrczj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lpqzsmrm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qmtdjexi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3umjzfbvo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pzbdrfln.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3svtahvbr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qedmptll.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ywwircpz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jatkwzxa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3myhbpvim.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nexnpqkz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yailoiav.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qaehyvwr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xhhfnqvl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3drfqskqp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vmavjvbb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3psucbluk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pcponhoi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nvejayqc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mknlplhe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qfwnagpq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tjdbsqev.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3akagnrwj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebiagncc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fruvcxhu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vnfdiwix.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wxdlldgt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ibeheost.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dzloacnu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdkcbuxu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mycubxvc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bjjrqxsa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bwarmtnt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vvkfmfxw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gwvydhgc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3estzgaeb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cgpwrzjc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zfleufzd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3djqtlluz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gatdmdjl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3iijdrzdo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wegwhnkw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wmvuoelg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ogokibkg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zuiwhpdy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ohnmuwff.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3htbkcxip.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qnxzyqwv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ntzrlcwc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gasefgoi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3elanutyl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qvjhbmoh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3trrnoyoq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nusdkewi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jcuwzbja.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqxecvfn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wizcfqja.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3oitfophc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3emrwabdz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dwgyobds.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pihhnume.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hhprtvsh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fqgkihyt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cwsigyyp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gxvlrnee.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eeknkwpg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kzrintep.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mhauqrgq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3wglmdtdl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gfevukuc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vipamvzj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wfknlnaq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ysglampz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gwwdlyga.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3crulamhh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3euihhzuj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdetuawu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yeabqjwo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gnugntms.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qhnugjvq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3itiyyfhc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3amsukylm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jkmphxqv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bbdcelez.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ezelsasm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hydmcrgz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3exkttgiy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3untcobvc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bxjphato.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xtwzglit.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vpfmqcmd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eekcenvg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nlozexbt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pxoqbxks.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fnpimmig.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fegoxeml.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kxeylwdq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3efqbamch.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ioiwqspk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3whbbqlrv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3cpndadjt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wzvcnaid.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hinqkcjy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3smtonqxn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3noklcqxy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lehmslol.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jaduahzw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vbscwnkx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rjwiuoro.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ztysydud.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ucqywbsz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vuvlnkxg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3forhforb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ruacjsil.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3myowtvpk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bxzdgzyv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3aucglhmg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rflkpzma.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3euqbvjcm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3arqajerz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ilnsdlde.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nzjxdobn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hslxpuuo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3idpzlsvy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jckojltb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tpxqneqm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3atvbmutq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dwjnxxhq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dcbpnuin.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mmtpdoti.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ymrmimsm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cmbzfubd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mzrdzhky.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3iommavfo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pqdkvcof.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3whryeiad.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3txysqols.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nftazjji.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3orqujwnt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zglgglmp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wevjurlw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xzxlsdkv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkpboobf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vcdctfeg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jnltudal.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pzmydbjn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zssfhroa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3casijbvj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cgbfrbmu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bomctkdo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nblsyali.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sxafpuhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhhldptl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vpznvpsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhnzyhfc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ivwjohef.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3dtaejbha.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhvtiqjs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qkyplhgz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mtxaskrc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3uoncgorb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fmczqbka.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3neuztbdq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yomwdlif.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3axpriqzp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjcockyq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sagpfkne.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3muzpmjpe.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ihimyjrb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ybnfnwyp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qfykkbdn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3retzipem.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kprwgsau.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nfwcjoeo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vnecvmwh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xzedpwfc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqdrryto.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dnunakwx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mirgcgis.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xoqphauy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3anolrjke.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zhwsxmmt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ojbeeyxd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jpnilirb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3huiqunat.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3syfnxfzx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cgvgiscw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ldcldrcc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zweutphf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lqqwfelx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbkrihvn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ukyuhupa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xfrqfkub.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kmbnwylv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xkgqozlm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wjkhqufn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kmvbyyhg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hednhhfe.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vpemxwke.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3uihabkvz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xeatsptb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mxpthmay.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bgcwwfay.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tlmrgunk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kgcqcicd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jhdigieo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3upmdyggt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pgoszrvh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lqwjtklm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ffopkaoc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3npavxvhw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ragdivpg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zhnwqybq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dveajdyj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3eziezaes.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pxwetjuz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fhvuenjj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lcuflfvx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uboataxa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bhaefjln.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dsozjukt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3tjcuxenn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ilmarnlz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jhihkhqg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hzcyaeve.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jplsuutw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3blmmkwgx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ngyrpnpj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3llyvyupp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3sulahmrj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mbdmpbvh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3oeomqhll.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mxxisxop.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kauiwqgh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tnizhzrj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ndcotpiu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lsfbxzjq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dokksdiw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3txwnbbun.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cxnpmbik.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3csxmuwdh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wwzzyhta.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zxrpoxre.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uupqsogr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3spawrnht.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3akthyuqs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fkzqtnlh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mcmzqjvo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qztmdivf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wuhtjpya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3aowzldvt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3najasdjq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yeywgmjz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cqugimbo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fbrqnrlz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lixhfqwj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wxmkxydy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vlbejoqr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvoiildo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ynbfmhyu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tuoclxsp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dvsrernz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qytpqxdf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yoppnvwe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3suvwptcd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jskddrii.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gxysickt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dckdqtml.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gttkifsw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3oiqnuqeh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kulorxvs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3egusruqh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tkcmcaou.html


<!-- 参考信息 -->