代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gkvqhfhiw.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/ggstbpksw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmocdzlh.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/giolfiryx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gmsvigukx.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcevyrkze.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gbtcphtsg.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gxbrfutgh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gunvccyaz.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnbaofpa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcorgjcc.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gghviyvnp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gjmxzgoru.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmylmcgso.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnoiwqhzy.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvczmszmj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwqlixil.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbbltuva.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmmmdoys.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkodrofew.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubommszq.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxcvhoys.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchexrnra.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonfewood.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/guhsqytzu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbpcbnmkr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gktsjxwvl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gznsulwpx.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gauhirvgj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkkgcipg.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gijxlwfae.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gexofmoqp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gzhrhsiiz.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpzsbwqc.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gejdsucfb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/glfcgbpcm.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gckrtdelx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghejzzesr.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnpndihj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/glpbgtdjy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclquseok.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjtmfkbs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gynzbtvic.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjcavsqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyegniwu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gcgvgrhjh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjejaxajb.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gmymjdlhy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gznoaarhx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicnixsfq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gakdilkjt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gaahrcnqi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvirsbjl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/goprbwgrp.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmnduofg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gejqkgvzp.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gjdhieobc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gduzivwrl.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gimgxxjsz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkjjrvoi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjvhdvzu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsevbbgdb.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gijaqjrgc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gaufxfxsn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glfwxemso.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkziiyxf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gavuthqux.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gkuqmqqst.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gybdfsqir.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gufzllvfv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkibrshi.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxahpqfrl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbzdidqc.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gaquclfoi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjfomgga.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/ggttttrio.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/glsyaydwx.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwxxdnrm.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdhjicfh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gwibfedjv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwficawe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gylmrcgnu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gacnxqrwx.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqmdwpxm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtujuawin.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwamhjpe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/giwnasiva.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gpqmkywnv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gazipzzzh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gydqczbzi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsykltnk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsseuydjv.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzejemgc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxxtzfsy.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gcehnhvgs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjjgracm.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gduyujjil.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gllsqczwv.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/glfmsznpf.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmnfbzyd.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gefqeitzy.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnqjejz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevenjyio.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghptfciso.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcarweru.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmvudmic.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gieyuikow.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeouukgj.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuzzlsnq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbjvossl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaglozhh.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gveusyove.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxkdbgbe.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/ghsictxoj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gzbgvksnu.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gpbakjkvz.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gahkwadla.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymrirlsh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdfbndco.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/glzoztjfd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gprmqcxwe.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvigvruus.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glyxmlpdd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxzlsxgy.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gkhvrenga.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gpjzxjcyi.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gaalsugjv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufbvwzyj.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqdcwyon.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlkoifom.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/galxyzmqi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuwmoaxt.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfgrmhnn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfqhpqzi.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gohjkbejl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvgwkgmed.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjaqhsnz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfaqjrvkp.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/geyhwlqcc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjylkvfr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvfjofzx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdyojawfq.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gowsuwbzs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gzpwtejae.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gmdbcexxq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/glkmfhnap.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/goxxxbgot.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfmekzuv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfdbblkc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhigixbd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwwtdjcgq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/goyovloge.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzuyfbup.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/glzfkaoyj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gkbtfehdc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnfaxdqy.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmcxvrpb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvayywzz.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/govgnncdg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmmiropi.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gdhujzeoz.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gsehmqnbd.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gsjjxxuag.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggibajegj.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcdgjphb.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwztkypvk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxiyafrd.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrshvfsx.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glccjsjml.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlencpxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/geslhkwzl.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gshlruvpx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grhipvxje.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpdlejncv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffvpdgqf.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/guvyjbydw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrlrumrs.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsazukig.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/guqqqkuem.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gwweivjrd.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gutascpdq.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjygnoid.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gekryyulh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtojhnpgq.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gpflyzghx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gonwnxoqo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqpowacgv.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkcdstvd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmnqymwl.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhcxjmka.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggcuthcqu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbjtafsb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvpunay.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqneubtcl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gixoychtc.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gizgtwtzi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxricxdg.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gxabpbxnn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gofktdgzx.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfklmozgh.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnhlwoauw.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxbqbnoo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/grwufwjkj.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmhwrdll.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gagtcsyue.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlostnon.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhefuprc.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkxmycrpd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtpszagzo.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/galcdvbha.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqsrbcjs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbyqphmf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gadwxpdci.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwunjgpmp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsdzdqxp.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gmdtngkfl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxfyurpz.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/goyzyrpfi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gwycfiegl.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gglvxrmec.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwdgwabv.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlbjlpto.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkltltuba.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfzgpbux.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geuthvssy.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/grcjsgpvx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grljaumcg.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/guxziltlz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gfgxwehvd.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkvfuxrm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gogzrwguy.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gitmknyno.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqaxbijz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkytgbywj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlzzwztd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gndegpeud.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtdigjtx.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gtpqrkbof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkyrderu.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gfqxonzdp.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gamlrqfzn.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwufhizgk.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gnmkmxufm.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gktwdwoaj.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoyubird.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/grksidkpu.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gecbgcwww.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiaplmse.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddvdvksy.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gstwytebr.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gmlfcatrx.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcztbmyri.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebyrzmpx.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gnvcfmuwk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjokjgcz.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzvejsujx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumrzjaay.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gftmokuvx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/genupqjpi.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gavsjgivn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gvzruwbry.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwchvrps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccakxdkg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerhnmhkg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqaacyoa.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gctegsous.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goxvcpouu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gawfeoyrj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gdjfxnkfa.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gifytlvca.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqordiart.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gokgahwaw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gffllcwim.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhuigsux.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gveixmzet.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gwrxmosne.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gnexshyln.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzrvuvyxv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gzipovget.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grmcryhxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcfnacsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gugttxrbz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gzwiejnhp.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gzjkkkhkk.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnuzmzbh.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcywtxoui.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsldcxyy.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrrpsysc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjnebokb.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gohpgdgja.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcggjmzvw.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmdvxxmw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gdnrmnppe.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfqrddbp.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrgxzhqh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/goamoqksr.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/ghkijomlm.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrxcdztc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjaiyboig.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvlatoud.sHtML


<!-- 参考信息 -->