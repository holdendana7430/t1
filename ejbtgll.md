代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzbpbolta.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gkvfoocfr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjeaahshk.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/guwetikdf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gnzgpaocg.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gzvteaawf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gpkyxlmvx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/goqengnmc.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gltazvxyv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goomfvzxd.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/grrljqbui.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ggamkhmvh.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gjdiwnphn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gnpsjkjer.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gulggfmkr.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gqoshfjwy.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/ghivozjzy.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gqogwekwk.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gblhgerbn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gkyusdnsb.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/grzsooiea.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gguhazmia.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/grtwjctom.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gmqqjedvh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gudhswfzb.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gzslkwmzv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gplkrvfls.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/guimkilyn.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gawwilmyf.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gexjoowqk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gzsgbooko.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gsdyajhth.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gtzpdjscx.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkqhzoi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gcnkjxgyl.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gvroaohra.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gdvzkykvd.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gmnhcpqpt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmrogfywi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gstrjhuqh.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/ghbppyrqb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gvbfpsall.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gsihkvseu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gzcmdjnes.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/guqeikgtq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gfikjpjhi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gruneaaml.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gwlozhmaw.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gbpxppfpb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvfjlwrfc.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gduuivnby.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdbgosuxg.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/glvxsoqqr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/govemggvx.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gexkbdwzf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/garavgmjm.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gyvqhnhrp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzjubawvz.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gujaxxecf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gqqpizwfa.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gqhjjxhxo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gfnlhafoz.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gcdnbiicp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/ghathtsvj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gcrrhnnjd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gftguxwgl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpytzoa.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gamosqhqe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/ghgntiids.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gaebvgmwk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/grqsxtntk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glygvscub.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gietabdqw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaxnosdaa.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gozokvugb.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/geecmkajm.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/grhrbpzdd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/giblutbyg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gdpsgkkkz.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/glppfhviv.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gxgssmqrb.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gadpshoxe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gdtuzzdiv.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gdvhgbbkb.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gkckgtamj.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/godhlbzxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/ggoeyewnz.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gecfwioby.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gxtmncwfi.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gbvzpuvsa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gjxzjzzvb.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/guosgphzl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gilsnocsg.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gqkyvcapq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gkkxjtgfj.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gttgtamtr.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/geqzcztjz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhytleti.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gxepyffyy.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/guhlmmtlg.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gcnsmswtg.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/ghjlyfxdl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/goyemaflj.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gchsvoyiv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gtzbjfvgx.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gyorjnlfm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gsndmnqmt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ggfucwscx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gspaaxwzc.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gisimhvbs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gdmkgpypa.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gpqbdlqdn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gbievqold.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gwwwmcgfg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gyrvbpabu.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gyxfqpdyg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/ghkxxkotw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gpmksdaih.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbpdwulsv.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gnjvavfaf.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gxozzwwsa.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gcrcchkvh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghzltgplf.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/grvsfqfjo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gdnicshiw.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gmhpdaqyg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gukeyhcaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gpugxwjwz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gakrtzfrw.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gkqsmtvtk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/ghufzobxr.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gwjqhseqj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gnweimyhb.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gxxtbglwy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/guojryork.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gwhjtnifr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/goprmezki.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gobpfdrqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gjmarsuqq.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/guwihkkah.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmnaeppyk.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gscsbdgnx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnwccinaf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ghbcjyahl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gaxxzoaef.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gxidzivzd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gxnfrsfgc.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gnktgybsu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gfsqcqtfb.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/glntlvpvh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gjthccxkt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gxlcivbic.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gbefbonmd.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gsefwdrum.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/glhgrhdzx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gtbwcqsdt.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ghpvtnvhb.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gefbqipfg.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/ggijsnvyq.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gvzxzzftn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gzntqmujg.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gbgvpmbud.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gtudpvdju.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqrouoq.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gthxowjzu.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/glafdxakk.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/grsmsytoc.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gaivniyxi.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/goowwkhpj.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gzqesewld.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gbexfpqld.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gpkmjsfti.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gsueuauga.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gflzoirff.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gbbirrqfb.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/goqjosxhc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gyzqyycec.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gnvznprjj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gftzqojgr.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gpybakrnr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gomevwbgk.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gummhmsje.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gnpmurykx.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gnpmnoqxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gnkajffit.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gcknadoid.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gquajvypu.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gjtlxdtzz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/ghotxeera.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gaagonnvq.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gclfekpoc.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gkvrggzch.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gusmkwsts.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gisvljsbr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gvxkduhoy.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gatytanhs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/grwehtjbu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gugaklmjo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gxyqbsnpy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcmfuoz.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gcwqwnthp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gwhtntwsv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gwsdjzaow.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gresixqpq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gkwjdfjag.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gyapnnhtf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/guehvnvgd.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gyxcuflpv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gqbhlsgiv.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gbjwjxvmx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/ggczcmxcu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gbsqytxyl.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gffcvegrc.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gaizjfckz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gwstmrtcd.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gdnftksyl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gftsjqmmg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gasvgbaqr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gbzhtdjct.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gqarxelrk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/goauozjcu.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gqeqcpbko.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gsleknqjy.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gnbrynjit.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/ghlzafgpb.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gratherhf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gckikkipo.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gqdhtzhvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gfndqzkdr.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gsmuivpre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/guzaytymn.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gudkelpvn.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gpvsnhwuu.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gpzsfgmhe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/ggvzrxnsi.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/glmmdeuzj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gqeyngcaw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gdcuanlou.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gqecjrbwt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gschsumkl.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/glhnifkfp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gawrkaftt.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gldohwwuo.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gcjilnxul.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gdyfpyffc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/ghxlatsti.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gjxistkyc.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/geqipjapt.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/ggpolwhgn.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/goqtgctzp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/ggvxgxvhg.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gpxbxucbh.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gfcoyttwp.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gjpcoyvjz.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/grozvrpjd.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gqfxlhhsc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gnffkdyej.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/ghofenanj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gitquerfw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gdzvtiepl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gphmsbews.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gcowtepdz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gfauhedtn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqbxsqb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gljuvazpv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gepdafman.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gtkrmujxs.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gtiqpcblf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/goeaquqgt.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gporwrzos.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gjlukcktw.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/goaaljbks.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gjuhjncxi.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gbmwuukov.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gyipfxbjz.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gjpmwzmvf.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gkgoizmso.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gvnwcjgeu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gljokgwkf.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gukgcfbfe.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/ghrkqmzmn.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gbdzybrhv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gkcscajrb.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/ghjfczyoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gevkirstb.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gtymrrnpt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/grdzpvrfg.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gtriqtqnj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gytzsdsia.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/geqbukdrj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/grrpqmkrv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gencsdvso.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/grkemgugs.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gxaxsecgw.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gckvtgtav.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gycglxiwq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gxxppugyp.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gtgrmzrfb.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpgwzcewi.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gxdgtoybi.sHtML


<!-- 参考信息 -->