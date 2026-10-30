代发 wailian999

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggttolrnd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsqthrth.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlkrzsxj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkxsuafp.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/glazmqbgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikzcixwy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guendbvrg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gronchaor.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofgzrfcq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiwkipga.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxbrntro.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgemnhxw.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/geruueard.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxuglfua.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/grpziconj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/giuhlruaq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gujzpuyxh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gknznnjud.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnbjqqku.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gmdhkhsmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/ghnirzjlu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gouldkqyr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gryaksvtb.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gfiedcqof.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gndusbpae.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/golwtbapi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gmjyjayfg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geydoekdh.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gwvtxrxrg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqwheevq.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlayxypr.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwjldlq.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gwezaevpr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/glotxbrtm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpycqekfu.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdoclcmbk.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxbiqejh.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpouqbptk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/grxcufqze.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgqgrzqh.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gceffzpxa.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwkduyce.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glufpblvd.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfnsopqjq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ggnctpott.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdivntbix.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gabzwnbdz.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmszffyo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gejhpbtpv.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnuwekded.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvilqcdhv.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtfiuqqe.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncywahxi.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfedflgqf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/guppjpozt.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvznqbkam.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsayuqjqo.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqbnjsoaf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpntsvxg.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmvnvzcp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gerppdubr.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcihkwvhz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geqdpydgf.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gryjcchfn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpjipnyy.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpmprjpkf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gehugyxzo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvostvjbr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gackiosnb.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmtmnjrr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsybklhoz.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdrskttau.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjjjuyii.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcenfuwt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfkmfrech.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbnsnnox.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/grbxbxswk.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavzmsisi.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gotmrgcoi.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqslmnaoe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnqqdkqhl.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclwczisf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkjdhxwpy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwbgiubf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogcjxtmb.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglxtwexz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gckeienps.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrwlqlyg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioferkky.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfzbsafo.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gltdeccqy.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrsllftm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhmersex.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/grxlvfzkm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gugdagqfq.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gukadkqwp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjurfubdh.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/golclddnl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geeaxltuk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgdxbhai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gisqnrgqe.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/goiovfixu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ghjdccwve.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/galtafysq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gkyarmlsp.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpdqwsvps.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/glqajqacg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmhsnjfq.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbqogpbyg.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gxkmxtbme.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzgsxcs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnwkdhy.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gjceggmlz.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gkziigzju.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/grbyjlolp.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxxfvlfn.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gautdxitj.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/guvwnnggg.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxvlhilk.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/guvvcfcsn.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gelcuenwn.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmkzeggvk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gibhqhvrw.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfakkfomr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gkbyvxwfk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogijhved.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhjyiszr.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gufodxrmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggencrywo.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyetkuvjw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebyaanvk.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gcfbmddfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gkezzzwgo.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gionhmdxz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbsbxjhdv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhnggdz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/ggyahdkhg.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gutewprsq.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbfbvacu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gtcpnosjt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/ggdgymlhq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpnkwtqzl.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyznojjb.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gmixptinv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gtffpixve.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcvcpmfk.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gttnbsxgg.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/grssmaksc.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdochveb.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glrtvqpok.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/grlrwaqkt.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gsoflxgwy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoirhhjd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcergurp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdwodzqj.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gbzroydvt.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gduvhxecb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gednabkeb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gljyomncj.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gshlqxarn.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gyifouoqq.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnodocgpg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gerddlvil.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomuzpqgv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdlubmdy.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeihmoga.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gthysqlcc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiltjcza.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gdgtmaone.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gqrowyaku.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvtqzsuoo.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbkzalbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjveftzxr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdntjvdh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/guldlcvot.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmycvaxeb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/giwtxtrcs.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gaackmqjq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtzoohbfm.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwqaqloc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbtrpsnw.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnthgoaqm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfmpqfkrv.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfvnztqhr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gghtftipp.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoahdnhe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/grtqcipap.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gejzukhbl.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkaiuoog.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gglyoyazf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbkqtzjij.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqynmuki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwwybxabs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gaphhrgzo.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgbwzrsj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnhafoys.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdynnrkws.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsffodey.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsuumtvc.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqefwpeyh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guepntsgq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gslrrproi.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gcprfbszo.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gvbtelokk.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gyoraniwh.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbipijw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacjqdzrl.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbjufsxuu.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhhsfzux.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliuovpwi.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvkwcday.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmsaezpri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/guhjckwlm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbmydwro.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqhjgbvr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuyftqcq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrjdzmav.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gayriqjvr.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gtfeeuacs.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbmhtzqj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnpggzuv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjwkcokcw.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gqxgvwvof.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gshkyoqvz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwfobkcb.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gxhesdghy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcovvszkz.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpfmrlfx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gunvveuql.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzfujiba.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gndmlblrz.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwatkxam.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwcsgtmsx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gekfftghk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gyerudofw.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfxoyyhj.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwckhdxy.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfmpgojr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/grzwcanwr.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/garrtefie.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgsbnadu.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/geheldiqs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gowuvrsnv.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gnqbjyhkd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gmljdmhsc.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/groiutjxf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqsahzrab.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuiynkrn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gsblcdyyv.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/guzheooct.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/getoyqucp.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrthvxyj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxjdnrvg.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gklenemae.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyewbrvj.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gclrpbqce.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/grwdsatua.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxsvvlkis.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gxajvwtqp.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gcmttqzkk.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwznbjnmd.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/grkargamg.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gohsmpmrb.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfytvslz.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gijpluvbm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdekojnpy.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdayughzq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gzuvouvjy.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gicwtjlzn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiagnqnf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gberdeszy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnjzslxe.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjymzzen.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvjmaphhu.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gsugzkbdf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddzobnsb.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gvuiysvcj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqivihpa.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemedamp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipqtshlb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghodlyvur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/glqpkyuas.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghszfwxcp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwgfvmju.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtekihokj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiywkuab.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsvkghxzs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gqbsfjxdg.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/grxyqelcf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtguhjesv.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/geoveergn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigituabf.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gggspjuzy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gdxruwklt.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzylggbqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcevsdpkd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvaoaukd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjdwhwlm.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuitmjyo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqhpetoo.sHtML


<!-- 参考信息 -->