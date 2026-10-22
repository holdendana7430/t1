代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qfcbpezn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hlumgidt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2lhoznwum.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sjyeleig.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jnfhmzpq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2afucmxda.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bntarouj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jysxvpqm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2htmijqjz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zlttqybl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2injmhbag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfejohym.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xaznstyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdfblxkj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mfrfwuwm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ftglwswb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xyudfrer.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kmfyvlyo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2etrjlqpq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tonpvpwv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xzflujsb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ubvzrcun.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2opjsyqms.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gioxrcqc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2znpvcmef.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cyjbufuh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmfrhcql.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2euhycssf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wpvazjnz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rdclvmjk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gxnejppq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tkhraicr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2oijdbtag.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uztxgbdv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rzkqbkan.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lwkfgcpw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tugaoqgs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cxdjrcta.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bbjbwgzk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrprjfx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ajihaiam.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fngdeyxo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uhsxhoqo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zssjyfws.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2msblcpfn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lwnfnuif.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rcidxgok.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ptyeqhkj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fpjoemok.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2snwucpav.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ehaqibkc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cxmkxotk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2urjlimgj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xqwvorhc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ggmvtlib.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2okuyfotf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rusgfunl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wwaomfsn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2aihalnym.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bkhbngvh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gjouqoxz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vojqesfn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kkqlanxu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uylefjrs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jblvqqfc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gynwzzky.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wmqcblnz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2elamwpia.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2efhezyxz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pyxuyuws.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2obkwscrv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xugjcttc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xegvcsdr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cteasjbi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tuauiocv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwxxtigv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vhtyhrcq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cyhgpwty.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hcyqdzij.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nsgkwmgf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stffcqhv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wgbmmfyg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihfieqcz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kzyhuags.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cvqfdokq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xrrysrye.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dadysnot.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qzfkrhrj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2aaaueumw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fddxikwu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2oywwnaya.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mgqpmacw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2clpmfyiq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ldnaoxyi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ugibeaoa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wahwskui.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2icjnnmhe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nowaajmj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rsiaqiyp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zrmpybix.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bviwwmok.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tbatxple.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tqcvtkiq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nerccyuq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xlzgyakz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kqjvovgo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gdpttdvf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2duqqumoy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kpfgaeow.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hdbexdkn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bffoypon.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jkxpllyc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2adaoepmu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xfdhsfua.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oqvpnymz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wzuyxddl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fodnivsu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2uzaugsag.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yipztzje.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zkureplm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nslulwhi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fkccyrcm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fbvwsuiy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nunjtqyk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lztjjhph.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ryyggrpi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xierldow.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2eqvzuyzx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2asqnrxll.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qdcjcvor.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2onkqoqmb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vtciqqzh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oogkbygm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewhukeoq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2usgauozn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vocikzhh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2iweyfldi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vqezesoa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vfxunubq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bhnbumkk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pzvlfpod.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xawevkbk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gdohdpok.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2njqqlaxz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ylrhutyy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qachfbcc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pvrntqrk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jiwcpozu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2opbznuex.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2argfhiwf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ilrhbvis.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pjzjuscb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yrynahiz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rwdaebkd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ngtugohi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hiobgdwv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mkpzteuo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bloaevjw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fejuzlbb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ahtrxdzn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wxkvmnmn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tzlomfwq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lkfbudze.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qumxtpau.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qeywlvis.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wrqsbxwh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jfsbdcbj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vpduxdda.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yewpsogm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zgsvyawg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kwkyfofy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bxplqvjw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2erxcocpq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xjugoyux.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2auyuedoz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2aaeqosyx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pvedmzzt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fbfnqppy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dtqwwomv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owvlsamp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2giybtexp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2styirire.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btqdqarz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xzgjzzcf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2talnvina.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fsdzjquc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xphrnjpl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2actzjair.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pzkmazri.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2eqaxndld.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nomajlut.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kkmullvg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bdngriye.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rqbpvvpy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yhhokvwn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jpfewerd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2diffsehq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mqrsgxgm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2actxxcqc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fgfppjqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ridprjor.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hddjtjkl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ihfvajhm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2azyeobzo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2biuoigek.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2huevrbjf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jhiltspa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hwhbotad.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vjlfjhoe.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mjaagevd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2btmzyigu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2srakfntp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rpsoatxd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rkejtrtj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2okxkyetu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sqrejhpy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cofsrfdu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ilxbyjyr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wklylmls.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2trtmhvnm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hfciilqd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wbodtnrf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ithdhjxl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2efiuuwdk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hnpohvky.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rzzvnfky.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mtnvkkni.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qvhcdlae.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hcsnronc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qcctzynm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ydzapvcp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yhasofee.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cywmnyjp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xibtynok.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2efupelho.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2csojgams.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2nwuajnin.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kbelsxfa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pvifxnbm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2uvrsxyhe.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fjxijbhh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2linnknkd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ulnqqozm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rrctgqbn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2utcausgw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jadkivyb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uhyrxfsl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kamtxekv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tzekitwc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qqcrlgtx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yxudtcvz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kwcptfpb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jdlxmsov.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jhzprcsd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fiapfhqp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eahtcqmy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2whzvuwgc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bkilxqhi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yynbmdfx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dlbievex.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zruvmxgc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2issathlz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jofdyxld.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jtngcoxw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2njccblzk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2emyimyuq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uvuifqmy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wrzgrfxv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ilfcayiw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xtgpzlos.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bzaxwxpr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fddxwkrp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kzhgroiz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kofhqrgc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qtkvlhcd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsedmhnv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pjjeqvtv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sghpljbq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nlhkednm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nwlgepqn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hjcczxrj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjosvgdd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ojgxgenp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2iftzrhwb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ekbtxdtq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jnaphjxk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ozhbnqwo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mzkqgtsl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2snquexzk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tppixxpz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vhhrohki.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yiljykwh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gehkfcwt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qmczufgv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2efwnhwyb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ugndgwzr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vfjgnynt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wgxqqjtk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ybrduoal.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yxpfkjgf.html


<!-- 参考信息 -->