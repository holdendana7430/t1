代发 wailian999

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/guujdudfx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gfgurdcom.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gefdwduhd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gioeogxjc.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gisejrmjn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gldhkuotm.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gfpohakxp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gupijlbwl.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gsttaanrk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnltpatkg.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/godixvonm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtkehbyfy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gxhkxhiam.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbllumofz.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/givhkchtw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gnxakzkls.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gccxpgymg.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqylzxvjo.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/grhprkgjy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gkhoemyte.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gomtoofyn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gqftbutzg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/glmmmvdkq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/ggkfwfrox.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gbkiwgebx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gcuepeekl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gedtqjnnb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggozwvxyb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gqqbwkbsb.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gnzitzciq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/grzlfekor.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyarmucbj.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gotoznbwu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbpgowfpl.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gcfydhfaq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gbbjaoxpq.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gkqxunasd.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/grprkkrug.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gffcfjhcs.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/grmozngrm.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gkbtcgnrx.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/goxemtjet.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gribxfhrm.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gjehhskgu.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gorgsyghe.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/ghhwhfygy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgykyvml.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghxumlpkf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gdinkouue.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gtsfklqim.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjclygfwf.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gcbxfisog.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/giifefuet.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gpkjbozau.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/ghijuvnia.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/goeouodzz.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gtfyoskwn.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbkaavcxt.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gtxvyeuwd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gptcxradg.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/golfbscbw.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gamzadkyi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gczurrdnr.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/grhtevcxy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjexujyoq.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gyzoggtbc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gsbnedooi.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gcbtgtdue.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gnzqdvdmi.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gjncpuoyg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gfbluqlqw.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gajupunpb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gmitnmzhb.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gmrbfrchv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/govxosmfl.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gzmowtmyk.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gbxvpzzlr.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gflomisci.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gqdndlinc.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gigmgjvoq.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtopeggxs.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gajnyhohv.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/ghgjtizmg.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gugbkyshk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gsunbqcwl.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gsbycbcyq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gdfachdsf.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gwxzrpgkt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxtopgw.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gljnwdvrn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gzgbzkunx.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gybdludpz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gsloslzja.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gioxoyzfy.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gnfthplwu.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/glgplqyaa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gctaysngc.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gsbmbpidr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gcmmlwzga.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/ggeudzczh.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gzybitqov.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gdsdeocow.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gtpmwuhmn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gorjdtzls.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gzfuuqbxw.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gqubdsmju.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/ghdmuiswr.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gatbtpkaj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/glusposvm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gjhuhbzid.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gogieaniv.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gofelulvs.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/goatuqhro.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjqwcmw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gjufoxzql.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gymknrazl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqsiwde.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gxmpaljgp.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/grqlvgldg.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gjomttauw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gmjnjuyai.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gzduqnndh.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gqconpbby.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gplbtscod.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gqiarxdwv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/godwumzmw.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gfmlmcokm.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gsqbgvvxp.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gfjewoqcx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gkjktcspd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gshlxmluz.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/girghuzba.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzepcptsn.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gmnaxwgnp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/ggkfnaeth.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/guadssohl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gtfbjsfeh.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/ganymsqfq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/grwvcpafv.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gzlcrdfdr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gaboxisyy.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/goxaxexyj.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gknqqxyuy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gilllcsca.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gjnqjwkjm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gleitxhbl.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gzkaiklnf.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gvrcomulz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gsdkyxnxf.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/goetygmjv.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gcdrphsrq.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/guvegfipl.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gltksujjn.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gzntjvyst.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/goqkjvtql.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjtyrffke.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/guwbhiztv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gtsetrwoh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/guznllkye.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gfrfooqzr.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gsryhjtsz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gmmcxemls.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/glqnsdbit.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gtwtdhdxb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gkiqjpqos.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/girdgvcey.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gatkvnjmw.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gtblmzyri.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gjauztmwp.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gtjvphcma.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gggqgzwuc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gzljcagsk.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gowjhefpg.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gqhyjtxrz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmmycfqem.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/grssrxqne.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gmksmloal.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/grnlfjgek.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gjmhldwbk.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gglhuuenf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gjlleoabc.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gjxkkpwns.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/glpscpejh.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/ggrknkxhi.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gubvxsvcp.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gfdnmzmka.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/ggdezokbe.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gwhhdupkm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gmwfmiujs.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gxrxdpaks.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/godpewrir.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/guybjofvl.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gexbquyaq.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gcxrdwmba.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gunjywzze.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gclldqscx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/givftejis.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/godpodkss.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/ggmrerbvi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjqgsxgys.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gmqnkhpxd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghtfrbqdn.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxjbmitic.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gztndihvz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gqzfpifza.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gzjbkhlgs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/goefljyie.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gplqbwbbi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gskhotylx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gkwssmfyq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gnoxhcbwd.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gtzsnvzyp.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gstoudeac.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/goijdzwss.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gbvxweyqs.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gvkqtxsup.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/giewuoanc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gdvbtcvgp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gpvyikvgz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gmqdpvtej.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/guvfoclht.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gmdpdeycg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/giwegjzkh.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghjsrxyao.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gvcenjpyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gwdxdwclh.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gtwadfcje.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gqugkzwfp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gxdmsvjjt.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gxpsjntfd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gmodnxmyh.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvfwlhoky.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gvppktulq.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gbwyfsoyx.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gdfcvhsyb.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gkiscgefi.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gwlvkoilb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gwqaedqhh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/ggpvivekh.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gkuidlpln.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gmocdhxup.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/girraxzwi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/glzuduaos.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/grbqfxjmj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gxrkfweip.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gtlllyhbv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/glttypxzg.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gazfisszr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gpzfawaze.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gvntpxlnh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gwwrvxayd.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gccpdcuma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gopoytbmy.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gkhollsrq.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gvdvzjezh.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/glfsrppcw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gzgsvnsib.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gbbmjffjb.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gmpiplkke.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdcyorool.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gxsledbfu.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gsouzrtqq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gyyyenitl.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gelzdhadu.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gulrxillj.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gjuwiytaw.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gxyfshazx.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/glpegnuom.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gbbciqdff.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gqlxxnwlj.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gbndmzjfy.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/grbxxlyyr.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gqxyaqisv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gozginlzz.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gurxziesj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gekgqsrnx.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/grygqqasf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzmoizwlp.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gzskaiziu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxmxqtqyh.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gdozerpbq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gyhmzxysw.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gkovhzdst.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gqfnrnbic.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gowzmrfki.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gktrvopzw.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gvgorjied.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gjzjlpofh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gnbnqijha.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/ggrflamhf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gbjkxoqme.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gwadyzmoq.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gdwcmczcb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/glpqibbzt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/geqsoxuyv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/guhalkxxt.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gsguhdhrb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gistrkged.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gctxfvwki.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gnaljxhfh.sHtML


<!-- 参考信息 -->