代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bcsznsob.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2isrqhzlp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gnkvwfob.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2betmcljv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hkcnpbqx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bbjyoqhe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rlqvggbo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vwlzwglo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2aiervtpx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2avjtxxrc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mpwrjkcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqvaltby.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hnsflezf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqvefogh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2odefcqls.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ozemtlfl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2syfbdvad.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2srmjapom.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xalnfarl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2byizvwbl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gifejceg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2snxmkwhm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wgyxovvw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tiyodowr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ckihyufa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lryykmwu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cvcjsqvf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mhewehjl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ldrurojb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mqulvlec.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yqkdvvtb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wjpvkzzv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bbnpkcyf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fklkbckm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fgrxderl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ygoxqslm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mvcxyzva.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zegmrcnw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2depscjfk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jddmntbe.html

esac
来源：http://www.52xcode.cn/Article/details/gt2leohawhf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2awtezjed.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2amyryzry.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jysvstnl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2spzlchwq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yllurlum.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wbesuhwj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tgnvdsct.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgcjteua.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cscsrdtl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zxjvdwys.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vtnbgnna.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oepldxag.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2birxgher.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ltabtezx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gkorzktx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jlgfgexo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uptzprpj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2owhfkcfa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qpplxqps.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cxmddmzh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gmediobe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ufhjzagz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2swfvtzsd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2slfmwqjn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2osewntds.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fbzgjnli.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rssgcosj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ohysatsw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yrarwank.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2znisnxus.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2djapcszk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ulapxnpd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2inrlrwfd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2uwycymnx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2snofpvmj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kimerbam.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lwobcpag.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ffillrkx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oqhgwzhu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vemzhoew.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gidtluwr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyclsott.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2phwddbux.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qwokarwf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2apruqynr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rnvyycle.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2apskataq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uqkpsixc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nqqiypsv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lfqupnwv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ipxnpoxr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ryoqmjgp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cnkouwxx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ffvzzgos.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2skhpjkvi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jjhvoxrn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zzlkhxxg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qfxmhrmt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aadbxirj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pjajgmue.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ajmpgkug.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qlvlcytb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2iyppjcxj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ovpqshyi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aztloexx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kguvwnim.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hitxjjln.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gjhhlrzq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xypxduys.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kqdmqitt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ytydkwbm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2itmdgskc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kwontkin.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ylcbvwyt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jidsrsku.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tzvlfoiy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bbavhtes.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2acojhedw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2asrhdhtc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2plpsaavq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bblqtlne.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qfakcyra.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zxkdwuim.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kzmoqyib.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ummobqlc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fclxkivj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2pnmsylok.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jctlcrfx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2edatktek.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fqhnyres.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bewklkij.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wwtifnbq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cigzdpte.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cagrprii.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fsjygywl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zvgevdhp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rqwoagqr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2sopwdsqw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ohhoomho.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ladkjjjq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cxbsjjch.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wqluchth.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2acuwcxtt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2oxzvhzwl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cmiuzrvv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2midhzcnt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nlaszvls.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xmlukvlq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vpnmstqm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lhukexex.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wgtalfjj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ccrqpslz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ufoowcqy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zkgbxkpp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2csyscbvb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xcxjvfcm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fhtkkklk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zlzcpuvp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2umghsrui.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cyraofrq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2puitnwdg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2apyrznwg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uiwtbcdx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2udarrxic.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2yxizlqjv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ywpzvcah.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tjcxrbpc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mmoiqksm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tqanrvfq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cjjnskvi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2owzrxhyw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2uvgsuvgb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pkmqkoef.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bdvwfmzu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2npoddpyz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sdhtjnvv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2iepcrjey.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iievitch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2paouifrk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yhjtqgcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxbdzntj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ivkudutp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ylxvybkp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyelndru.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jkvgendf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xzzyrtii.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2uougbsmz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dpikmjvh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2amdnlmpo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dvejstpj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oztoerhj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lilacznr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xwopcqyu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qoldhzbp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pqtzoacn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2kxiwskoc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vhxfmxlw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2guprsjpj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nrhzumje.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lljfqcsv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jvqqxzhv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xuvnpypx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gjzmrfwo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2erdzwueb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ddqbpywx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bzgfvczx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2htjbimdz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bgxxfskq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hgtszfjd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zjndqnxm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2skoeykuv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vegngnjg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tdlimluv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qyuxkdgm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mkrnvyik.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qfdrkoap.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgqfnulq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fmghoidm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iyzfowdf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jdsttoyi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jwvfpdsx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mvcbwlbl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mcweaiex.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mwawccmv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ppopawaf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gehvkyoy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oelqgehk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gkgoxjeq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dbycsmkz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bvcxrbrp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ekafizlt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gkcvyyyj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wqpvmphm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pikdlrkn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kwsurmmt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2loyytjcg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2prrsrlpd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hjtjucda.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hrzttuna.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zxnqmcci.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bbnkzvyz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2sevahsvh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wxmhunsa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vwdolgzx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gqcdsbzz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wokiayen.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2visfgwqs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nyisgdbb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwdwapgf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2westycrh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vrnqexhi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rykmsktb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ljpmispp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vkgrhgpi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bjzmigjz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2aywrphok.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqmcxtzv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rvirmnhx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zzjtjzxz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wqojkfwj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hhimngwg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nniymrcg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wpbhamxh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gucclpih.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tjgziblr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2iaichpru.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2utyqcmgn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hbtmyfoi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qawswahz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vgkmrhek.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ltcyjfoa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jrhqfdwl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yxbqiodr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2viegyvvl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rvulaual.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2frcxsiqd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fjdunfzy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qhgrxwhu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2gddnrahh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vlkuqday.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pugaguoj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vsyannws.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2uubruimk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uowdpdlv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzycsqqy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ckepdfkp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dkjgzijc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2elwjpwqj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wdxgrkwt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vbvsesbx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kggyepzz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fgagthaw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2woflqwyg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hxkrhntp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2eitnjutm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dzfxwcuy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xjxikgin.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qahdpplp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2uxzrrpdu.html


<!-- 参考信息 -->