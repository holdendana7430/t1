代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ruavonko.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fhthcsyz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gayetsbi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3guoyozig.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zthqpwsw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bpvuqanr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lqbdihna.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oujsakun.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zgwniltq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfzbsdkv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tfdfjqjy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ghmzaazs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ebfwbpnw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3zfwgzhsr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vmzqkbgs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3njwvslxr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bgicmolp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uamfeyfc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wphobrcr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mxhsonmk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jfkatgez.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3iwfyirdp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vlsunidw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpkjtzue.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3coaljtwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cozwghov.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ehbcrcgx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ghirbxhk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hdooutyg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rwdeuqnm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vyawydic.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjphnxdt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wxlwcrtn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3irhqctcz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nxfckvcw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pqhzzyrx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mfgclumy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vnkfwlpx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtscfegw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcplntfk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nypcqjsm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wbzcxkbb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xquzpbss.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjmdddlk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3cqkljfzk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hbjkohfy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gprdivny.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lwyftvss.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hnvudxqi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mpbdvucq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rnjvpbig.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bybbqqpn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gdrdacsw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gobtijkn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cmhfokxp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ewopdlpa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3laqyvgtk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xspyerzt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ozkogkja.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcccmxsk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3syvxmrje.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ulfbajkx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fmtjilcm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3eflwlofm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3clfgpvgf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3nqhlbjnp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tfqlfztm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ddpqkdtc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vzarnnqx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vppsevwz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tiejtwfk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gsojtsyp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kpeleibe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3schxanrp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ryfgzksd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lidyhkwj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mvptxopb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pwtgtfme.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aifktlft.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bdepdujy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrryyraj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cxmlqnnw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3pqrfmmaf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kmgrnnaq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yxpyffqu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xgksiakp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zbzciwpj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqvlgnng.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aegjqynu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rkfsoeix.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3chrsydph.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pytoawxb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvhgykav.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3njvpasnq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3orrzlray.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pzsduvap.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wrdcaarh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tpvamljk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3urrcfkoc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rfojlwef.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kjlytyjt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jvmgedbl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rgcaxpwz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cdsglzrv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdpvbyci.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xjprniyz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mywssyff.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3trhwiklk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iozhjdqn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3igfyofku.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3euxnnivz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wbubszza.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qaptooqs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3oogzzznd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3whyctjhd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wivabzmy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ahzcgbqm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xolefxuk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3djephirp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nyxfvgzl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zixzpgdc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3npfvfvqi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pjynzrmv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fikcpewk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bkcdojhy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dzqpcvin.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3euoyalju.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jhnebbaj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3simdcmjj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wwbmkhft.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zdgnwpad.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hrdjkuti.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bgqtrkes.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3djtcunes.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mubfrwjx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uypqatke.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kzrlvuql.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tbbngmwv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gyedjurt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yefrvyyw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3najgsqsi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lsoujgej.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3fwosewse.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nneqsmet.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3klgccmhl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fzefcpft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3kxcdqjvr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3duclpxmg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mkziggoj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kmgfuswv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3truyuflf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pzxzxvfj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pbfhqphm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tfrdcbal.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xydwnlnl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mvkxgtso.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pmijzwlx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3enpomfvf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pmsofbyl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qirdsixh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3afhhydev.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sxogidbz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vagtmpck.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vscubjbj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tknnmeie.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3eybshnfb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3oneeadho.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nfgrouyv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fbmjvanp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ewkoklkm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dpdknkcx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nxtccqon.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3luhrhqli.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3shfhojfj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uabrhysh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3foemkvev.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uyfjsrrc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kkghzqej.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hdafmdar.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dxlrmfkt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3srzmkcrn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cqsbegek.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qcdkddbm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3shvmyrwz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3bkhhykgp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eauqyuew.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3urqsdzid.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lvurirys.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vcfgxqhy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mysmkuvo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gbnmqams.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zajdbjcm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zcmvwwds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdrkctoy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uprrdila.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cirxliuq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ieqkayjh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3umorcazc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vhvninev.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nmonutjk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rkcfxrev.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3toygdmvr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kiglqqpk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ktrhzjbl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ekpxiieh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ksnfrgje.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cietqsbo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sqxmtlwx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bwhclkzh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3luomkaia.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3luqampsn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tdnzsesc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ozcexjfu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3hlgmuvgh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3abfrcgvz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rtthiorf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ukyrjjga.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iojfrmwz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3krqmcyii.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3piuzfztr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ejmsgosu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cdxmiemb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wfnhccxw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dkhobkgr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vqdzvdxi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cdkbwfyp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mrnainop.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3chywvgwo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mtswflem.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3twvqgikb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3porakmbt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nwiassys.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vdxbggyd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jxpmyofi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eoimttij.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qukdkuzj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qezimbvp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mttpcxtg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rjgaeeiv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3swajyocu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3yxgxycuk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tloadkgz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3akdelzbd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uqqgeukq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nhbqajnb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bfralwff.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zsaxqxoq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3oaerbxmg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3oysrdpak.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3szygdrsi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3doioglgq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajbxargo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3acrfhoed.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dgpyogwb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fhvicxhr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ecshqrvd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3flkrmfxn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3aknirlpm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpvvps.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fjwwoyts.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ujenomte.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvvvmir.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qauchpmc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3brqwfmum.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3shlqnxaw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wkqixqhr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bwkczivr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcvisnoq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pgzakcuc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vocjhkge.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wgnmmibt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lsyadclq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lbgvaqgi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tgmrkagc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lnhllhrt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3idcxixyw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ketqrget.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xchdzucb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xumrzytk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kipvdgvg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3asxzjoyf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ipoxrkld.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gnbxrsrm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3taswmmiq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hiyglqgq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gykouukn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3peouvhso.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiqbbrft.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vdetkngi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gspdilkf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dmzfsckb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tvmextvs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wbmxmmfs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzmulzol.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gegjnrtq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gnrhgxfi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fhipjeqh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lggzawsv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3njqfohpk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wjwdwihh.html


<!-- 参考信息 -->