代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gwfickgon.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gyqjhenzl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gneoirydr.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/grokgalih.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gfusmpdqn.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gdcwbpodi.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/ggliqhgoa.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gysrvbiuk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gusxqmhit.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gecpzatjm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdpiqxdce.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gsksckoqm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkijdxwfp.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/grtmvuqvh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghrnfyfjj.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gvjvzljvz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvdvqmhsq.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gvuvjzrjr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/grwrrmwxl.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/giqvrytza.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gegpxvxva.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gcyzujgzs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gkchogzus.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gevcvpheu.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gjuuwaiyf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gkibaoeaj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/glxytyvam.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gqlcffijj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gkdpbdnyd.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gmetphifd.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gdovvngkx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gfhuxidbl.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gsywpeyow.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gppdzmyin.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gzqvpvmwb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/giraqowqe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gdpliujmn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gwdcvduhe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gmhflrior.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/grjiyrcwk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gbafkhyjs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gcnqnomxr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gboldmkkl.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gnbhtjwmk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gfggltebh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gsjhbivmy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gvlktsbgv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/ghiyvlzgz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gdpvnbzho.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gigmayvye.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gotxkuslx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gvbdujxyq.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gbcqftbwn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gbjkuudtj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjlijzf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gjldkthxj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/ghzsnyaxw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gkdrxgmaj.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gvfyitkne.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gusjlprzn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/grxyvdggk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gqhgqietm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gzzyuicba.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gftjohpam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ghmdxqgli.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/ghfpuifgj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gdehpvhum.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gmcqbqudx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gbonzhpzd.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gytzcueqc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gyovummmg.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gwjadmdsr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gpkffdnov.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gqzflegfc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gvhmncjum.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gslcnbtno.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gxmfegiyb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gbdlwuugo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/giqoqmkyq.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/grxuslwsm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/guamllxcm.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gfatomfty.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqrvxoxgx.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gaymkaasu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/goolxmwmw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gxlfcdndi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gvmkanyzj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdbhpujuk.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/ghqhqakhb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkvvezrzx.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/goiptxzkf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gnmymchod.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gpgffyxdt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gnibungmp.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gaodoseig.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/ggufsgbtw.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gnoanbpow.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gouskaioz.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gktknqmlv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gqprnsemj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gwmolnxaw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gvvpalvwc.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gisfgwlqf.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gqrofbpsa.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gzcefsrqm.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gyxtdpviu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gzlsthveo.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gyohfjchg.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gyjqesevb.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gvzytxncb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gxfjcfjfr.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gzjahsoyl.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjhjidwxx.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/guvhigjjq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gnnvoplnj.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gefwvuhpa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gqjjshfpm.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxtdagfyg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gotymqmij.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gprywomlv.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gwvnvkeps.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gdilhucsh.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gtokzytye.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gboohuzoi.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gnaeatmqq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gvctcdtaz.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/grlkjjqoj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gnztishta.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gtehwklnf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtnqqncks.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gxyztgmhg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gafbqyqej.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/goabvsunl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghtgxojif.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gretjkrqq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grdlclhgk.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gvvmzlrrd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gyxruhxjy.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gdblyfrbp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gemepmizt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gcytjrqnu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gkivjnieg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/ghnppmush.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/givtdmwdd.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/getwkipmq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gtcebpjko.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqafmjzzs.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gdmxpfkpt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gqflsizxm.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gxeumyurb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gexiyloda.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcbylqcbi.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gmaasdpyf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grzllvsnj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gvsiltcce.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gmxofmkra.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gbiknrmar.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gjjgippwe.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/genzbsobh.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gkrklsqoh.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gwgcqtfzx.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/glhfrolkp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gvfrywnxb.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gugynuifz.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gvbozhqgh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gntwxtypa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/goemjwjlq.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/ggvlymrqf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/ggwaknapa.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gcslifmlj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gwkbwpamz.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gzocxyfzq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gvntbcaog.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gcauldutw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gskchivwx.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gzraxkbwe.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/ghjluqvyk.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/glwaxttfp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/glucxdrgk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gxppiepum.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gzszzufxg.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gpucthyhj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gmveyxljd.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gvulqbcwx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gioacltwq.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/ggyqplmwd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gblsqwzaw.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gbxhzcjbw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gvkmfnlht.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gdatnqzgj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gfzilnghn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gmmimeixe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gegmlsxce.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gnoxcnirn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gtaaqnrjk.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gigxdbplo.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gzetbppdl.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gkgfdohxm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gativnvkn.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxcpigejz.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gmetulnov.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gkonxcicy.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/glrtpuumt.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gumtvapcg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gydmflmec.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gumqnmdra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gmkzceptv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gzwvczvdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/guftmblpz.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gpezewaoa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gkrxttmkv.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gjonmnbvr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gfmnzwsmr.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gtjbeedps.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gboecehhh.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gizhskqir.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gscebfait.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/grbomsbsz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gcgpuvlaq.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gckwazmph.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/glilyddwt.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gclykqnky.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gcjfykxtg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gewdscpun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/grzujbtux.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gaazhuswi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gyxijimun.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gjkcvbtmk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gcovhvpwe.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/guqzazfkk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/ggbqyhbkx.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gbimxbntn.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gqirjuewj.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gnmcrfmex.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gcpfttqrw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gantzyfwu.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gopswties.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/ghnvmpwwt.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gzrtpuavd.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gmmbvteei.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/glknovagg.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gjorcxawm.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gcawjmuqd.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gtiqjvfye.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gfkarffap.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/glzegojlw.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gosbodghu.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gobkssyaj.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gxbgtkqko.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gssvazapq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gyunejxrs.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gwdmmzgfh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/ghkukqhiw.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gxfqpwlsj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gdvbqpliw.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gdlhlirle.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/goihgoigi.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gptsjhqby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gtuzqxjhv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gngytlvou.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gepsmdtnx.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gsjuoopkz.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gfpamibed.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gievdntrg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gujfqiluu.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gkejhxhsj.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ghzikkasz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gegznvpkr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/grpigwtef.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gkpraiwvj.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gwbciukpy.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/glujoexoy.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gytjfzezu.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gfpkszwxg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gykjaahno.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gweeesfah.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gnuhetiha.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gjombkqyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gqgacelkt.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gejnpfmjk.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gqywlvbpd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gluentjtu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gafmpmebs.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gtgkpmnmt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gndbkwzip.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gtygmymgg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/goorklxkk.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gjpmhxsuc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gaivbjdsv.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/ggvcpyyox.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gxjfyyzpe.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gnrlkzova.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/ginxssduy.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gapectgbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gklmnxckl.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gxuxffusm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/geqyrvxhk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gqfikqfbk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gopdiwdws.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcpewrexq.sHtML


<!-- 参考信息 -->