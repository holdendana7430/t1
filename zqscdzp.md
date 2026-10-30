代发 wailian999

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpvvhmkyx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/giiqwnsmn.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gyuinovgm.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gchiebyiv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gtqssrwoh.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gtrwzfomm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gmaesnaea.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gqwgcplgn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/giahvfsdx.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gtbfsbstz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gflsxvxqt.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/ggpmjxbto.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gtmdrxqtk.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gnlibtwxv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gstwjtxku.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gbsavdhvx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/ggrlgrnmg.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gpszfebvi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gzybcexta.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gziouobpm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gigynllbx.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/goujlxelq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnhujlznw.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/grxohtkzs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmrsmusla.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/givlllxrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glxhimncq.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gxttogqow.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gakqenjmf.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/geozlhboc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gtldliqhn.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/ggwtwlppb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gusbwswrb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gryhnpngh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnyrsltje.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/grucnpmaj.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gnzjpddok.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gxsbfcncp.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gqnrhwruk.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gltmawyrn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gdqklbwxw.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gngbustla.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gyqvewytp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/grnhtvxjo.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gtvudreby.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gamjubkzk.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gqkcwebhv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gulrkbwfd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/ggbqchunq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gqkfdyqre.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gvihwcjqp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gkdtnktzo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gflcabdrn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gtpbhailv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gwyshvric.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gxbnqrbjx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gehlwhrms.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gkmrctucp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gumqaemik.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gnzbwudwf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gmiwelzph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gtdqpvwiz.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gcjmfqmeu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gqtbttjgj.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gzuwwhagc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gdnnhrzxv.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gnmjyzynr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gluumaepl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqieoimww.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/guevyfqnv.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gxwrndsho.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gohxzpwgr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gandfkkdw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gyirnplqq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gzpugnrnb.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gmjydswau.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/goeailavb.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmeoecnxe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gufwsfryn.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gjmaosuld.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gdxsgbumi.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gwjcdqxmr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gjkofkwas.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gykvuceno.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/ghsydbtgr.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gsajquhjh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gvhuzgoch.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gxwhdfumm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gbjbodkup.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/giymfacxr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gygtzrjze.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gdayqrstn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfdseuzgy.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gggafhczi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmctnrkqf.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/glbhtkflp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxbegfifg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gedfliarp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gbfeouprx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gnomnkgki.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbrmfax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvpxncnhq.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gtfzcayxi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/geqixnbed.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gefppvvsi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gvwclxnui.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gvvdeccna.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gnjbvksli.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gfevxggmr.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gxqjwcgho.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gdyavjawt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gxgpofvju.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gkdwcjtdm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gwlwbbxbx.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/goxhhrrxm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gvgcpntxq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gjrisegpb.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gltwhiopz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gksnnjarw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gcuilmalz.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/glrmqsdgu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gefdaqahy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gbrrqcxoj.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gmvpkronu.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gylfcrbho.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/guscjrikh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gwskqopzn.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gbtsdetrq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gmrvtzkpl.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gsbpoqaos.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjrjcuvor.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gmuknuqsp.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gwngranmk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gproatwyq.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gexlrtxah.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gqfmsudsa.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gucgbjkvp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gbwfhcrrk.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gifwwsyaw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gjgsjqpaz.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/glyxiaocu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfugoesev.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gnjbzdodk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmheuquow.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gaaikizyt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtkcmdknd.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/geyzbptux.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdqodxmzr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gkkldkbsa.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnjqorrkn.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/grhytqusr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gbgzcfugx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/ggwxejuqf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gdicimbxd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/glnekftmj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/giwieurdq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gljltrcmk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/grodauafj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gecfhgecx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gqwxfderu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gxqkzguud.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gkfoxcdwh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gjdfonfqr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gekwniqih.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gfqudgvot.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsjcyyhaz.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gtmtavlpb.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/geziuyvvh.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gxltrhhkf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/ghsuwehzz.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gzhjujdui.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gdfpcvnip.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/goawypzpb.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gayessxgp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gxveqndyb.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gnujphfbw.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gcojjmkim.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gukudcute.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gwtyawbwu.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gvarchvdr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gypmwmdhv.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gvnpezbiu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvahzqtqn.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/giuhcpttn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ggfcbfdlf.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gprgbosbq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/glqcjxgcj.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gwddojukx.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gosqovaha.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqduzupa.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/goqxgxmxt.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gpgrbxxll.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gbuaphlvy.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gmakvditw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gijilvuzz.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gagnguipy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gbtvpuiip.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gxnahcdbv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gxfhxhtcl.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gzrcagvvl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzstxwnwc.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/glkcynngz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gxcpqigoa.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gzcmonzbt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gvzkdiost.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/guwfveucb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghzbdmprq.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gqhcneuac.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gtwbmzucd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gywuxcovk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gwtngtkko.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gwyxqhpff.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gnzhszgwt.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ghsrubtxo.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gaklwrohs.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gofpfeusq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/ggvxtiels.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gfyvtobgk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gotnzlsol.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gqxnkztwx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gxoukiaug.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gzqklxqvf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gzttpusgj.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/ggemcocnn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gmznooqmh.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gbmonpalz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gmxpkruip.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gxevkumjs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gqvxmvjsi.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/goxfbnomw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/giswqbaul.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/ghgkjupjt.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gwjsgcato.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gfmhwnpnf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ggrgramow.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gjkbdtqkw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gtgwvjmae.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gavsstrms.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/grbbqejgp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gnlgrhpqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/guhnqebge.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/ggdebsubl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/ggzrbzqlj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/ghcxfkcvf.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gijhcdlwg.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gfbybxljk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gubxwcimh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/ggnsjveww.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjilzmykk.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwpssycju.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gobriupmt.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gulvyortc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ggotjvijk.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gncyhvbwp.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gizcmxvtr.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/ggftvywve.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gswbzdtnn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gftyrbetl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gggozdqlu.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/ghywzfutw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gxkkdidtw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gsjfcwpci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gknauwijy.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gptlhdjbh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsywzhnrs.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gtfcxmekk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghwwdmkwd.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gazmsjqgl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gutovqury.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gpkqteazq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gogknhnlw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gawrklovd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gjcfsowzt.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ggtwfzhyi.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/glnbtaxej.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gbxlxnnut.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gxfzfwfzs.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gdhvshfkt.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gtkftocbv.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gdrekzvst.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gkllgyjds.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gcruhmipm.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gddnxlvou.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gytxxbdru.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gscuajzpu.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/ggpbeuanm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gwlgltbql.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gegpxtvjr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gfogysqmw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzsdpjg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gwbhmrmrw.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gfxvxxunz.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gaechgmyh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gsgxgjazs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gahmmfvzj.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gbtvxgzqr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gzitiokrl.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gnfmgykwm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/ghlyoqdrv.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gbxwkvsyd.sHtML


<!-- 参考信息 -->