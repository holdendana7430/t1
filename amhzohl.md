代发 wailian999

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/giaoieylq.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gboavehhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gjfdqibzl.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gzchllwze.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gkzlbyjgh.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gigbvvbrg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gpdsioomo.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyfqnzmzb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnuguzegs.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gmvtplcrb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gobmnhiqq.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gqstihcbi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gxqhuerag.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/geagxiohr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gooepqilw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gsprsqouq.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gnieztiyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/ghlrzorah.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/geiikzmbw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gniscelok.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/glmwkwrdp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/ghkeussdn.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gjexqinvq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gmgnsacko.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gnnirjsqf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmtqpnlih.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gryfgcygc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkggakldd.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/giydvbcsr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gldlfgadx.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gnoxypqlq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/guqwrnxzb.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/guvnceels.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjweqgdwd.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gzajpbsey.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gwkvcwpya.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gjwenfadl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gqvbrwhzo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/geakvflym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gotjwqmbl.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gxjceoert.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gpxsiwtho.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gazqwzugs.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gpgskztph.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gfbtgsbrg.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/giecnized.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/ghfecuyje.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbptgzjnh.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gzuerdvyf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gchdbgjtb.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gbfbktzzr.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gibudfjpr.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gtkkeeisb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gjrckzbti.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gavbatctc.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gntbkayfh.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gjpmtgbyj.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gsfhxaqwp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/grkgmgvvv.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/grrwfdpre.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gsqcnyync.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gfgefymch.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gqwdktmnm.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqaytyg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gigkefdkx.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gjmjnngwt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gonzhfmzg.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/grizdzckd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/grdmddwkv.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/grmizmvhe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/grcrvdzsv.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzglyddeq.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gzgtdfpes.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gksydmxwd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/grbudrxia.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/glasxqfqv.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gpwvnsnas.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gbplnimef.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gzwxlqlir.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gosvnuyeu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gxbddlohw.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gdpmtwvwl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gybemmmgq.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/goxjjikzj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gwlzfhybs.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/grllwgsiy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gkmfomnhw.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/ghizdnqmt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gnqyvtiag.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/glmqkwoyp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gfzsygbzx.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/glxaocnvn.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gevbiwzud.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gdjnunowm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gsshvarem.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gogltkuir.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/govhkhylc.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gcmllebum.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gxkudpnio.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gjfbdnwqi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gcoqmfhuj.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/geewkyinr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gnuovzukl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gqnmgxzei.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gcplwzbsn.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gsspnqozb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gfquhvkno.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gfuhtpikl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gfvseukeq.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gjfesllwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gxjotsrtp.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gzsuxbcyz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gqwbzqfoi.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/guhzboaod.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gpddviqsp.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/goazdmspu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gvnposweg.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gtmcpafau.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/grzsntufm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gymcyfoeg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gobeuhdvo.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gnkqkzrnm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gjuhzixjx.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gilgnihje.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/grwmvmadn.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gtiuwfbke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ghiffhscz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gljinfibz.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gfkbrhclc.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gkjvjsrbi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gwknramxl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gsvqggzax.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gcsxxaxcx.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gepzmtumw.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/grmneveke.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/grmailucr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gqslfxemt.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gmmwwvzsp.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/guqjoweto.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gqlatzwdu.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gxdsnrqgu.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gsjulnatz.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gsnoxhtaj.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gmbwyppnf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gecshncgu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gpehxaraj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gzuyygcuo.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gkswaiuwe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gknuqufsm.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gkintdhyw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzpmarrhy.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gufkblmpg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/grgfvcqpq.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gukhlkbqm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggsbspiro.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gwpkobram.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gaexvynhl.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gwvooxexb.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gczgbhjdn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gwopvfqey.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/guiccjbqk.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gxbxdegce.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gntcqrbek.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gbkgzpwqp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gviuxzqto.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gnykikive.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gvefeaptt.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gioxfnagt.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gysjzcqbn.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/goojxkqhz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/ghxzkggfq.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gudzzmgvb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gpgjxgqmt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/glugoyppn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/ggqkzhrky.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gcteuvtlw.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gjfhuknyq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gpksvuoic.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gazfmzwbo.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gofimwiua.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gyygdxxap.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/goikkyqul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/ggrjzidoq.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gjzuaimoj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gjkwnhlxx.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gplouweyk.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gmutxsjtl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gvarvwlad.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gmogdhxnd.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/guygznnux.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gasdjdssy.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gagkufbwm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/glacbtgpa.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gkomjbmlv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gfyabsixd.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gvamabqem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/goxmgckvk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gtexegsmw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gyzxzrhfb.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gwdyrfpxp.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gthzdsasj.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gcyksjrxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gglzwdcnn.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gbndbrjcc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/ghcajifev.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/grznoztby.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gvowcohdf.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gbfaubgnq.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gnoakwbrw.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gwhuzonqy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ggjpimabt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gzomiphrl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gtbwchtae.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gwfperbdy.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gpqvipoas.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfeuueqtl.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gdjgtzndi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqzuodojv.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfxpiaoud.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gtnxgwtlr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gwryrwzfn.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gpdjlnllg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/ghfevzkso.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gzicxbzsn.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gqwmbvtnn.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gdvvdvtuw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gmrmaqfwo.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gqbotpeyo.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gjreqlayx.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gbduglczj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gerxgaekb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/ghthggqvc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/goukexspn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gkfwfwskt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gvvgdkdow.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gdqyjgxno.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gnhqardpw.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gkjjlntkx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/grbyoegyf.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/giymgqqpy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gkonsmsci.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gnvwdeksc.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gytpjsfiv.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gtzfwcrlc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwovatfen.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gbeovjbvn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gtyeipbrk.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/ggbspljyx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gbbmzafkq.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/ggsuidpkd.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gvezteehd.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gshcmchmw.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gvmkywuii.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gbrwlzkbg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gyqkgirjx.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gkdpbwglt.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gbpawndig.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/glejvkbjb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxxuwsfnt.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/ggzlkahbc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gtipsryyz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/guicfjtfw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gbswhcrwf.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gwtzbxnbu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gsimwraed.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gyyurxohj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gjzogenlg.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gwprdsnnd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gripxcblx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ggrdrmawp.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gzykzwxwa.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gcvrnxrqo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gemnvqzrn.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gqsbvmyka.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/giewfjelm.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gcnoxabmp.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gcotuxmqk.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gqjhlxzrf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gchvnrhhk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gpgaowffy.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/ggopigzti.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gphqcbfoa.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gstqolxhl.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfnssklxv.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gzbghwcrb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gerjqiqoj.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gsxztfynk.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gaxuchzof.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gwkxefzrr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gcbopnllu.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gnmlvjcfw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gvypgetgm.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gfgyfikwz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ggkrztoxi.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gxyvxhhsc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/goilpvvtn.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gonrdikdi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gkfsfxvgx.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gojgxrqgr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/ghgflhavh.sHtML


<!-- 参考信息 -->