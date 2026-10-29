代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gsfvxozji.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gpnxbhmqn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grgylssgu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gnkkwpqce.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gkyqsrxyg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gycnygxno.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/ggvxjqfsz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ghlclnjtd.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/girobmwhf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gbfiyykib.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gorujyfcq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gdymhdwyf.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gygbfmwfw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/girmgyala.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gkwrbwhqv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbkiaimww.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/givapqtnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzinnzfol.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ghatpbmpg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfwkoxaml.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gkjgpqbsz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ginjopboz.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gxciqikuq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/guuuvccfb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/grnhcdsgd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gphjgxqef.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gfqviyuxc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gzdjrqtnl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gjhzcoigw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gavpzromh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/giwniexgb.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gswfaloia.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gxhdfksrp.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gdgjmvkxn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/ghlpkawab.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghwpmuslj.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gmpeoaqen.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnjgyqcci.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gjutjdrfn.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gfxongsrq.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvfhiwr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/ghmyrshrs.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/griaaqlut.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gtnthpwfg.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gxcoozdyb.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gtszjzukk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gfdabkeqg.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gthfruaoe.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gtbtjnfkl.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gtvwdlolx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ghtvtbpir.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/givdndhyr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/goqlrbbbs.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gnwhxorxq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ggmzajezr.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gjsvycgum.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gzryfzynu.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gcmtgocze.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gwwkgsugz.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gpigajyvh.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gtmqfaajb.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gricfrlvh.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gvrohlcwf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/girzoeqhm.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gqpismfdo.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gpkgfvlut.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gyxjhruea.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gjazmhkyn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxwixfyqw.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gsiozhajw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gokjsmlaw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ggpxvmfkr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gmjxdscny.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gdkwsybyy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gdqtmnreg.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gkmxpwmei.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/grrbchpas.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/giadepxja.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gwmyavxwe.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gmdfoiiya.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gxvzsnzlh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gduxzsjip.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gpnwdzctx.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gjsqnkjth.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gbfezilca.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gkbsevjdj.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gbqmxdluj.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gqafujera.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gbnuibeav.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gkpkpzars.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gyunhtszo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gqkmumlhe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gvusguqdq.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gkbmfwfwn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/ggknyndxw.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gdyriosvf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/glcgpuaoe.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/golclhlrm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/ggetbsxri.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gjshyftmg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gxnvdhwjm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gpetgzfzn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gvraklzgp.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/grxxmvyke.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gtgmbgswx.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gompurgmq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/glimodnpo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gvrhhierx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gyvuqmbmf.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gxosatdog.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gkxuvfhfv.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gohwxogpl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gnzojcvmr.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gvunsfkkr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gkoihmlzp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gflvzhadv.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gyaxsvidw.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gcdogyedu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gtqshcqlf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/grhzwvpfs.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfvknsyek.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gdphrbkhv.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gvcowtalg.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gpwbzokwl.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/ghwtymldy.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gvrwjvlwk.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gyymxkkry.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gbgxuijas.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gnwzfrnha.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/girckgbgy.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gulepbjia.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gadgntvsg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gozmrgrup.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gwirmfptk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/ghyjwtfhv.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gayvqvxgb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gfijnabdg.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gzrhqoeok.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/glcztxkgl.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gveyxuarp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gfvchhuwl.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/ggjfimoti.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzvepozcm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrwkdze.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/ganoaqacj.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gkhgypcfw.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gcteujkpc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gjzvpgcjv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/getncdflr.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gzlwxsnsw.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gfwrllztq.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gxbfbsbcu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/giihwnjnq.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/grhdqyqug.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gdleojspc.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gmtdmldjg.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/grtvwybqo.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/guvhjzkje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gdfvgynhr.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gqfsubjqs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gcgipokiy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gjcundzpd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gsubncojm.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gbktpwosq.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gssrkwgqw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gjraklden.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gauogdzmg.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gdzuyxrsg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gkdhxjltl.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gkgtzlsme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gnkonecyl.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gefnffeji.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gzxhvbwbb.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gbezsjeir.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gtzfcjygf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gumkvboks.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gcuojnlny.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gkldrasyx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gmtnomkem.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gambfedgi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gwrdpjggz.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/grgzvsxkd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gdnpzptky.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gxukismbp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gejwuuphy.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gxkwalesb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gcbreqhnn.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gmbdpzmiq.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gnragssxg.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gutlycfem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/glsmjjyts.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gqniuokgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gdapmgsdp.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/ggqvqkoye.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gebsisfib.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ganuskprc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/ghjpohbgk.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gvdmvzybe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gljgwjymr.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gyixgqkxc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gxyadzvua.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gsxsavqvf.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gimostyfg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmxpgizdq.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gotsxojkx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geuwwnpmr.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqtmkfkwh.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gyqljalel.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqmkbsyn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gvfrzacwe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwgkxlky.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gdconhxge.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gxlimasux.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/geffoswmu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gpmaclbsg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gabtfihvn.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/ghvobyqxz.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/geoecaeak.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gbnmplhfd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gonfryxuo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gracendqi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gewawhthk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gffnfjpjz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gbqhekorw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gbbznrqtz.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gfjtvpqzl.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gdmlsjlfn.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnfyjgovh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/geqxeedli.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gmxfgvaau.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gbnmwxoro.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gmgdytglq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gvlspdyci.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gzgxiompq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gcxypauwy.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gpbvuirgo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gponethyg.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gmdylpodw.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/ghfhiyidl.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/geznpcuaf.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/giozltgkd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gleatnhlt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gouulnezz.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gaxxgjbtc.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gbnqaeuqa.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gwqqipauz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdyawosbx.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gtzczqfsn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/grsjqpbef.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gjwctqjls.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gxkylpeij.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gmiubwreq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gfhguxeic.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/grjbtubny.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/ggyohqrqg.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gwfqinblu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqnhwovi.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/ghwotitpa.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gtiuaagzg.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gqdzuchws.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/giczdvdbn.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gtxhpobdc.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/guzqjzban.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gabpmapvv.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gzeztuyuj.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/grtfizvmh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gzaabxune.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gwopyxtpl.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/grqpepjgt.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/garweyltr.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gxnboszvm.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsfqybvuy.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gqmevkzpm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gncackbjz.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/grddudwnu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gavhrplyy.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gdqwbdecr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gcurrlhvc.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gfvnwwbcf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gxbexqpta.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/ggjosjsbk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gparuwgcx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzfmpmk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gvjoaizla.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gtspdtxqz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/guuasfuoo.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gcvbcksje.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/grrrtbhee.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gailnqtlq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gtpvnkahw.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ghzsmfkrv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gjsugizaf.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gqxqwwdpa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gsqcuxswk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gljdivjvf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/ggglrdqec.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/geloebbiw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/glsialwod.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gaywixboc.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gmrsxordl.sHtML


<!-- 参考信息 -->