代发 wailian999

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gtituynra.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/guwfiqnsp.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gmkutvncn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gzyilwhmi.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gypftdotp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gamuocybq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gcnsutpcq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/geywujfoj.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gxvkqbmxv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtgbeffuj.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gcxhjsirf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/ggbfaohvu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gjgfhzoiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqybtzxon.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/grgkaknwz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtfccplma.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gbnykuins.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gfxcuxxsg.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gxtxcqaga.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gpsxjsybt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gjsjfdviv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gkbxajxex.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gwtsjaktl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gtuodqnos.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gebvwsmrz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gjmbjurct.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzcusecof.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gtvisynbs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gakeojyut.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/giczsaugt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/goplbhcky.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzfbsrqrz.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gzdxlgfzl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxuulnihb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gfavksebu.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/ggzmigdoj.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gybjrmkhw.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gnvdnmzaq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gddfjttyn.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gipsieynb.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gcdjlvdxn.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gosztvwlh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/garsmaocl.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gznflylgc.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gmjkzgmrc.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/ginimhtpq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gqcuedttb.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gfkziiyfi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gljzzqrpn.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/ggrogkixc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gfufodvzx.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnlvrptvf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gbgdrsxxs.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gosvfotlb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvpqywpxt.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gvotwvvkt.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gvwtoytmm.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gnrmidrrc.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gvbmogzkp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/guxhdutah.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gskqzfyra.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gzvwihlcn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmxnwpwcs.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/grvkmgmto.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gazfwyokb.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gxkdzytqd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/guoeygtdl.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/goykeujvj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/groagjvjv.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gpknpswio.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gomhezfbg.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/giwdytijd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/glsovtfjr.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gwonugyjd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gmkzuoviw.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gdcvssukq.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gfaqcfdtw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/ggulriguz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gvnusjkls.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gcuxzofux.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gghvefivs.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzxysloww.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/galpxapua.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gkrziflzy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gewginokv.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gqhsbvoxd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gaaqpraxd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gncaljhva.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/ggacdsaeh.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gelgqjqwc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gymxhohnd.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gpskguekl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/ggvbalego.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gapfzmxpu.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gzowfttgd.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gqsopuwrh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/grcopgtna.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gvnozntep.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gxogdhmrd.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/glvsmzwvj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gdczfoyfq.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gwgumgxsi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gfpqcmdxy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gsszldayn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gadmmmalp.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gmvwirfhk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gfyxypjms.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gpkaxczry.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gcxgkxgma.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/glpnkpcuu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gtwllvzmj.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gmkfyhdgn.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gkxvekvjj.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gadmjifyp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/grokctcxe.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gsnaoaijx.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gztasziju.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gqugvjhtj.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/grecjiwrq.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/guftuhvon.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gtuuysuwz.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gnauxrfmh.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gqnglqjgg.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/giisaljdk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gtabrytsu.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/ghmjpvfop.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gxwjrouhx.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/ggsbkwfca.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gkwdumspn.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gqslxyjsp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/genpswamj.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gyprlzprh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gotikmyhm.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/goziqvsdq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/guvgitunm.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gnagjkiif.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gehzmjmjr.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gpmveyfia.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjgqiuwvv.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/grnsktqsa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gmafgtnqk.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gyddsdamn.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gokrftshc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/grjrxxpmq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gtgtvgxkk.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gjnutgtnv.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gkuoolqet.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gsodcicnu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/grwlsfjyr.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gekertjwy.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/grqxupgca.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/guywoaves.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gmljsdhei.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gkmppxddf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/ggpekbqka.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gjrvfxqhs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gbpfjfyvy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gbytucgjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gnzxuoeak.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gsxccsyir.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/ghbfrnsxt.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gwfexglhg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gyrbhdzay.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gbheylrjo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gtshycrom.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gbuakmelz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gdlqppzfh.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gxlplwhjx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gqxnuiuyh.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gvwnmsytq.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gialrxwuh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gklbjqjaw.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gyzoertzv.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/ghnpjrrrm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gfdwznqno.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/ggrzclhhg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gitxkxufd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gwwxcrjar.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/ghnzhqnjf.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gmubsdpnn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gploqqqoe.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/ggudlnwlf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gdvajrlws.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gdkxonwpn.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gpmrbczgp.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gmxaggqqq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gywlpamqo.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gtytxvhyt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gqwrhooed.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gtidjfofr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gylsrfymh.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/ghxajjlii.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gudvnozta.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gulcpwezt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/giwjlytsm.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gxkpilaep.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gqxbxawpw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gdzkraihx.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gaeygxqfa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gttkplrqa.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gxoyuziqr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcdcndvze.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxbaythyb.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gylxrihnl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/ggqpvmkqx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gmxirwjam.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gauuzhgnt.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gyhuabpap.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gajytythx.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/guhzscaja.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gvnawafqu.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gfwgnhydw.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gdzfxufhj.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gibrmtmgb.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gckqimbtl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/ghtumtrhm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gmyvhyhdz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gjexxwsrf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gnbebzvmn.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gvmtmnodn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/ghbjfintr.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gudbjgvmk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gkkkzaxsm.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqdhlhwjj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gnggfzfhj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gywtyvbkg.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfmovmum.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gylywmaet.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/goegxidwm.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gedhzphxi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gkcyhltcw.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gwtphdony.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gpxejhbzc.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/girpsqotj.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gixytoggr.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gzpdurwhy.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gumsqatnx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gynqtezra.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gdihudqet.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/goosurixt.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gydzyjvyw.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gsvtvjsdn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gevogxyye.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gsbybdldz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gqkecjrhg.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gzcwdtrgc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/geaplazwt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gsphedbyk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gumzvhnod.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/geiswvaso.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gznbesjnx.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gkiuhxafh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gbvpvmgmx.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gbusunxke.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/grnazikad.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gwuysxeqk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gilnhkuqo.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gdzgnfeil.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gwftlbyyn.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gxturctab.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gxnrnvtxw.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghuosadjq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/glsbcgjej.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gfxfwllpd.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gifsiaztv.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gffqefnis.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gsgkndkuu.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/giyatgyrr.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gkszhpyus.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gccrwgvup.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gdauzzwal.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/guestvtki.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gezsfotwd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gaizldyyg.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/glhejskis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gyqnzrzaz.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gcrgdrcdy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnlecddne.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/ghnqhfzkh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gprqkdgkb.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gxuahzgps.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtblpjvmh.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/goazibzns.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gqhhdoezd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gwvhocsbd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gulldfolg.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gmcmwtfyb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/glfxwsnrt.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gyspcpjnb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gcyhbocia.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/geuptysgs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/goxbhtizh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gluzrcsve.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/guihycpfm.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gabxwemwy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gztkmzgdl.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcgshzw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gzhmtlvkg.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gxtcximfh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjacaoon.sHtML


<!-- 参考信息 -->