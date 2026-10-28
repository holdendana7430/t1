代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnqzz.top/gtjyltuvji.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.0kj1m.cn/gtlihmwrhl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtptpyomhf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtcpmuyvia.html

================================================================================
来源：http://hz.52xcode.cn/gtsctuhmie.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.birdmap.top/gtevktmmsd.html

================================================================================
来源：http://hz.yj20258.top/gtalukxtrp.html

[Q01] 创建表
来源：http://hz.yuanzhike.top/gtiqreyyld.html

CREATE TABLE users (
来源：http://hz.cucudq.cn/gtxcxzcixs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtsumkheyt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aibaodan.cn/gtxlnjqsus.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shangyingyoupin.top/gtzsbesxhn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtejkhstvo.html

);
来源：http://hz.smart0.xyz/gtxmcfwrmy.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtctdxwchu.html

CREATE TABLE orders (
来源：http://hz.aizwys.cn/gthxoywiry.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gtfrkqtajx.html

user_id INT NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtbsjjjqid.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gtilgxplsb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuxming.cn/gtbxumtfmf.html

);
来源：http://hz.redwolf501.top/gtkykrauwl.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtyyqmwbtd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtonohiiqh.html

[Q04] 修改列类型
来源：http://hz.jinyuanbaomall.cn/gtmjgqyiov.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cucudq.cn/gtibwnorke.html

[Q05] 重命名列
来源：http://hz.jqgfzy.top/gtbcchmqgn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangkeji.top/gtrpcitwjm.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtjviaqzrk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gtpnmgzinc.html

[Q07] 删除表
来源：http://hz.svipenyu.cn/gteyopkwac.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuanzhike.top/gtcyaszfup.html

[Q08] 创建普通索引
来源：http://hz.zhengqikj.top/gtsqizdwrv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtpmpznvdy.html

[Q09] 创建唯一索引
来源：http://hz.jianghu66.top/gtwopsyuja.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtodralxla.html

[Q10] 插入单行
来源：http://hz.tianlin.xyz/gtxnnxufld.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cashguo.top/gtsakxhrox.html

[Q11] 一次插入多行
来源：http://hz.wangdashe.top/gtpnccsfzx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtbfnpdprf.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtvwsuvzdd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hysaishi.cn/gtgbuajncn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtwttmplug.html

[Q13] 忽略重复插入
来源：http://hz.pycfn.com/gtecwfzlqg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gthdehjlgo.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydjk.org.cn/gtyfinndrh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yanxiufei.cn/gtdgwraftd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fzhhl.top/gtohncdekz.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gtcxncpyot.html

SELECT * FROM users;
来源：http://hz.c1oappe.top/gtghozodeu.html

[Q16] 查询指定列
来源：http://hz.cdnleiting.top/gtbkqpjvnw.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gtfzytrbmi.html

[Q17] 条件查询
来源：http://hz.ivvv.top/gtffxgcckb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gtewphoyti.html

[Q18] 模糊匹配
来源：http://hz.hysaishi.cn/gtgrjairjs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinyuanbaomall.cn/gtmgwcqbep.html

[Q19] 范围查询
来源：http://hz.ydjk.org.cn/gtfcndyrie.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtmmbxntur.html

[Q20] IN 列表
来源：http://hz.shuidangran.top/gtsdgxsrta.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtfvhktwnw.html

[Q21] 空值判断
来源：http://hz.chenjidiqi.icu/gtyrvlhtpx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gttdmmdmur.html

[Q22] 排序
来源：http://hz.cqqwz.cn/gtkmskhvtx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtrgiquinl.html

[Q23] 分页
来源：http://hz.tian-w.cn/gtvntpengw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daria6918.cn/gtwuosxhke.html

[Q24] 去重
来源：http://hz.cheryme.top/gtxmmdvami.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinyuanbaomall.cn/gtyexfnlmn.html

[Q25] 只取前 N 条
来源：http://hz.chenzaomai.com/gtmpbbwwnv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sxryk.cn/gtkegoxwwe.html

[Q26] 计数
来源：http://hz.9152youxi.cn/gtmtjqteor.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gtmuhzunsa.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtkokdsevg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shzxlz.cn/gtqqseypdc.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtcggfwlre.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.vqdsnc.cn/gtzyspnzze.html

