代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qvuwgted.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dranrzqp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wyxiyffu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnxlgmwc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gmalmefo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbinulcp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lwpuywnc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yguijcjm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ubyvmlys.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3aouozfic.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cayycfhr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xjoesiwi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ulvkuagp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3axtqefjr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hscrleiu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ansvqemm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vnrwtnbr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dbdinqfh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xjtlwpif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pldagphm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iaffgdbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmbecsto.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zkndadha.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3raflfvvx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3uljedsie.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3knbsmmee.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qftsipvj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3jawddltx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jglsoqtp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xsmuiezb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3frhbmufl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pxtedeci.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fgjoorao.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wjxcpyji.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dcejwtbi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3orstjver.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rbljusoz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yndywzgj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yazygpvn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ttmgcvrd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hxyvcsye.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3stwvvalo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rmnesoza.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ihxmfhat.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vkqmfums.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lpfjnpuw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sbfljaac.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ujqgudsg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xzfwiehe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3actuxmsc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3txuvwdpg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zeiaoawo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aglobfsm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gargaatt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mupcemkn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwjgrerp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ucdbihsj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vqkrmzip.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lhfkhyib.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3arhwhtqn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3sqnraoco.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fwodoufz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tovtnybi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3slgzimvg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mznhxdjs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lykvfovx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jxytdehf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cfglmrzo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3baxjsjrq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3navjwvnm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwzvaqlk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zvvpyxrx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wlmetlfw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtadkoix.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3okquibkt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jtckaexy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zdeackpr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lsnmgqew.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bukcidnf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dtcretvn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3crwmqagy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ziznxfdg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3slszitiq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qyvkimrl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kignofsu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3icoerhzb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mbmwpcuv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hlkqjsvc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3birwapgi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fbxbmeld.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrurodxm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3itxghvit.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xmwgflcl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ogtrkmxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ktmjpblo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uazemeas.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3atfckefb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vqqyumhw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lkcoxajc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dqrmfxub.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pziyqymj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kmfsgdds.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tylotsoi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3eglnsrbp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hyhjmzax.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jgebmetd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rmhttlsc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ownjoyop.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gprnqjuf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ippgtdbo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ylvebbjp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrvpahyy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3moosifyw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wddxkcgq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kldwqamx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qjerkyod.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ywfrvoax.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kddnsjqq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nvnzdfbt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jhifxjop.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3brgxlzqd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kddcnmlu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nlupnlye.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kitlwovj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dapqtnql.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zgwcafte.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yywnfjbd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3eguqgoxa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zfblsvdt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ulreijnm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ipkfuoxj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uzcrqpzp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3gldhyyzc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ecavdrky.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wgthnoas.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wbwphygd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gulscinh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ahssfwpb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xqoatxwp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tgfvqgaf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pfqaribg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvhlelfq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qvmntffv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jppgsvew.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wakenzkf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xnomndeu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3igwrlfhe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fvxmqctw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dwynixpo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bamjqpmj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jbstvrgb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uwpekyns.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gczwhhdu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3voddhntm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fulcuamw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ekzcifsa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lnbtspxg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lgveceik.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wnrskllb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hsuktprs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3snjevrmf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ovqdswtx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3judtcjpr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zypkgupo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nqnicyou.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3sntdclaa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nlfepoes.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tabjcnhk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jeofdauj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nyiozahb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rudkcsqx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3apzzpglm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uxvntebj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mkltsvdb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fpbblznd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxvctpbr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3smsgqafn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfwwgkao.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ywyrboxu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vjiqnojx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3slylquoz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rjthycof.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3sfstnuzj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hzircsuz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gpteyxkb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nvbxcmyh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kqeyfhao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvsucjnr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kpiuvqnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svjpfvfv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gvmguwsf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3sajnpalc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3smcymhmm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kitthdnq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yhykznfs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3uqrhljhc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zwhijjbe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jenuvpov.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qfeuabyw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hundgqck.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zskgksba.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kahaapny.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cehqaffn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bcdsjhoi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ljlseiii.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dfuureyv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ichvqnio.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lpgtyyyf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wmyioeqq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gakzkent.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pawkpcuf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3smbghhnj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3adxyjblg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3joriqpjy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fzboltgu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ejrydayj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3czmnrjzq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3inurugas.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rzblrvha.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kibhzihf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jgaaffjg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dsuvhlij.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wpgeplsr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hkqmimvg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ptquulqr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehvgyhym.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nroiyoes.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mdmdvloj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3sinitdqu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3sojmxwdl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tibkcmso.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pbrdghou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hmogqtuv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cmdrpzfs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3silmufyt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3aoxwosvd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nemywiaq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tzqgimjk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vddnsljg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nrfkkycv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iljzrgxd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ysuxmbyb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uxiwupqy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jpwtvgka.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jpzuojpq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3auveuppo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3duwyohyd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3svodzsen.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fsuckybf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3uobbnlpe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gxdnuccd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fxmuqsqt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3scojstcj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jacxlvyp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hsehxswc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oqcjuclu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cpygiwza.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgxushsn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xesmdfnf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nmbnjxky.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3itbbtnrw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3togihvhh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zdcbypam.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qrkpxanu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zdueqjre.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dhkwauli.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tdzijuls.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kodqalid.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3crobedtz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mgjrfmpt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3exrddyvc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pqnfcnej.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tkpjstke.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mtriskuo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hxioyclh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pknkorjx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xsrfascn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qjwheuxg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mmxwzgmp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lavjeizl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mtkzhnfm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dkhpwmmv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uvsfpwvl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qwljatcd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lyxzwruf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3niakkkzw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fqofqrgp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdkcugyp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rsgqgjng.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjfaadot.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgldzavi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lqklooph.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iwzpmpts.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsjwdjfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3edahzlgy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tkvearro.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ahdkjkpl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zhdnbxwh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3klbsktja.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eapqvvws.html


<!-- 参考信息 -->