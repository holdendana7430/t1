代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glttqwhqg.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gxjetawwr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdvwspur.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiuykzlo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gtfysbwam.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzwnheep.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/griysukia.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gpipjmptn.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwkikfuw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmqyfxgn.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwoodmy.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gsbrypsgf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpuzmjiw.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmuywmwtp.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gtnliuzee.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gskobavxt.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqczqmbh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyobobep.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gwsemfhsh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfdwrqan.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgkisdnb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjrkuvyj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gssctjtab.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbspgymgk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyfvtpjb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gbywisnjn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcekjewe.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gurzqfgza.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdbgvaxk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gvptherfa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsckiulmd.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpsslktq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/glparjqvn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqxptnaw.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/goxopiekk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcolunkb.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gbkazwcat.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gvfpomtnp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gcswakcaa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gidddweyk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrterdex.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgwguvsp.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqggbuejw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gvxhuamdv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gcktkwpjj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcsqpuvq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/ggpbwbfnu.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/glylouavt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gphzdfwuq.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/geafwmpeg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gtqiqusqo.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxworncv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxixqrfy.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqkydfom.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbizobrw.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gnvyftiwb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gtbgnpxsw.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpynzxjjl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gzwtawmxo.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gkuuicmcs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gdfipjwrh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzdhcrcp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbyhhcdd.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxwdqebf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpwpnvqn.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfldqrni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grreqrjod.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitihjdyw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gjmmhmccu.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gycnldyns.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gyywrwnyb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjfuoizgv.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouwehfex.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gydzlldsk.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gikavebvt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/givzgqvnn.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsmehwbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzrtiqta.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gevfineks.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gslxduvqj.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvuezqds.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/ghgcwsvrs.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gchbfacgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwofipzxr.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/ghwwasxeb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/goqpvwuij.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/ghgnpcexf.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnvcwfkw.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdpyyzmk.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gcparsmix.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gsggikwgz.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/glkheyipi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafjzriit.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyxebrel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsurbxyz.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ghljravae.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftvieovp.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/geyytfzwh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoampvrg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgpkolio.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/glrbmxmlm.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggliarnne.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxubtglmp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gncnkbgnp.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gomhhrdet.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gihswivkl.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gywmsdqpb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gfxxuklrj.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gpujxcndi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gcwscxewh.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gpggtnkzj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvcwjlft.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gjatylncr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmxhjatt.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgdqadgp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwicdpxb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gushxsmyj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gymwqvrhq.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsabzqai.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxhkbmy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givgiiows.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzijqbkbe.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbnturfz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfbhtekv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzjhdxfa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gijcenimo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuzqdiao.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggydlgqm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gyflkatud.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gudkudzra.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqjuwebgx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsqeqyio.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gfkkiuvav.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/glligyndy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpadxqtwy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghudfmvei.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpsxfubi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwvsvqztu.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/ghfmtvypk.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/glsymzvxl.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/geavgwxpx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/garlouzpf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gklbrjikh.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpolzmjjx.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyehhqsv.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gykuwoawl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtednuau.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvhtntrq.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdknujhr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gwewhefhk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmihgedwu.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guodqwbpa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxysficy.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcqzmxco.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gddtkvwhz.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjkmclbt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwpinicu.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcabqqfvt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvgbcghc.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gnihmmzuu.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvpclmdh.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfylnpoot.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifcscfun.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gssvbcwxh.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcydhyyu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssdyhzo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqvbnmep.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gjwnywzpc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvjmantfq.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gghjcrnmv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gllxhzmut.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfyzswph.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glutfddwl.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzidgbsi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlaukcmp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsaapqcw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwzlmiipv.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiekubus.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gherwsjpi.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/grikehnml.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdyasmpwi.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gntupuadt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzmvdzla.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gaaweqiju.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocjewawa.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqztryqe.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkdhozsl.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxhchskwz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gewiefizf.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxszrhkkn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfxswekum.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gdbnoahso.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrgemzlw.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqvntdmfz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gdpgqzzxm.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gempwdkjr.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbdzifbo.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyqhcztk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiwrhwvt.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghvyyruga.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtzmowikb.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/grwbzixko.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gsdgebwxk.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkoqscov.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcxwidbm.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/giubnfodj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwiaxqcd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkucbbpd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gzqgzrsxm.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gvmcyutac.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gqddamvud.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdvdmtmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxskuwleg.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gvezwzowu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gawlpuhkb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtynnyxji.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/grpwsyjun.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gdbecfguo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/grcerdbya.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gccxpdvqo.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpymsqtx.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgcfvcug.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/ghqhprjfn.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gqodbutee.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gvddabjcx.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gscjnavfl.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gixvelcdn.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxcecjb.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gutfxsfxd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotvljobr.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gijthbgmm.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gxmnhoubn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxdgmhwh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gstcslyqx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gchwponyf.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gthtkedkt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwizcqymu.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gonhxnxdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmskxfrwd.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcsvzvtv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gywnxnnaf.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gttvseekm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsinshptx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnylnekc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtecbuxq.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/glgciwacp.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goefqhevg.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/giqhockhp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlqmnbqn.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvpmwjlq.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydaiahyj.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpsbznyl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/grkdppmgt.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcrwcwvz.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gqvymxkea.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmgsqmst.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvxxoags.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgrjrkci.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/guokpneyh.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcagxfrt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gynwdvljf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbztvpvvk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gwyuvvzai.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gffzrmizj.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqkzggda.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidjcxqqy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghgdpwfl.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gnwhxkhxr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaaduakb.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosmmuiju.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnttjwvr.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyrrhacz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/ghjtmurtz.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/glgafunnc.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gelpimaox.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtvmfppa.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnkfocsp.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ghmeaywyp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gemzgbsjb.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gwobwmltn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gbrtaeksp.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gsveqyawv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gntrbwssj.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gtcilubfz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvdqbau.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpltpibfm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsfaetri.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgqvyybt.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gykmzttut.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgpecepw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjhgnkbyv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgxzqwhm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbbatfza.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giyzskmua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkkccaet.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gtjtnjded.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gptnasxng.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gkzhbqbff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngxktpkx.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gkgxbtsvn.sHtML


<!-- 参考信息 -->