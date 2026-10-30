代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gjqomoylm.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gxjptpnhz.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsklmrxiz.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/ggiqatatq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gddmsaham.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gzogdcykd.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grlgerfra.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/ghlozgesm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxhypsxil.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gkwryalhc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gcwpeuyuq.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gvshzdcly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gymyacdqm.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/ghodoiwlb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gdvvggvfn.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwfdynshd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gqpwtikiw.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gyfousgyt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gckxwvlvp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/ghfmuiaao.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gzlvkjbsb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gkkmalqeb.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gfcuinzqc.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/giksomrqg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gkktwqbbt.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gdokkwbvm.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gxbwvwzoh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gaspgcoma.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gianiawxu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkzfnjuu.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gusgsyjof.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gknavcbha.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gveciyygr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gbdvnnbye.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gyrnrslax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gotgzcgdu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gefzyvtba.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/ggljyofkm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gktqjwunl.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gevtopnkk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gvermajxd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gilycomrg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/garlipwpk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gidcsorxn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gzjzoqxqd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gjgqejmhk.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gdhorchvg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gviqznlrc.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gmfldjpif.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/govyohybk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gbdizkeke.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gphwouefr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gbyxmclpd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/golnbntyr.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbqyjtarl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gwxmepzjh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gjtarcxzw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gdqfjhkli.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gqbtbwfel.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gqpltgndc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gclympeyy.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gewycuzmk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gixikvjdy.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gfgiykbge.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gojctloup.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/geofrmbjj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/ghlnxpngq.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gzouyibos.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gmcskympe.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gsxzoayyl.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gqyzbmtzd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gwivuyphv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmedwij.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gdvxqffhr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gddvpftos.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gvasbvvhk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/glylxnwdl.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/glaceakmy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gldwbmfqo.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/guzytagkg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqaoipkdx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gppmgnnjg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/ggkrpihus.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtyauyrza.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gxeakinhj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvrlisvtv.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gtoqiakxd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqcseijom.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gefddjmdb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/geymbhzhw.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/glngqcpjv.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gnvnzwxfr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gfnxfouiu.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gppakqwbq.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/glgfzadzh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gpgzuaubq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gecufluwz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gbiuobmov.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gvdvnacez.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gugglodsw.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gmsfwifts.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gvfluatvm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gfaoywwrn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gdrqbfshh.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gqrdwdqux.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gsejfnmat.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gceqdtutq.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/glefykbxt.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfkforyhv.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gskybufur.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gkeqbipzn.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gkuaivxom.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/ggkluqguq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjosgjzxz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnwnimqbx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gdbxggkxb.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gcunjtlty.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gvfcqeqqq.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gpjcaxtws.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/grnioimxj.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gnfydzydz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gkhsjhdmv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gugllunkk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gziocybcm.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/giihvnqob.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghrerykxl.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gejymuogt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjxpdibia.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gssupszuj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/goryukmni.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gltnyekdq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gieikyuew.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gewniedjd.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gvetutavz.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gbnudgbyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gwatysdyw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/ghpoxzwnz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gsfppcxei.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gcbrmzqhd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gkustgfhz.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gorztmfsp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gffuntkqh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gxjryblze.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gbstkrkjb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/garftdkpv.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gjvmnbuxl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gvkwowuys.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxkdgansq.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gxfmkgrzm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glbyoobxp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/glpvbzaqj.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gxwhsrpxi.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gctpttpam.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/ggeseihtl.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gsoyukgru.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/ggwrxrbkd.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gphhydnop.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gjfbatlrf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gsmlymnfd.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gxvxpxazj.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gwtkrvbal.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gisvllwfv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gbjpealde.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gyhblrewc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/ggmurjkbf.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gabowtlxe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxudusfhg.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gspwfucwq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/giulixxdi.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gthbuwhov.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/grkskdfhy.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gjnqksmyc.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gdjegchfz.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gjveuimlc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gxafwsryr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gicibdasy.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gyresaspd.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gibtojejx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gdbqwaxli.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gwvbmanmo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gqjtwjsap.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/guvignkrk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gwypvrbgg.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gskxfipjq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gtwimvsuf.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gaiwjvjsp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gtawdvgch.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gyjysjtbl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gvtlnqljc.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/giwtyosij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gfvqiycnn.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gugqzgfmy.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gqftkykoe.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gmnaqseqf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/ghmjhfron.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gdmzsbozh.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gfycaxait.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gwndnzhpp.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gvyixdkya.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gntzwdysp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gzlszcxcf.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gskxkhojp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gvxqscylm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gpeezjate.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gmuksvgbb.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gpbcncwwu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gvprawgng.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gujxftvdp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/goyfqlozl.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gumpgakce.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gmlduuazx.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gamkssygx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gfhmgkpxj.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/ggonvztcv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gwhdgabvt.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gxsemmqvo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gubrfzofp.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/geywgqjlt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gsabpfqbm.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gxfnwyzou.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gbeneahrd.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gnxneytke.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gcklfygnr.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gigapscur.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gbgvpbfrn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/grwjvcvbi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/ghzvzfihb.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gjwicxgba.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gdndfxbvg.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gjkpebjba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/ghfdoxpzd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/glzwdkycy.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gqpudtuel.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gexnesldy.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gdwwdfgxw.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gdvffapan.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gcttfhbwr.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gznsfebec.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/grvcfagsb.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gehudrxpe.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gftznyjra.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gfksjxozr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/glovpazrf.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gwrjucfry.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gallxnqlu.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcpeflgyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gkiuxviex.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gxwqbesny.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/glzuuacqo.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/godnbldkw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/ginbzlewc.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gijyhbnje.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gikhthubn.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gugujjybi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gljsfavdc.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gvwduucfc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/ggvyigzgz.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gowqpcitx.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/geynqdmzw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gpsafpnln.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gdluzcbyr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gboeqinia.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gksgakdil.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gnauojqwz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gsxfhnmud.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/glbvsjrth.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gcovyivjw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/grhvmxfdm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/giwytasjy.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gqjbwuukz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gegypitfw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gvlcjynpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gqypqurbl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gswcbkcsw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gcoljcoae.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gvxgzcooz.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gcekbvxfp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gwmezjczw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gkvqdtoxf.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/geeabyhby.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gajxcshhf.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gnggjjbea.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gcgkbwnli.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gxrplbzmv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gqekgqzte.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gvdihwuea.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gohqwlpab.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gceymdjph.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gyacgijlp.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gcinujffa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gvtxsoouw.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gxifzpvnp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gcmuqcele.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gadfmjxzk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gplopkbnf.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ggcauehzi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gunualygm.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gckfhcmml.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gwkprvqsv.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gnfemzehs.sHtML


<!-- 参考信息 -->