[Q29] 最大最小值
来源：http://hz.yuanzhike.top/gtrsopuefl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenlongwang.top/gtqvuwulmq.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtafsszzrs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtcwjwanvt.html

[Q31] 分组后过滤
来源：http://hz.jinghuilouyu.cn/gtxyhftmrw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.birdmap.top/gtbijlatye.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtuhuopnyo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtmlzcsvud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258.top/gtxamihpmz.html

[Q33] 多列分组
来源：http://hz.tanke756.top/gtbigqnhig.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.meibo888.top/gtisueqhqa.html

[Q34] 每组取第一条
来源：http://hz.yangfankeji.com/gthhmisisx.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtrjabvizm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtlxnjvmyi.html

) t WHERE rn = 1;
来源：http://hz.daxiang520.top/gtlqerghho.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtrduvgkbq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtawhihyuo.html

[Q36] 左连接
来源：http://hz.zhaomingkeji.xyz/gtfwbbaoba.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtphdmpegs.html

[Q37] 右连接
来源：http://hz.shanyushiyangkeji.top/gtrklvvqwk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydjk.org.cn/gtrwxvivtt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtohhucvde.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tian-w.cn/gtjohutjwk.html

[Q39] 自连接（查上下级）
来源：http://hz.hongshengwenyu.top/gtdhyvvuyw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinyuanbaomall.cn/gtjlraneck.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ehwqpu.com/gtzlwtiabh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtyphvkoqi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tanke756.top/gtrysaqyla.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gtjpemnukw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxinkj.top/gtpfaddxuv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangkeji.top/gtaouukqmd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xinyue.icu/gtriffcxim.html

[Q42] 连接条件附加过滤
来源：http://hz.jinyuanbaomall.cn/gthibmsdsl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtcvkeuldb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtvjpktxwu.html

[Q43] 标量子查询
来源：http://hz.wangshuangyany.cn/gtljocczyf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtcuyhnylb.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtlfbyeopl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenlongwang.top/gtfydrdlrx.html

[Q45] EXISTS 判断存在
来源：http://hz.shuidangran.top/gtznukopym.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtfqwaneiy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangtech.top/gtfbrodsam.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtkwiszdfk.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gtxvnvdywx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gtgbrrsvek.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gttntbtpca.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtopnfhmnn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhoulong.xyz/gtychmnldq.html

[Q49] 更新单行
来源：http://hz.yongpay.top/gtwrwfaogf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gthgqcslxt.html

[Q50] 批量更新
来源：http://hz.shanyushiyangkeji.top/gtquzbuidy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinghuilouyu.cn/gtjrxbsvik.html

[Q51] 用子查询更新
来源：http://hz.c1oappe.top/gtckjpucuo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinyuanbaomall.cn/gtuisdssfw.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gtkfhtrsvj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangtech.top/gtgdevwxan.html

[Q53] 按条件删除
来源：http://hz.sxryk.cn/gturidoiqd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hywenlv.cn/gtxmohnzan.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gtukfzqutx.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtrgmvvzqi.html

[Q55] 排名（并列占位）
来源：http://hz.ydjk.org.cn/gtnndmcdrq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tian-w.cn/gtadordsec.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtjzwqikez.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gaohongyu789.top/gtvvbgnwmq.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtuhnphwmf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtijccgkpl.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtsdtzlktw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258.top/gtkeqhzaez.html

[Q59] 分组内累计
来源：http://hz.fzhhl.top/gtduhbocvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtmwuhvoix.html

[Q60] 取上一行 / 下一行
来源：http://hz.jlsjyb.cn/gtzwvowggq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gzhubu.top/gtqbkidmci.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sufxvd.cn/gtsmtkmvab.html

[Q61] 移动平均
来源：http://hz.nanxinkj.top/gtsjhnmgsg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ivvv.top/gtkwgdqfbe.html

[Q62] 分组占比
来源：http://hz.0kj1m.cn/gtujtrtpfp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtgskdoipf.html

[Q63] 开启事务
来源：http://hz.jinyuanbaomall.cn/gtsjzgsmbp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtqsqvejrx.html

[Q64] 提交事务
来源：http://hz.wangshuangyany.cn/gtdvxgryqc.html

COMMIT;
来源：http://hz.quarkkingdee.top/gtfmkygwsl.html

[Q65] 回滚事务
来源：http://hz.nanxinkj.top/gtkzhgarbr.html

