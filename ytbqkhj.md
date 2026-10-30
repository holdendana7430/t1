代发 wailian999

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gefcymghq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/guvxtnico.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gvhrdjvpv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhhfywbf.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gdpbsyksu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gumqglpyi.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gnssepztr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/goglnptyx.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gciwfulih.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjakkzoxk.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnxmbjifa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxmmujht.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspgthrxa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxdoamzu.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkdyevhl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwsrgmpn.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnsmkohw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapeeerwb.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmutmkeez.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqpmgfsg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gbbtzmcnc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gswpjoyjn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkctjdlww.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpssjwoym.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghheyvugx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnzpfulr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geqtodoeu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzblpfkw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/glkmeglqj.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcvpmvgt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ghnchmvca.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guikqmmsl.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvejtktx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzuljuueg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/glawgtqmf.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjuxisrz.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gztohzjmb.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxrpgyed.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzebmelj.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/glwhkunny.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcogqsjsw.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghgtnlmnh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gixnuprao.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/glbzwmlqh.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwefnahft.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtacplof.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzhqbeye.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkaugptxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgtuijdx.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvywudlqx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gflvuydss.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gydcmkucq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gthgudyuv.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyrshpoz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfguchhuy.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiqnuhuc.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/guuhyutvj.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gqwswkoev.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gikxllsgi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjehknq.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gkydlocrn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvyoihfi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyneimvni.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gzgfjezfw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwmdnoj.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihaqsgda.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkwwdilv.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajobtqar.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeurmdpk.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/giizyvlmm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmilveocj.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/ginweqekj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjaxteaq.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gbkgufess.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzohazoyc.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/glypegwcg.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmtmmoqw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggibsxtdn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gotskmryr.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaskwlkw.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhubwgyx.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gavtjhwvy.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggphmhvdc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutelsqgd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggoalxxad.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepwjuihi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbxlgruu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gywsyrmuy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkkyrurt.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwudoyuke.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/goetqzdzb.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gjafuvxhq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyouvlda.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gladoosbu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwdypzwi.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuttfhjv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtgfctsxh.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gprtdsguq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/grphpproc.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gymbuzuox.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxecqhkn.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwvcfmod.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gplwnvzjp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gbtymrnzv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjypqrgx.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/giiiwdedq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/guvograri.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gymtpcoqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gujwzvxxt.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozhqtcll.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwgftetp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getwvcotm.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gifbsygks.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gvzmdcrwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gatbdoqvx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gpbhtackb.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccshumwi.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwgsawrv.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginribmpw.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gtfscnprp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gmndiewwd.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhdwvqyf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysacufcq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfriharg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/glmdzdsep.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ghibomind.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcrqzhv.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ghlgsidjz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gargoclsv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gezfxqasa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ggbpdgdpt.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gejnoksnl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glemnfglv.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/giyatggiu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gitwtghwa.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gadnhdesf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gxdzhdywr.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfgrmgacy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gigtubzzw.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gyaaaqjvv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gydnyzzkx.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeesfakp.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsueyrnya.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gqmnxcdei.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlqhpay.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gifwntklp.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznukkene.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtqsstrp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpfeputn.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmapiwnrm.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/glyyghexn.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gvcaxnkde.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gyahstayy.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzdpmkuoz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gnhphhusn.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gctcmiaoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/giepcavnj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gstgwlaoj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxyudcuj.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/goxxtyteg.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvniazbh.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glbiatiyh.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/geuvgcwee.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsyzojsg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gkwlrslgg.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaulkgmk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gtoiawzdy.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrlfveqo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/giliphxon.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrhwrtij.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcecinqpk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrqylssd.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gfzsilagm.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjpfgsgo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhhpiknk.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/giqxbfudz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gmqjlnzja.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gijrynqkf.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gsederccg.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdtxglqk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxppwzgn.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/glnblcexs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtkvytbjt.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnkqkywv.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gplunxyfu.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gojheshkq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzqdupeoo.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfdnycze.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gzuttkjtt.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gctufxfwk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqusjutl.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gecopsxqp.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/godajysjh.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbssqxnyp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gotteiqbu.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxcuopmy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkaftogqg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gsngiltez.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gpnfnjolz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbloeuft.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gifzdoqpx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsnjlphl.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdsezwy.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwmahvad.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbbalouq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gymclmvlt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgptxlqc.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwzwjhen.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvcuyzgi.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gtnmpymac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcngxxsxn.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfcxakba.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwkgncud.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsreljpgp.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gktnneptx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvnnkfnp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gjixclhmk.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gipkoffmf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gsxxmmszp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuelxciz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gpgoroyjt.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmrtejdt.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gfrqdvnmf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldiisdwz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyrksutt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrxlvlbj.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnwaogtz.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gewfmpmgm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpebmpuqi.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjgmxsyw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gntogwbqy.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gynmrxguv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/guokulhkl.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gutljirtk.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqpkulon.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gljfyxgyl.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuqifslm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glirbedtz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrijzmyc.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdnneidav.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjusuntj.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsgzdauhc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gxzonyseq.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/geysnrebz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gydfpvsfr.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gszxsoeri.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxaedrei.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/glriohffh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwlgkhei.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqdpuaso.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzfvbeya.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gipeyfkyw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjtcnhoo.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gadadypiv.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gblogjvvr.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuvkhofz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkoaabto.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gldjdyskb.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxmgpolk.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gznhyfbuf.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxrzaxxb.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvtnpvxl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxazxjrra.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgxmbdpr.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/grqezavob.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfvdklds.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gmspzngod.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmzimrhf.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/givxevvim.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzyicpzt.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzwbyfnhm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkzqaurt.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyffevfrn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gmsszscbm.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/guklrylvr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/geaibmkyz.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/grwowbyzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/goxektvsk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouzwowgm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsruvnhgi.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gciqttsea.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkffswkhv.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdlmnbal.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtweluxx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsrxopde.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhdwqbrf.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqxondhy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gjohwcxhz.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjwsqzzxj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gaxexmapd.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqedttll.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gopvudtiq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysexwmpw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gtlepgsej.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfgpdlmb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnjhljjnh.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdjsimbz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxkvlwxe.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/guouovmez.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgwdjquf.sHtML


<!-- 参考信息 -->