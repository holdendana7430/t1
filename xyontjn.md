代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gkasdidux.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gartiilgq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gtntbyujg.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gvvdzhhac.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gtnwoibbm.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gjjhabzkq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gsxqsuvkk.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gavourngn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gqzybuknk.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/glejamixq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxgdfimox.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gbowxdbzz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gdeknwvtt.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/galgxovej.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjnifigls.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gkviavkol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqtioyiyr.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gwquvhoxx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdymrrrib.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gkuodezrn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqaokvsue.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gjewyjwzc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gfqafuuud.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/glbsiqsov.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gamiazeof.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gtdiepasj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkbqnqkqm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gpopvrpik.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gxpoqfglx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gnaouxlgc.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/goqqgvono.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gvegzfwhv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/ggdfbpdwp.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gsdynzotl.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gvfassrlb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gvswctkcz.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gvimaegpj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gixmsalde.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gtsehtgxh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gwpqttwgx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gncfrktwo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gcpfptulv.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gkdxkiilk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gsukbguxq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gmtiyhgiy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/giuaqvmes.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/ghumexuue.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gcsvwnzyi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gaolxdpgl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/girvxkrgz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gysyhywkk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gusszymib.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/grzjrmasb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/glpywdrfn.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gigkdetcm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gabzzjedt.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gvlqjlyym.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gxsrkjvri.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gwmaakttu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gclrdwurp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gefmgwzqw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gfzcrghcr.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gwmdcscqj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ghoaqtlui.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gvwmluumb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gwwmzvyxq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/grfgbccuz.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gdrxbkotz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gvmqcwgbk.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/goilyzhyo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/giuyvebyh.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gncjnxeke.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/guchagboc.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/glwjeweiw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gofoorsso.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gtfcttxao.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gjgcqkinz.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gsuufrpgx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gsddhupjc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gqddavmzn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gcxothljh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/glgawbmis.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gawcdkaku.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gietegtwc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gepkvxule.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gzqkfcjey.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gockpiymd.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gqjpwgpxo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggqtzcaqn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gxrmrfetk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/giindeobj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnuiedcjp.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gelsmbffa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grhxrgqbt.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/goyajxoio.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gnscduuaj.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gbtpfsczn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gcjkhhmld.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gzfgkklvh.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gdrivqpld.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gnhdjtube.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/grspamlob.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gockcqnjp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gjehndfsq.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gvvqjgfeg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gbervojdu.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gjdovoyfo.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gdiflbqpj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gaksbauzd.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gwdjakgva.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gdpgbnejr.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/glkljtnup.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/ghujhrzdy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gzdqislod.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/ghymvdivl.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gxatfkqff.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grguuwkvh.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gfndxhuox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gzsuvqdds.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gvqawzozr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gbprvqtir.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gdlkijoxj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcspjhorz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gaoadyrio.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gaknawdop.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gfuxrjaik.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/grecknmog.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gkbtedkzb.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gqecghaos.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gtbpcxkof.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gjilduqga.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gjffqvniz.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gsklathrg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtvuigdcb.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gyrjnnpgu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gvkywiyzr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gpomwpgfz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gucrrrlfi.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gmcqnuvjv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gatrdeako.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gcqjewfap.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmweanaj.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/ghbgderep.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gjdmrvdto.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/goegodpai.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/glfkmfshc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/guwwbnlji.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gubidvosu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/grsdweqgo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/ghfjmtnon.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gezfvtgur.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gohmrozka.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gwrsxryxd.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gipqbnwli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/geexdvoju.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goirtcmyu.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/guqfhfcdn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnzlftdkn.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gepygzbxq.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gxfzykmod.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/ggyzrziso.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gagrprfkc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gfutsymrd.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gtrmpapdk.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gicsscgzr.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/goxifuuty.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/givygymmk.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gdpsuvrom.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gzjvjlfnh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gpctalzrr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gesrgxwiw.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gjnbmlcnv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gywtmutli.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gkmivnlub.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/geqzfrekg.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gxkzmmogu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gjbvbsjkh.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gxtmufocv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxxkbkacw.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gdyfxkafx.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gxzwysrzq.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/guulojhne.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/ghuzqcmgc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gugizxvtz.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gbpfwfvwz.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gudrbacws.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gxrolswko.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gngvsemrj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gqlluzxed.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gtdpmtsmp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gzwdybeax.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gbaalxohn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gtolfmhtn.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gtfrwtovv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gfppzyhnj.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gwiujozxd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gqdfjsyeu.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gbxguvpfx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gjprcbvwc.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/ggsccwcqb.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gncenkdsr.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gwyhgyjcy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gcotatvgb.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gmjkdcvyp.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gbfmkycyt.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gdppmkcws.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gkucpmwou.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/grdkeqple.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gebwiptmy.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gajvgomhm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gexcvemna.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/grbtnsanz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gyteqfvhw.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gllhciubf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gwnsstmvp.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gtlgaebcc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gvuonnmgx.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gtburvuku.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gqfgteofc.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gsmmyfcsn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gasbpleon.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gsdkgonlz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gjwwhmear.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/ghvwjjqvk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gnthxoabk.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/goxqpqijn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gwvearxac.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gujjfwvxs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gtuzmaexx.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/guvtnrjir.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gvmmsvwth.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gljlidbke.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gokrmxmkx.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gaixlwvqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gwghzzdrm.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gmybtgpec.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gnsecqyed.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gtulyrxpu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gkflctxfz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gvrfatowk.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/glsydmbkp.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gdskhjiey.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/grmpkmhip.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gpizyutvl.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gqbllujyi.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gqoeelkkw.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/ghvihvbqm.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gicyzxzux.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gfbktjynt.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gkhlmddvh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gpvfbvmzs.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gfneglrzg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gwutvyafm.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gextbvrsi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gucahygrl.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gvewjwlna.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gajonazph.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gsvskruxe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmqmmmvmz.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gbkkcprsn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gdbvyikhz.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/guvnvoirh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gsgktowmr.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gkjyqlrxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gsltitene.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gctncxqti.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gxwmnjydc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/ghjxechnn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/guhndcvcj.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gvsoojlyq.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gtdnrggzq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gtceicoim.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/glzkiaabd.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gbeurtfac.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gxnwosvxv.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gjlmisfmr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/ginsypsok.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gzzmuaots.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gjupcsfni.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gngqhwjvv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gkyagnevl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gjytrgwde.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/glocstwpn.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gebusukoh.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/geqcgcfmj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gdvvcuhhj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gkrividdj.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gcxqchvqb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/guyfzspzx.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gaebvcagw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/ghebndcqq.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gzpljsmxa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/giibecnut.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gvgvfcrno.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/ghhgnnzjd.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gtcmyakdj.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gaqleloyq.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gfemopmaf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gqmomhxro.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/grkgvwkkp.sHtML


<!-- 参考信息 -->