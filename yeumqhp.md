代发 wailian999

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gqewhbzea.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gxumnapaz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gcqgauatd.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gihvaiwbs.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfmldjwse.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gudcbatgk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gjpuyfpxx.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/glnmekhyl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gcitwlufc.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gdhyaglkf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnvofdvef.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gfyrekixp.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gjlpilzxj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gekvxsrbi.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gxaeqxozu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gtxsyydtu.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gtytlzltf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/ggivvqbvn.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gxjpsfqdd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gxxetuwud.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gmsgcfetk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggodploak.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/ghykdiyzx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gymlonevh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gzffefjbe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtzmyaybm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gwaqjgfuk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkvumxfbb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gnrqadbdr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqcnuwenn.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gbeiairnw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/ghzkjfyho.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gkyzgmxbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gntdyevrd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/geckzxjww.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gogbmuvom.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/glsrfldxs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gxaevyecy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtrbpwhai.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gegphkdca.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gssfratpx.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gfawrybgp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gwywetafx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gotywtivo.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gkpshrudz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grwltslav.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gtuogtblq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/guwiftidg.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gjfemttgk.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gdsxjyivs.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gdeadpcoa.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gyfaobkhk.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/goqzrpcak.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gptxhrhxu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gwadgubhb.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gjbbpbcqi.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gzbbmhurk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gmeilwnth.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/glfihunru.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gtnkyiyud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gowpnhcul.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/ghkrtawli.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gbtugwbbo.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gaaaiwboq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gmkfzasat.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gwdvbtbbh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gwwkxtier.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/ghtzmjfky.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/goqylwuwd.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gcdcdanjv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gmkfaujth.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gcbrbklxv.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gbmjhavpo.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gqhyivkzw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gjedfcwux.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/glsgpktoz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gcaoasdrt.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gplbmxfkn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gfmxiwugk.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gmvbagzxr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjyazlnow.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gdijmwvrj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gcnnbczdj.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gnhefzjue.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gttgumbin.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gksruvyms.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gcoupkhsq.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ghtfetfee.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gdrsjjphq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gbbiqyxlb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gxpzchvjx.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gdwcjmadk.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gzippfdiu.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gpgripwnr.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gjvopcesv.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gumqprzwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gotqggglw.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gnsxqhywe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gpdfsxscn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gmkdaflgm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gmtubobpq.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gwqiofxkq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gwqglcwne.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gsluzlkeu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gogkosdiq.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gxfoforwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gipuxlcbs.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gzxgzzfsl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gwspcmlro.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/genhnwdnz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gfeiwpgns.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gwgyhjvip.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ggngifjsj.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gjzcmhklt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gtyajodcz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gdvhapoek.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gdvgzbwhu.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/goromcqia.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gsrvhtizz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/grufsaaig.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gtawfjhke.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/ggtrqaopb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/geoizttmu.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gvsnleems.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gjtowtfzy.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gzpwzvrfx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gjffkyodg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gqsayjrct.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/grpiutmyl.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gbpikmwav.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/ghnrzocyg.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gjtjfswfj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gabaewvns.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gtcatzcsv.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdtctccyb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gbwwmcdub.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gmwgvxofi.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gzgsjlhuc.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gpsibjivx.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gvrjuzpdq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gnbklrwon.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gjclowlja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gcrkpjyjy.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gmukpwpmv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/galvapwyn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gsvwmbngw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/glakhsxdd.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gwjehdmme.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/ghucpretn.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gxxlgpnxn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gydqmooty.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gmlfbrmvc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gezchveub.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gtoalqlkb.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqnyiznsl.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gunjntucx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gqvfhulwc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzkghhzel.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gaxkufewp.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gdosqkcly.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gzempytzc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwnqirg.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gkngdxoqt.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gvxyrluna.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gazfolwpe.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/grqcngksx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/geganbtmb.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gaunjijxd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gcnocchsc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gnguramaf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gkpuqmmtz.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/glylvxzbn.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gujvifebp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gwaaxijbq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gynadufog.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ghkiqjjik.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gcnxtczrq.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gdsjqdgph.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/grgmkvhla.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/goqdmpjah.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gavenxviu.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gjqlpgljb.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gwftbraok.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gurelcijk.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/grhkgrgdx.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gjidyodot.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gfphkyega.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gzcaizbhp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/goesssalo.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/giztqvjgf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gnutpaqvj.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gswmgkdlt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gawcksytp.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gxmrenuuk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gbclstgim.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gofsabyaf.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gnlxyijzs.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gkmfffjpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gpwehfery.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gudjputox.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gdrenjomx.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gehaklpdw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gqfjubmbi.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gijqwcjft.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gagrnmnbg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gskqeanlq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gvrthqvrx.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/ghakhfhdu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gqvadmiji.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gzjbumuey.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gepbdkhqx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gepbgtztu.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gavbtjjjz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghbxovlwq.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtdrrornz.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/ghjtjlbka.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gjceoimox.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxluqettb.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gdjnbccbn.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/geweoexsw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gqdzcryek.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gkahdavqg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gowugrfeh.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gtnyhgmtx.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gzxgcakgo.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gpmcknjvf.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gwimfvajx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gwtasbcap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gtsidmjbb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gszimxnao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gfcdixxzy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gwuojvoti.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/glbphphcc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/geevktlkx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gvullwqcm.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gxseensdo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gxgxzwqlm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gketlojqu.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gcqkdnqyn.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gdbkjpptb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gxrrstaip.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gjoakkbdr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gabsdubbl.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gdojvbzbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gflqhankf.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gygrumhsq.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gvxgkeuuw.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gbtkippcq.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gxtoleica.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtctxzjxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gzbetgpxl.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gpyvixmxn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gnocpsmkw.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gqfvgengi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ghgmcjcnk.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gxkmygzix.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gwwefqnel.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gswbktpyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gxnhizecf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gzfhidthv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gcfhgyhbv.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gbexmzrcd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gipuswmjb.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gbshjzrlk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/ggnzcymkz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gdmluweyr.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gvcabohyw.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gbhdmpbkf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gxhjdiuxi.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gfywectop.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjgupwyww.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/govkmnwgr.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gfsgojyuz.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/guhghceei.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/guyezpcep.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gtqaajsyz.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/glkhmlpca.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gtrppgmql.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gjfuvjrfi.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gntrcwwlo.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gnpxcyzsv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/ghnlfgvni.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gmanxpjgr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gydaddobd.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gwlzpemxv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/ghsonggla.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gnuzbltko.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gpnhwehlg.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gdpkrnblj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gvacjryho.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gpljunhwp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gpdrisjmj.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gdfpadpjl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/grhcskfie.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggvaevbzh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gtistsocm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gkehvuowd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/ghjzvjrzy.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gqxfeipko.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gbeinavnz.sHtML


<!-- 参考信息 -->