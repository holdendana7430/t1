代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xvpfmfro.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cxivhbwc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3clygottq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vifkuxdd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3axbjkhes.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3erkanasw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zjxkaoqj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tyolbjfd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3akwqehhk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uljtlfdb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ovdavdgs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3wddmzfks.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hsvoecrp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vozhcqoi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bnqrcrlr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tyrhbxmw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3obgjblsd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gkrjqfll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xppxnbwl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hszbuhbi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3eyxuojxa.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pnqvgvuj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lesvnwdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkuexips.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vgruiyde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxtbruve.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wmkvvjyv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3oogvdxit.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ihxnjlzw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ihkzhete.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fbobasbo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcdneosu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bazcamre.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xixathca.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3etpzrdug.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3alpfnvyb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ztmwwimu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qnvbghpu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oznrsslr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pgjyhheg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qrcmcuyc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ddlwjkon.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kkizrmwv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ofmafucn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3inaeccgc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ybnnrjrc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kemjoaji.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qptbvohk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3owhooftq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ohcqncso.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pbuhcjjc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dkhjyjna.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ozvnihxx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxmulkjl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzaglpmf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3otcsdcub.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xyhniauh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zpbkwgzc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nwukfuzi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bmuxgbcf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3yynvmdee.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tfdbqczn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3daiyslwj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3acmrwflo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mfmxqqcn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3omncfvgc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3amfpvtrf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eqafurbl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gyzhgkex.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bwgbzzzs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vmiyxvlo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gautpzdl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zvbcmsyt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cyipwmqf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nkiloomy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wmsszzey.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3cljjsone.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sdsmzptn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jvbgbzni.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3cjzlcrnf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lkzakkaq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gbkrcryx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xubigkal.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wsprlqaf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cjzfgrpb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ibzurufg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wvxvbouq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3afapnhgx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nicmqorj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3stourlrg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kvjtvial.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uyunwtzd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jmffhxoh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3nlzjwftj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xtsysrwh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tfogclsk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vybarrjt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3eykqzsgz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3svzdktwg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wruvoqis.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nxycwroc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nowcjdcl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dqdpwwmz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rrzvdkvu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nebluvsy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jshepmoy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nrhtvxli.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3arpqrgqi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3flvoszov.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qqyobyxc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vaqbacbw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bkpzyrbk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mlawldai.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vnbuosbn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zkbuqtja.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wdassoba.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bmgjgvlt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qbsacbke.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ikclzemr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ohbnlzyf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jzmkkqlr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3agwszfnr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lontccoh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vjvxnpgw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rbbzrzrp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lrmhpwqp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oueovxii.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yfkiihjt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cquahyar.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ehqltbad.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uvwjbgsr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wkapthqj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vnofkjan.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3aexeyyqq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rdvjpqms.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zyuvvapl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fyydbcdj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3leamkpvx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tiuwrqmt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rlnabtvr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hemaswso.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vzprqtxv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tmioglxx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jlwhwyyb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zcqpfcop.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gdbtxsye.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lmazqzqc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wudvdllj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3crjyfvvq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xgiihmgg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3opmqevnq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3erjgzkwv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jwtmlmrk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmzsuihh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3iucmkzzk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lnudtljn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bqwnmtcn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3epyodqec.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zboisumx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hbeuyliv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yqdoabce.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hqvevjbk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wtnssdef.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cbnjevnb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3alwbtpko.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fiseithk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rbchefuv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jwjbyjol.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3pmlrloku.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vttowuwa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ykicjhhf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gtlhueti.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lepoiywa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zcubszph.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qvknezks.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ozzniply.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rjujqhrt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gimpoaov.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lquvhocj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hprqfuni.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3coieskoe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmmjowwj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hruwiqfq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ntdmwbeg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bnwteyre.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rvdpdbxl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hyyjcjcg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3knpyysnt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qglyplay.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lltuhvzl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fvtvijgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otthoxdo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nhufxghq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azwxlamh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wxxfoved.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jvxgydvj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3fktpqduj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qwhqjgxc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3oxzwwaau.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3owrdifgm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sbaqudsg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kfezibgz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iqgtchhg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3utooyscj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3llbabzkm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yqekwbsj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rftormgl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3prlbuqib.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mgbbvxke.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nvasoazd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tjyndksk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cygjtzqc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gryoafqp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3plejnmdl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bctpmevn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzxwwasf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3snyvzsxv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ocorgrlf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jrynvnth.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tucfkmzn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lknckech.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ahqbfwgr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xvmrkcgt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jekwhbmk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mwmmxhfz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gcdxlton.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cgpmnbmw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mvtazhwh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dgsfyyhw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpcpprea.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3abqjdplq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wzlaclyp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3aqgkxfiy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wutxuhnt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vmtnuumr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3izxsryil.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yvgzppew.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zxxpmmow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ioaevmiu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3abisrpxf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oueulsex.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3irygnyvd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3piewbtvi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gaukrrgi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cektkxdc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3isodpuhi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ewqbbloc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tarpsrsu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vvokqpjh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wtlmciow.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3beqqzurd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpcebfge.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3osrnxonw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nfknuune.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3weohmxaw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cfvrcnwe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zjykloep.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3riaumemw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rpuogetd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gtkqlkli.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xvtvxcod.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zituyhnt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kvqqxqtr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zskkvvxi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zthxxjxc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xwmgxrfy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3owsstijw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uasxshfl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hxadbepp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pjefabrf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jlhezytg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qckdzght.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xffzsbef.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ibptbxks.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ajrhbust.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yxuurblu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3guyqihqu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3oirtfyxg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3axguynvk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwpkkbpg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jxiyjsjb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mowehmxf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3alyztfom.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3krvqcjju.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eidguorh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dbrmphkz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lpomogid.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfvvjjg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xynmivsv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kkkfzpla.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3aycnlsbl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdjamkrl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pmivvzfs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qrypailq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jmdzdsnd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mctitauy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uductdfg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hsjqdmpm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cpcemtgz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ekxrewza.html


<!-- 参考信息 -->