ROLLBACK;
来源：http://hz.cucudq.cn/gtekuxhpvv.html

[Q66] 行锁查询
来源：http://hz.jlsjyb.cn/gtdjzgrssd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.316326.xyz/gtzxjhyden.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtyxwstqtr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhixingplan.top/gtzvqnnbyf.html

[Q68] 保存点
来源：http://hz.jqgufenzy.top/gttyajrlzs.html

SAVEPOINT sp1;
来源：http://hz.xinyue.icu/gtibempuyi.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtvcwxwllz.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtpgqhjhix.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtfrodunvt.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gtkwysnfbl.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangtech.top/gtrsmysryl.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtzohdsbqd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtlutblkzj.html

[Q72] 查看索引
来源：http://hz.haohaochexian.top/gtetlzqbpr.html

SHOW INDEX FROM users;
来源：http://hz.jqgfzy.top/gtnnrtwvhe.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtzttovant.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jianghu66.top/gtxzuyyvsa.html

[Q74] 强制使用索引
来源：http://hz.jqgufenzy.top/gtkaehnejn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gaohongyu789.top/gtaqtbtbgn.html

[Q75] 日期格式化
来源：http://hz.dashuyun.cn/gtkddlpqvm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtcedumtfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenjidiqi.icu/gthkaqwvts.html

[Q76] 按天统计
来源：http://hz.hammf.cn/gtkdfrlybf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhixingplan.top/gthskakter.html

[Q77] 时间加减
来源：http://hz.nanxuanxn.top/gtnvrgnnxv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.iojbl.cn/gteufoelpc.html

[Q78] 当前时间
来源：http://hz.pycfn.com/gtxiaqtfni.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tianlin.xyz/gtccdiqune.html

[Q79] 字符串拼接
来源：http://hz.svipenyu.cn/gtodngmkyv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.meibo888.top/gtqfmvsdsy.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangtech.top/gtldwiikpv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtefxaaqga.html

[Q81] 字符串替换
来源：http://hz.shangyingyoupin.top/gtnjysnuua.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtsmyxjcol.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtcsqolksw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtxlrndmyj.html

[Q83] 大小写转换
来源：http://hz.fengsongda.top/gtrcotqnvq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gthuhzuibe.html

[Q84] 去除首尾空格
来源：http://hz.sxryk.cn/gtubbkshxo.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtaucglkjy.html

[Q85] 数值取整
来源：http://hz.vqdsnc.cn/gtnfegkzws.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.redwolf501.top/gtcxfsytwp.html

[Q86] 读取 JSON 字段
来源：http://hz.jyoumei.cn/gtsbyxcnhb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jyoumei.cn/gtctgwolct.html

[Q87] JSON 字段做条件
来源：http://hz.nwbrower.top/gtjanmjkaz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinghuilouyu.cn/gtshqaspjd.html

[Q88] 行转列（条件聚合）
来源：http://hz.snrcjt.cn/gtubuuelsz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jlsjyb.cn/gtawfjyqww.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhaomingkeji.xyz/gtnwgcftmt.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtgsarvdak.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gtwftninnj.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtwcqayqin.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yangfankeji.com/gtyxicfsgb.html

================================================================================
来源：http://hz.dianchejie.cn/gtckpxevnp.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtxtcwuqhm.html

================================================================================
来源：http://hz.xinyue.icu/gtswolsmzz.html

[R01] shebang 与严格模式
来源：http://hz.daria6918.cn/gtqfpgulep.html

#!/usr/bin/env bash
来源：http://hz.316326.xyz/gtwvvfclte.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtykdcvnfg.html

[R02] 变量赋值与使用
来源：http://hz.daria6918.cn/gtkgwqjpyt.html

name="Tom"; echo "$name"
来源：http://hz.svipenyu.cn/gtuwpvsbah.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtxdagsdmf.html

readonly PI=3.14
来源：http://hz.gotoacloud.top/gtklrptkdu.html

[R04] 位置参数
来源：http://hz.ehwqpu.com/gtxxygxhcy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ppjwa.cn/gtggfcvaiv.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtipixupaa.html

name="${1:-default}"
来源：http://hz.nwbrower.top/gtgaxtndle.html

[R06] 判断命令是否存在
来源：http://hz.zhaomingkeji.xyz/gtrmeejzfc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtzypgzxvv.html

