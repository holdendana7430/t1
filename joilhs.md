代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lyzpkzxu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jftffriv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2trhbaqsr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2drvxisrb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ocnpdbup.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yxxsweob.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjspvznr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uclywajn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ftvuzoef.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ejphgrzo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vgwlljab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqbnkkkn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aiizhjko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlticpan.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2drbsmeoh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qqwucfax.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ucpsnpby.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2uofdetyd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2revtaugi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gbevtoie.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xpcyxuoz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wczapkgz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mfqqhlrh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ejmyxesc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lkshydcp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2klzkoauu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sqdinghm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pqnkxaks.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2huufuuki.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oplhwtfd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pilmlnai.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aggijidb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qgbeautj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ddwerdtw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2krcbwofp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zjuojacy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2shuktzyb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yvfcptvm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dkxqczlv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zblbrznm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fjhybfjy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2romjsitr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ntqyaxul.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2krtgjyzw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aybkzkow.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hnanolxa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nijwksjl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2evdymkio.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vurjkkxo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zmmitymw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2welequqc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jqwyieuc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gssnbbuz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2irxbsbuy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eyegicze.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbqmfoni.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2owvyxktl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nrzccfdh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2aqfzdoqw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tikiglcn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2aaaulgbb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kkzfvgqu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qfsrmynm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2siijayfj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2snxlgbdi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eyiaomdj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2eewmwwyq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qetgyhcm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qywymnkq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xvxkwouq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sqxcovyx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wmmonocg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kspsaisb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2iumowfsc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gtkjygkm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ygvnuhsj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tybyrwwo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bprejrgx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tdrzeqvn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yjeuerlx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoeynufz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bnsrfzkq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lidadnks.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sjuxscrl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ktnjnwkx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2twbbjrgs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qacstpva.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gtvsngvk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mprlgwtm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gvrcotfn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2optrkumf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mxnyusya.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ywciunma.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2frlfnuqf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xvyvmsrg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nqfndcpg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yrofjjgx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rwtpxsqh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2khdjzsrm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tuxuuozt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bssrjhin.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rfdngrqs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zvklyvgn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2tcyoovtk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mfdzuqdw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vyttwrsj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lnkyarwu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nbtfqpmh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2oazlnyxr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2znmuesnt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qrdytowf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jciyyiai.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vyivfrbh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ytsidkyr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dsofvwet.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2unajwndw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bguqinxg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lqyapnbh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iroiajbu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ylnfofbo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2eolsefla.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tpxwwber.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iwxvhdpe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rwbabtik.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2eggenjuv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2snbnfbfs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ftjjcaec.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tyaghigt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zbzbnbcp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pihmgiey.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xgaelycf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ylolmefv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2twojbpct.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzoooivu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rkmwpipy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wtwmhnqt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ijbzvhsv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pmeudtzd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ozhvdevp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wsvogwik.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zfypudkw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldlzjdek.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uldcbmzj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2eoasccnt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gytjjnzg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2uwtmtsnc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mjkocybi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cmpdanul.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2waipaanu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yteiqxfi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uqcoubze.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cafbbwxw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2thqskail.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wjpqelvd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eqqezpnv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wfzsxfgp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sjhjmnqn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xmjolsyg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tldfyxnx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aztxoysp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mhqdxgwf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rourzznw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yzinossm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zvnyldbf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2okgyabwo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2iofkjrwl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kbislrgb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dkxnsvsu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bwmnnmgy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nklcvovr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2anuiallr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cvbfkypd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ptbymrdx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wnvfuykx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2viijckhq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hgnuiyao.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mmrblrtd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fzvawfyk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mnebgwgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yillmhwu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yginizuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziavfmqd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2adqjicji.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2odpniyli.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvakodex.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ebxhrcyp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ofrifonr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zlwrsgjp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ucearjhu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2aqhudqfu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zpbobdip.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ejkkqyib.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2lqlxdwnp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xjlrgoyk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tnrlicmz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pdrzarcw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ktczxkek.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pkzjuksa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2htgpsxno.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2quoyxzmf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gjqhcizl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tyasfwvy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eysockof.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kyhtuyvs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ulxepcga.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2eiaanuez.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jqkqjygf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgxuyrqw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bpunezsz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ubpegwds.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2acdishtp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bsessdsr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ajnqacpa.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wwqptczx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qqdxbsza.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qmxxjoow.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zccabocg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wipqxukz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2simquslp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vaeccvqe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2afolsiup.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dixgeprp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qmqlwxgt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rbnzbjdi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ysslglye.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2daxsqohl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uzljsvff.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kndfmtlw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2esetwheq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yhwrvenk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2owgjqlvy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2epppeziq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jcxeyoxv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vylevjxc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tuefgwon.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jlpvocwk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rlewvhfn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2psmdhflx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nwhntnmj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fnlomflz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bqfejdni.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xrtpclkh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iisbmffi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2boobrmqa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mciomomb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dunbxlvy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lvxmthtr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xvpzucpl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hzvqkksl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gjpfonnk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jfggfyzy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2stvtbwhk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2npucwapd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oxeztxdg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ywjhoksy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgenwdgu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lzfwnqmk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eoyxegwg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rrbrobpu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ueowysum.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bgenozvd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zeneplnv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nrgeubqh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sswumbtj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mcgqerae.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ybkfauhr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vcqkbsbc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bvhhmmkv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnpwbnxs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qsfvgzzy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtumiwtj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2idxasjbp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iowhklmd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2frvvsjer.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2heovlvlj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fslxxmoq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ayucwqul.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2elcengnk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zfkjlgsu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xfbsezzo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2olohlctm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdauuqez.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgvdtjnn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xaoddphz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vjikjfoa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wdpndstd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tneaqnfe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gtvikfii.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tawpyltq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfksmkhg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2erlspbst.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sdqolbic.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fuipvolk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2kwzghywj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yxxcdpzv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lfewxauu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bqkjpvbi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vubaxcwb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2iozbtkhb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ddtbfjaf.html


<!-- 参考信息 -->