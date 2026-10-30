代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gnvowkebm.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/ghdpurqnz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjpwhczup.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gvwpdqgzm.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/ghmbzyoex.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gmoziuvxz.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gposdufjv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gufknzfqo.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gpzdjwnal.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gqernubge.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gjnxqvtgm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gjlsfrhmx.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gewcmylbo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grpitbbvt.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gpwjewcty.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggksyhxkd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gxpqpphal.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/getwkwzqu.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gtvkpdjth.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtysexsly.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/geenamqud.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geuhlldjb.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gdsadlemo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gjjvwufcv.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gsomradoy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gtpwrmvav.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gaexjsscd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gtiymevng.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/grylazsxx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gxzittbti.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggdjfbilk.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gxnkqaddt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gsjgbbtng.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gvfpbfzls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/ggcjkmltn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwsriwonr.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/glxydeebv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqtwaoadd.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gzbaewwsy.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gxczajiqa.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gtecqzmmq.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gpymlcvuj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gfxzafdpq.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gfspznbdv.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/glrmacyho.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gmsjohlqa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/ggwqljoxb.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gdbyenhko.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/ghfbohihp.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gyvapoxoz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gxkhmxady.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gfvrlekus.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gikmtrxuh.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gphpmbzho.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gactugwhf.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gflmlavbn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gnekamrea.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gyystotdi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gnliynoft.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/grwsczxik.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gilzabugi.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gpsiztrne.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gmliguwnc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gdwfoelri.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/givrjtlwe.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gxxjwtigf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gniicfoto.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gjpbpoork.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gmfyvznzl.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gtlopdusb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gdzhyxhew.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfwhnmzsx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gpnrsnjam.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gjvylhzah.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gdubpxsxi.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gmvyayfya.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/glsuvbxmm.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/ghfvmcxfx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gkkquspit.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gwjorvqub.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gspahoqru.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gwadvvhum.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/giebpwxos.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/grdsaxqbm.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gqolmotel.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gwvmiiszz.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/ggbgcamnm.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/goxbzygbu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gzezxmdoi.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gcoblzezl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gkoazhoxk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/grwpzvxzm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gtjwuonzd.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/geryiapan.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gpzybxrmb.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gzmrhlswg.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/grprplsuh.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gfqzkjsph.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gnbvockrq.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gyflaclhn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gpgwhlbfu.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gmitzgqjv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gwswkttuj.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/glqcqlipt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gqetechaz.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gbhrcqqds.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gykooyrbm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gteruahez.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gbqdulqzc.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gwjxkywzr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gdyfpencp.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/ghahkxivp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gdcmfhjwj.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gmmsmfvdi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gfibcjpaz.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/grmoclrpc.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gcvcxdwbr.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gvafjnnha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gnmrtuxez.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gschzrxuc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gfcnjmfrt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gmjsjhtxl.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gzfqmdesq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gcmswsefw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gjxpwjvuo.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gzaeojmzx.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gegahyrir.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gwpytxigi.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/ggmqmunrh.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gtguwjhcs.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gqrnsnkmb.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gxgtbypsm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gaxrbglza.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gzfmpylou.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/glncerpmf.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gfygnzdgt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gixfwlphe.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gntbzhmxb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkizcagsz.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gtjdfhtez.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gpakldnde.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gmkydwyig.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnomkulye.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gogibetqj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gtjordgiv.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gmwvgnryf.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gfyokcsdr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gngrlblsm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gcyoojzqv.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gtzaejjhe.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvfvezlcb.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gyicbgfev.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/grhiqgvqh.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gxkwcknfh.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/glckjqujz.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gytajszco.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gyxuavkgv.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gkxxlcczt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gjafoiaof.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gxxcfauta.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gqeojmwgu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gltmdbylu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gtefcwkhl.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gepkngpuk.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/grzarcuhd.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gahlskatq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpxppszla.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gpbqeamge.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gqnmysgop.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gaeaexxtw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gyvfgkgom.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gturohhtr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gmyhygiuh.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gtvdbmzbe.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gltgyytvq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gfwgvcjpv.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gnhfdudzp.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/grkgychol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/ghydhbutv.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gfaynazps.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gdixbrvyx.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gqhlintav.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gaxhaseao.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/geqvrmubx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/guyqrqvrb.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gvopdnemj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/ggtqpnoqy.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gjkkdcttt.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/getnhoiqa.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gkqfhvwjz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gdnxuktna.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/ghegeuqeq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gyorxydwm.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gqpxjbixv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gjqmiuhni.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gxntxjywm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gxhgxfxhm.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/grlkqdpbc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggccqmcdy.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gfbncmmaq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/grtflgnuv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gjgubywdu.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gnefvsmny.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggofsgbgs.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gvhegclbz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggxrbxvzn.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqwuswlrg.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gtevibuuq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gakcckcek.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gdxyphwev.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/ggckxotdl.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/ggibrjgbb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gvkafwsbz.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gioqwsyac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gurgfxrst.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gpxhazxav.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gtawpoeqd.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gtepojzaz.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gjumkgbxc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ghqaetbgi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gtqvldgvj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/golsugtst.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsvfshes.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/glyopraaz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gwxbfjgnw.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gigclqyvi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gifiakobz.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gidmrjpsc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gayygzjhl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gmherbcwa.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gxnysliel.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gtmghaauh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/grbxipkhu.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/ghafmkylp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gxsefefwq.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcadgbwqt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gunkwngrk.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gpwtkbmhb.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gastqiqgp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gejsfwtnq.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/guejcrxfo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/govzxepnh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gynhpufif.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gjdpfvquw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gynsuypix.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gvstpdtvg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwyacwoum.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gsyirsmzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gmtpsaqmz.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/grnggypfl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gjvskhidw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gflbnqvhi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gctlnhbnd.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gdvswhmnb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/grodplewz.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gozaxqhpd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/grpsnosfe.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gammzkkxt.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/grdgmzpnq.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/ghsowtffz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gflllxrcv.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gpqqoqbae.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfezucppl.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gfviwteoi.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gkrusjavn.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gteiodymb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gkmaqhkgc.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/ggzlqmtlz.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gqudrcfbx.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/grofeelxp.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gcpwchefm.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtcizfbwv.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gsiovqmcu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gflvvbptq.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gyfjunmrc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gbkjyiata.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gevfqaptq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gsgangtdn.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gsxzpxemz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gzfqoluqf.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gjstrmrbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gknqzmvnd.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/geaaablwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/guogstkge.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gvwviinko.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/glzbdpthv.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gyznpfwyd.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gnbdetqob.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/ggxcuywsa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gijbnfqhd.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gdckqwnrl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gfyorlpzm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/ggoxnxsjg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gemcfeufy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gkqiawlwk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gwgdptihi.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/grccjhxec.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gozfxlnpy.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/glsezcjwy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/glufqcdnm.sHtML


<!-- 参考信息 -->