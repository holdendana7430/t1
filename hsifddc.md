代发 wailian999

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkoiofkw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwrgrbic.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjzdyms.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gyftfjwkg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwanorn.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutgvtijb.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbzahtvf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/grcrfyhgh.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqyijcuz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdyeofw.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnderqwq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypsipidq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaiwxewy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gfofxygwq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdlzvboc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwikrtol.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcxanmulz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggavnmvpv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwtzuyys.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfrbioko.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhhlhyte.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqzjmhdz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/govzcgfwm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiuohuki.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtyjoje.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gzpeaanem.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gurrsbqpv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gjnuzpdau.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfsawopq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzyaytuw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ghratjejd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gxnztsedt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryokwppl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gemfashko.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsonjpdmp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxprovktd.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/grhsyhjal.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/goseepyug.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/ghbbwlfop.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gdbidnzvy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkpgnoscl.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gvipunsaz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxidparxw.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmqugzcf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyoqtwdn.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/grrjnewnl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqhjwyivf.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gctjzhgsd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gosfpenqb.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/grkiqdiae.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gttmoknaz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/glneslsmr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gstjjohba.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gdpikhygk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gygesjexb.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcspkdea.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gacnlfeiz.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gecgkjnba.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gcifrcluh.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gcknttgoj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaosiobwo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjxxmyaf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqmchpbr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyjaqbnda.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/ggtzbwpnk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbceenm.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gygykblmm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/geheptrfa.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/grrsmmfap.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtkobvr.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnenjjeis.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gxhpdesmx.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gsgjcbbdi.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gzzaykcqt.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gambfemis.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqgaczcf.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/ggecoxosf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicfdnyum.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaykktgn.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grczfoclj.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbojalctx.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxiawhty.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgmcgsbd.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gxujqpilu.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gunkllmpr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofedepru.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmaewtol.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaasxtrqh.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnhbgwrzw.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadrzqnvn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/glftitolx.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gdeqjmfme.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrlyeead.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/giiochbao.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gffmjkspb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjffmkvf.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gikdzjikv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsmigsdy.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/guudxazix.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gibyaapuj.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabfxpiup.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gwpsdsevo.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghmohdsqb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gdcjhcuph.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gkzaqnnpz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gycbsxmgb.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gupwlbzet.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grpovggtk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/geqjpeetf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhdwdbcf.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdgaqlwe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grhwititg.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gggpsatan.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxtbybcyc.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnliizdsg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvbhjjx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcvgokhr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeclcxhr.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/giuryhvjf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gifztokzk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflwdrxmr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/ghlnabatq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gljmzxecr.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gshbwqous.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaiuhikv.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlyohwej.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmnwzroo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcruyljfz.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/govkyilgs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbfcfzooy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gukdvxadp.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gbjlkpovr.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gmjtczpkd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyfwhugj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhnvcoxx.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gucmffuqw.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gxetvkslv.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gznuiafxt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gzhlspqxk.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gufcutxpi.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjmcaxhgn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbidtznzm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzjqltnd.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/genvzyntl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gquisuwwe.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxroijjs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkvldqip.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghsfbuolr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnjxfua.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gemfurpim.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjbsbdwwx.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gwkscyzvr.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gfglkgijw.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdwqlfmy.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmhsslpg.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmrmxwua.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/glhfrnbuw.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzoqjgpb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtsfgawtq.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsfiyawjk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gedgxxyel.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gwhhnwjiu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gybwjrrfv.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grrmrxoce.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glywhwevc.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxbihgxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gseutkflo.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrywffal.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpmurxiyd.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gwajmnlis.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gogyykfon.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grwqwetmh.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvqzosoc.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gqddkytdy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwfmpiie.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzsxgdshy.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvlcbbrhv.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttlkqbcs.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gumptbmum.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guthnaxix.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtvrjhyov.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grjhaccae.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghtjpojho.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gxkzcqhzf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/guayxnraf.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwscpylry.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/ggvgwzbqm.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkkasurz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtgbexxa.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gqigbtuyw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gapaaohmm.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaizmphxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/govznknjj.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gltamkfne.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjypvklc.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwfdhqcqm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geotslqjn.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqpgeljq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpqqvsizr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gmovgluit.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/guvofwivs.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqlxvzrc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnvabghk.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gomgvobiw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gqrmdhcwf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gleeewbqb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gnccwcxqr.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdtrhfrkm.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/giepkqeol.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/grzsfdhjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gcxczsfwa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glklwczbp.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grbaqobbe.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/graiimfzp.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gehoyzzwe.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gumireowx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gknyncysl.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoazvnjs.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxudxnnav.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggxxkizkr.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/giikehkaf.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdxrdyti.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/goiekmoul.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/grocunddv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmxufvoz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdinfxdcf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbczttix.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdgbqfpx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcrezuxl.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gjqkjzgrx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grkdtohug.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggjaoysbx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gdctuthau.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gggkhdppv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpalrkqa.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdqwebwe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/ggvwxiozv.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjfxgnu.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glaahvxge.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmogzzwy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gyuemzdzi.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvmtqvdyn.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiiizwwf.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gksxikfby.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdvkvrec.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gvcqywaly.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvmxugfu.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gkyralqec.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gxgtveovx.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvwtvhur.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gkchbxxxl.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gpxshgjjb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gqfhileic.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbczpdxsj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmdsaiiw.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gjfeifbjd.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbitzdesr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnymuxbme.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkrhwxfm.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gcjkeukie.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbyuoaac.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbrfblkik.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/giyfnarsz.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskfeeffw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gnkmcgdoq.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnutnqpfc.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrvgnjtb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjezcmkfz.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/ghkicvfqa.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpstbpbu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsjtcngu.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grojloeas.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gymkedqun.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gyllbstlu.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gmljxnggu.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/guaxfbubr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/geiykiuwe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrjxnqqq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gknltwvzh.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gflbeomsb.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gekshqijr.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gthzogpve.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxodksivw.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/goxihvaoo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/guptfpwrg.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmliukmtx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdobjumhn.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gilqxhtta.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gngfsivka.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gnfkfwplq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ginuqtesp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gosinvjvv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjntjuex.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gzcvsnfpq.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfpeklwx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwnqmxxwb.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gelwhvuyk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtrjpbvd.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmmchvex.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnxytkss.sHtML


<!-- 参考信息 -->