[R07] if 判断文件
来源：http://hz.chenjidiqi.icu/gtdpwcdaik.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gtenvsbxfh.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gtbsatscaf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sweek.top/gtssfnjfgi.html

[R09] 字符串比较
来源：http://hz.jlsjyb.cn/gtsgjvonue.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fzhhl.top/gtqnfrvumc.html

[R10] 正则匹配
来源：http://hz.jinghuilouyu.cn/gtsmelvkrx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.bjfxy.top/gtsadzukad.html

[R11] case 多分支
来源：http://hz.hnxiangtu.top/gtrpydiegy.html

case "$1" in
来源：http://hz.ivvv.top/gtdpaflfry.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtrbujvkvd.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtuqtzjnff.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gtkkrxkcch.html

esac
来源：http://hz.hysaishi.cn/gtbeizenph.html

[R12] for 遍历文件
来源：http://hz.jiagoushi.top/gtcgtjazkn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gtwfxcetyb.html

[R13] for 计数循环
来源：http://hz.cucudq.cn/gtvygopucc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258888.top/gtmdzsubdw.html

[R14] C 风格 for
来源：http://hz.zhoulong.xyz/gtlahtscqp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtkuoulzoa.html

[R15] while 逐行读文件
来源：http://hz.fzhhl.top/gtqchvornl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cdnleiting.top/gtkwxqcswc.html

[R16] until 等待条件
来源：http://hz.zhaomingkeji.xyz/gtojwvkuqw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gtjlygqhij.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gtsthtvrlb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtdrhtxqvc.html

[R18] 遍历数组
来源：http://hz.ehwqpu.com/gtctkjruhd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenzaomai.com/gtdquerxfi.html

[R19] 数组长度
来源：http://hz.daria6918.cn/gtzxhrxdwy.html

echo "${#arr[@]}"
来源：http://hz.yanxiufei.cn/gtvevqmzsf.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gthdmpxxrx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.52xcode.cn/gtfvobktxg.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gtghxkcruk.html

echo "${#s}"
来源：http://hz.snrcjt.cn/gtywijsozg.html

[R22] 截取子串
来源：http://hz.chenlongwang.top/gtxjxndyst.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtxdvqhpat.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtscjhcrgy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtxehbyhky.html

[R24] 大小写转换
来源：http://hz.cheryme.top/gtoxrblrkj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtlcsvserb.html

[R25] 去后缀 / 去前缀
来源：http://hz.cheryme.top/gtywxqqrvd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gtrkrhpslg.html

[R26] 命令替换
来源：http://hz.sufxvd.cn/gtycbqzysr.html

now=$(date +%F); echo "$now"
来源：http://hz.jinyuanbaomall.cn/gtvemrrldf.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtucyltrpo.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtfkcykkwg.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtwsvivlyp.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtypvzmcei.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtaulukvyu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtrexkjcax.html

[R30] 函数返回状态码
来源：http://hz.mhx1999.top/gtksbpqals.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtaymwcwos.html

[R31] 局部变量
来源：http://hz.snrcjt.cn/gtnrfwdfww.html

f() { local x=1; echo "$x"; }
来源：http://hz.dianchejie.cn/gtugyxjjou.html

[R32] 参数个数校验
来源：http://hz.xuanzx.com/gtxppvnpof.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.mhx1999.top/gtjlfspuow.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtlqharbtg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guowangkeji.top/gtkcybqsas.html

[R34] 退出时清理
来源：http://hz.0kj1m.cn/gtngewbffy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtqnlgmceb.html

[R35] 后台执行并等待
来源：http://hz.guowangkeji.top/gtoblbpimf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tian-w.cn/gtiqlgrkzp.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gtwjyjsxfb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hysaishi.cn/gtfpcncknp.html

[R37] 把输出赋给变量
来源：http://hz.zhixingplan.top/gtfukbzvse.html

files=$(ls -1)
来源：http://hz.hnxiangtu.top/gtmbdwznyn.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtrzuojuua.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinyuanbaomall.cn/gtufqcshun.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtkpcrvxtb.html

cmd > out.log 2>&1
来源：http://hz.tianlin.xyz/gtuqiwpgvi.html

[R40] 追加写日志
来源：http://hz.shanyushiyangtech.top/gtrjgikdnc.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gtacnvzpke.html

[R41] 丢弃输出
来源：http://hz.mhx1999.top/gtwayidlaa.html


<!-- 参考信息 -->