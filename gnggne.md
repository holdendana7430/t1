代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2aymehntl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2evaibqqq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yfdxocmv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2bqujnazu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cdbmgsvi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2aesbkvrp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgwjchzi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2khbjgvjk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gnknljlh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2tlppsvxi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xpmqwtyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrvhwtpx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2btchdjjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eszswghy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mgjlbjcs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2drskgsjf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uyumelfp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2essizrsv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gwrqtvsa.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jvzslxtt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vlnnizwm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfboiqau.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yuaovmwm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vortdnsg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xugzwepb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ieethsgm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2unochwls.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fogzvlpy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fpfnovbk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tewzsznt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2upigrhfq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gaqfilvm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2licrtetn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tbtxkuty.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tfigbatg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qpjqnkuk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2htfgiuzw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rdlbyuuw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pjfrzovl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vvdjwwju.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yhujteqz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2igyurueb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qodxjsdq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oupneovq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wsykglty.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2iihrjdjv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ejfwrnct.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eyrmrjdh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kouscazc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hdhaevsm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2izlalpas.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nmunenoi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2idxchupd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kjrxyrke.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tupuwrrr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nljwoyhx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2uefeqtck.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jqhycynb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vulrqopd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ncaoyood.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fgwhvvbe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oibaymgz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bkhqcnze.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xugiuktp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qiifdzxn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rjjlmvij.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rdjebivm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uwivfvuq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhvqqyda.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ijrgviae.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aahjjaaw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2awuikaih.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nsuhmchw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2egjexgjk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2icdknign.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fwzmbbsj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yguhdmei.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jhbeqtau.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lffftpta.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pgoyvpxy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ukwqsqke.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ncxirmwp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrmiopqh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2iuikmras.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2srstikcf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vtrcudvb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2soidtwjz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kusdrgjm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2znlwajnt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2sixqzjfk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fbrygprx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qjbxjfim.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtfsjmun.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xviwotzf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qighoepr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nunpauqm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jlxbemkv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cbivfraj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qgdbijla.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2atjlpodn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hwgwpcwi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mhsptnhh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oiapqivd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mrektcbj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wqgrerqr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2flkbmtea.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2nkjzcava.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dlmbvpht.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jvoceaez.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tyilroqo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nwszbhiw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2slyacqka.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gtcvufxx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2seywcbch.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nwshpmdj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sazvdszx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tpmhoeez.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dsdbiahf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iuvrmwyp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2msbzwhnt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wqgqxzrj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2noqsjoda.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dlmzmdir.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2osfcndxl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ushnlkjk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bsytsrut.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zjfhpnjs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jzbtvgpw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ijcfehdn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hxhsfuld.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cpsrfdsx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jntblpbk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zkkbpdjz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfsizbcq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pxftfeat.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ycjvmsgz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dcomkork.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nglohcad.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hoggmeal.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nnpqzsbs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2yanyeogh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ekfiakoi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mtzxcmza.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2yzmlbrtu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tijnuipa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2llwkayra.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyjbqnh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sjeusecm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ouzhzthj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lxkiymzq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zjemqkao.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mayztvdb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kxtvuwit.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pkgzened.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jfpxgvpa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2unteniyj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nwatqzxu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2rpclnkbv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sbngdsvz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dkcgzxor.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zhvudbeb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yngkdalb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gqypkpdo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2irwpryxi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mhmjaoht.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2iycezjwk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ssnnbdlw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tngeidjz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kxzmgjpm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mxltndst.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2miijrftf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tgvoietb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fkbnpdpg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yopoednd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ioleiliq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2stoibnzm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mxlviiby.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jtfwnucn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nniifizb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtjecate.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fcinchgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgihdykj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2btvjezzz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cdpudymp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tufrnbsz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sncqykjn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2sqkiiial.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hqufqrxo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hykuiolv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2macdkrjm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sqnzestw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wagjibyc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nzhhlhim.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mzvclrzq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sfijlqgs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mvjoesed.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2werfhzvs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bnwkwerh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xbtclxbr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lvwfiiqf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2uwjzbqny.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qiprtsxh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tigipmic.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvbwhntx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2miyxupvb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ybdqejvr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sghjohzi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rxpzlmlh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pxdbyvux.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aelzvanh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2sgmmtlnh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fouvnohk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hlqionia.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rioacpss.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ajwkertm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ybtjkyly.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ricrqagn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnmpzylb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qyspurft.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pqglddzb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ycayvljh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ptsjkgzc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uftcvzyx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tjsgybrz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ejpmdvbq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vpolumra.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hapohlik.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mltljkao.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2fkwcegoo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ococfnlr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2twtnvpgs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ptpkujas.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ofyderiz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mjowpkqe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2filthols.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2emvahhgj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ahblqzhl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2brzljgwa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2shisbtdq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2anbanede.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gglhvgag.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tkmnjqlj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pnxlsemf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gujxnowz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2iiveekui.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2daeyawgl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2twksuzpc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2greqhorm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2owdmrxav.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaslvgjv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tbqmqjir.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xgzserng.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kpnydoss.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bjfsnhwg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2napsedbs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ctcevxpn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rvnkilzt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tpqhxhha.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ejzfvwaf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdqhuusd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2sctqxysf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wewfkwtd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tddldoou.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2buqzxqwr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2naqwgvit.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rzuohrma.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tvldojgf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ezhmnafg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lifxtcsb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ynckypif.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ekrskggl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xhryyyww.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hlscoboq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ylqhrbpd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qitbmsne.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mlkbbgmk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2itdmozbj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xkxayywr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ehrqmped.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wainlbys.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ooyfhpga.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ipjyzsbj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vixpwegh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2smfdxmcs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fplzhiuo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bosxspsn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ngvjqsnu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2revtshgq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zfiepngn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2frootjpl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mabohdyd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2botgkhue.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zetpjeut.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2blgfvnec.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hebbupzl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gsxandsh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ohwbzzrl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zxzekzcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2twzprzbu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2srxytqsg.html


<!-- 参考信息 -->