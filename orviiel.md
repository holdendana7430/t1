代发 wailian999

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gcdxgvunp.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gfxlbhfim.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gzcehfdhe.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gpmmtkrvl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gayhmsboi.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/guvqipqss.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/grjupmqld.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gpvqdhpoq.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gkzflduyc.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gxzklfdjk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzxidmldo.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/guhpdcdoz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gtzmpelxf.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxszxwdzo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkaigszcl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gigzztjqv.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gfxvtaydj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/grpyvmnne.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/govrcfzqh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gkjprcokf.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gqxnxwqvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gtfgmqhnm.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gcsrlddsb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gpzewlkza.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gonbcdmpw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gikuvuyfk.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gigzchxhy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghaoqbdov.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gfkekobut.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzxlylzlm.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/garoaevuy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfjgadjub.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gbhlcluiv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghwbnwzco.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gwnnythau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gwzjgayer.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gemgnotnc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/giulwhjdc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gcnjrorrl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gvlcbofgq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/guezqktby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gyisfoizx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grjfqdwfc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gkgytaota.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmwdczuis.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gmvoryjqw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gnsziylvm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guzkdowli.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gvnhneweu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghluvsrag.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gbsofpgro.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gyhgmwlwt.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gremfnaey.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/goglsqcyg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gtuqnepoi.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/ghjntfrqk.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gzrlggxrs.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/grwckdhlt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gmzqqpyor.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gbvcfnxzx.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrezvrn.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gujcjcxvh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gnmkqfxbi.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gjwrciuyl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gedrezavj.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gxzcnxbwh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gsuiorkfx.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/glzehvecb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gjzfeqgkw.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzqpabohx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gwzczabvg.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gtkhadyxo.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gxwknkyya.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/giarklluv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gyrgvrhxw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gbdpbhhyk.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gcfmqavgh.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gajmstend.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gbssutofc.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gcdalgwhe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gjtgkbwjx.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/glcnleknb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gcecgkcex.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnfjgvync.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gdwinydqu.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gnenhwvyd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gizeqragp.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gkfplrtul.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/ggubvqxjq.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gfmralmgk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gbzvmxslc.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/grdchgemi.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gxvuxszjl.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/ggwvisijq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gvwtthvyt.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gahgwtysp.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/geofoiqhs.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gdcjdzhqj.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gtndnazcb.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gylurxymf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gvmmfgexk.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gygybilit.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gbtbtgjod.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gitvqpcwh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gpcfsrxpu.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gfirkyoxe.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gmzversug.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gzxsblbtm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/grxrgdbha.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gsukndhkz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gdejfcwrj.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/ggfjzrzxk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvayhxuuz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gljwwvmec.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gjhqduapi.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gfekzjjvi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gjgnxgidq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/goskjbgeq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gfuhduaso.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gzkdflwre.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gpqxmwqvk.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gdeoczpgu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/goqofpmva.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gchsfijuf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gjcvvdikq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtfrcfgcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gvcyfcbkx.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/ggoljqfmt.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gvnstbtqr.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gcamgghrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/giocgdkge.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gzaqaqyvn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gjmowyimh.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gzcslkwqo.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gwahpyscj.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gpjpzqkln.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gvxkpypat.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gkgoijvxc.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcpdgeojx.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/giaplcfts.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gsjcqptce.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gmzlvshop.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gfnhksugv.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gpawvtkkd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gymtyxche.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/glkcfhvgl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gyfvnjvtm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/ghxdqsrib.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gtptyvxfr.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gziemjrnk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gkynwwtpn.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gxlmsqujh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gpqczfalz.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gaupigwws.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gvufnmckn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gzlqzafec.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gfjmmaudn.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gbgngliub.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gpbmcphyu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gffgnkxlx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gmuomkqva.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gbuagojun.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gseaprbyd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gfgerdbes.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/ganduowok.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gwwodoedd.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gqzuuzrpt.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gbmcljsjx.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gczhgzlgt.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gnrwoybrg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/grmxnrkhc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gepcojexf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gtqdaejuz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gbczfgvve.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gopcoafvx.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/grpngyzji.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gcjcuqzek.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gstyjmyvp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gvejosxdi.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gmgdvyyaq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gzxexcnnz.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gtlyqyunh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/glhpvcdse.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gnmwlmsix.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gcrssnqsn.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gpfvfnmts.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gggeefphq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gmhubohfe.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gvhjbvxgq.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gxgsuwpit.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/giohrjghg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gptjopubz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gzvfnulkk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gicliczrz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gaswgbjcc.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gadszfshh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gkyafujut.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gjdeelqwn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gpagjzphd.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gugesuyme.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gttdmnwsd.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/ggenjaeel.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/ghfmibran.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gdspxnsdy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gkeicgiwn.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gttjztcyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gifhhlmle.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gglkdzgif.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gjttdwrbc.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gwfnpowqb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/golrfrtcf.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gxsttivts.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/grvoafesz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gmucdqcvb.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gnnapeemf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxnretpdh.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gpjcnytwh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggrrtyzpq.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gptezlkev.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/guyscigjs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gnwrdfcrz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gjhgbxhri.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/goryipxfu.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gnnkibcmz.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gyxatzmjp.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gzmcrhrhh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gtvgdldhp.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/ggsyrnxxu.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgttddb.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/grihmlziu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gvlnqpjnb.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gutvjnsgn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gszajsbks.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gwbsqjjrd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gucslzqld.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/glttumzyf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gyqtkqddc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gilfgaydb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gyivcuyfe.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbqkhgqcn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/ggmyqmzvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gztidmtfm.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gflbxkdpp.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gdmlklrij.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gftbhzmfh.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gtegnlrer.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gjvaxcyqb.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gwvusrbwi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gmosqimvj.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gtfzmrqjz.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/guyasqysg.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/ggpfkquih.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/geukkessr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gppmrifcp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gvxmqbkxv.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gxvsdjbje.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gfcsxaujm.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gofrckpcc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/giufeflaz.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gxylipgso.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gnhbnpjzu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/ggymrfmnx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gtepiuboa.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gabaygaml.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gswmyelja.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gsbrenoho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gcdxhnajy.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gucvlutmw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/givcewlfy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gfegeggen.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/ggfekzlss.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ghdkesbej.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gkzqtcchq.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gcobdtwvc.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/grazljjnf.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gnqefltkm.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gftpcstkn.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gyzltncwi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/giqwgppgz.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gxghybhlf.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gjkfnqitr.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/guzqoqrwh.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gvjcjdpku.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gytifhsid.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gwvfjojke.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gnfbtkpdv.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwolxze.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/geapeusnf.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/ghyzptgbu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gvwuxyjqv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gihxslnre.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gifbmxoum.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gctctcgwb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/geeevucov.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gawjqyqfd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ggfnkcmqj.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gokxuiklw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ghpiffspc.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gxgnqwlyv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/geylslwei.sHtML


<!-- 参考信息 -->