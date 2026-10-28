代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daria6918.cn/gtjsirwjcg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jianghu66.top/gtnzzulxuw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtikydjdap.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtnhngsrhb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrdhocnjs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.kuanghao11.cn/gtapcwrzdp.html

================================================================================
来源：http://hz.sysykeji.top/gtxjdanqpc.html

[Q01] 创建表
来源：http://hz.jianghu66.top/gtzoabhjpc.html

CREATE TABLE users (
来源：http://hz.tianlin.xyz/gtlquaceku.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtrbsabucs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigfzy.top/gtbnmsaxkm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cdnleiting.top/gtkkyzoyvi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.andypj.xyz/gtggrlgflb.html

);
来源：http://hz.jiagoushi.top/gtrhlodeqc.html

[Q02] 创建带外键的表
来源：http://hz.zycfv.cn/gtwtmkaneh.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gtvwrlkwlg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtfpftqqvp.html

user_id INT NOT NULL,
来源：http://hz.pycfn.com/gttlgzbfhy.html

amount DECIMAL(10, 2),
来源：http://hz.fengsongda.top/gtqpgjmtdh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yangfankeji.com/gtsncfgmyz.html

);
来源：http://hz.jinqigfzy.top/gtwcpzmoik.html

[Q03] 增加列
来源：http://hz.daria6918.cn/gtnbqawzwa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.c1oappe.top/gtsayiimyx.html

[Q04] 修改列类型
来源：http://hz.gogol.net.cn/gtelfdwcqj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtmcfatyhd.html

[Q05] 重命名列
来源：http://hz.ydzc1.top/gtqclfjbzu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtrkwhbydr.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gthzsebqmd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtgxdupntf.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtsurndqzd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangkeji.top/gtfaezfsmd.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtvirbwoen.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cucudq.cn/gtjexceiez.html

[Q09] 创建唯一索引
来源：http://hz.jinqigfzy.top/gtfuncuhjr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtenchugqz.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gthwrnqntb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.mhx1999.top/gtvhfmfgov.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtznazvxck.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.mhx1999.top/gtyosadquh.html

[Q12] 插入后取自增 ID
来源：http://hz.svipenyu.cn/gtoyfrvzuy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgufenzy.top/gtrnigtjtf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtpngxbfiu.html

[Q13] 忽略重复插入
来源：http://hz.ivvv.top/gtgsnqrifc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shuidangran.top/gtbrypcers.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtqkncujrp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtackwiqlw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tian-w.cn/gtjmbbqqqd.html

[Q15] 查询全部
来源：http://hz.aizwys.cn/gtwmwewuou.html

SELECT * FROM users;
来源：http://hz.hongshengwenyu.top/gtvsrqfmql.html

[Q16] 查询指定列
来源：http://hz.gogol.net.cn/gtncknadkn.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gtivlbeazx.html

[Q17] 条件查询
来源：http://hz.ydjk.org.cn/gtkstzganu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.iojbl.cn/gtwzsjhqij.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gttgakybdu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.birdmap.top/gtboirnsfv.html

[Q19] 范围查询
来源：http://hz.jinqigfzy.top/gtjzccttsn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.birdmap.top/gtcpygdunx.html

[Q20] IN 列表
来源：http://hz.sxryk.cn/gtjddzqfqh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gttlhqsouc.html

[Q21] 空值判断
来源：http://hz.quarkkingdee.top/gtnbhgzcgl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gtodfcldqo.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtazscrgof.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.0kj1m.cn/gtubefjiqp.html

[Q23] 分页
来源：http://hz.c1oappe.top/gtajtvfzig.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fengsongda.top/gtgspolfiv.html

[Q24] 去重
来源：http://hz.daxiang520.top/gtxmeiotnk.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gtqrzltdfq.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtksiprlcu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pycfn.com/gtyvpbyiki.html

[Q26] 计数
来源：http://hz.hfpthk.cn/gttdfwsobc.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gtautwcwiz.html

[Q27] 条件计数
来源：http://hz.52xcode.cn/gtqomotrvu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinyuanbaomall.cn/gtosqvqneg.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtvdvztvki.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtsvoommxd.html

[Q29] 最大最小值
来源：http://hz.wangdashe.top/gtphtskvtg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtyuzkrylm.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtczrafiqj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtvdtqxdmr.html

[Q31] 分组后过滤
来源：http://hz.guowangkeji.top/gtsrwfusar.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtmwicdfnx.html

[Q32] 分组拼接字符串
来源：http://hz.xuanzx.com/gtzopgsbwo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtloxdufkd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.svipenyu.cn/gtgflclqrr.html

[Q33] 多列分组
来源：http://hz.feifeiyinyue.top/gtzkkgmwlh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258888.top/gtlrdqsqez.html

[Q34] 每组取第一条
来源：http://hz.cheryme.top/gtnpanizlh.html

SELECT * FROM (
来源：http://hz.gotoacloud.top/gtzfxukuou.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhaomingkeji.xyz/gtmhzekwfe.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gtxboxqxes.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtweotmabp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtwrzsfrrv.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtnyhpnlcv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtsfdxuiin.html

[Q37] 右连接
来源：http://hz.xingfuxueyuan.xyz/gtnnotkoot.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtvbnskpdq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtuzraxtvz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhoulong.xyz/gtwemuseou.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtsobjckav.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gotoacloud.top/gtftskvoik.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgufenzy.top/gtgxsrdmix.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtonbngfth.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxinkj.top/gtqfyogefq.html

[Q41] 多表连接
来源：http://hz.chenlongwang.top/gtjujuahvw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.svipenyu.cn/gtndxsizqu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aizwys.cn/gtvaekjfqs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.svipenyu.cn/gtebjrppkm.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtjhbuikeo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fzhhl.top/gtubalqjnj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.0kj1m.cn/gtvagkjdxn.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtwhfkwlzl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.havefunace.top/gtbnkmqzee.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtrordeqro.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhijiandao.cn/gtwnsablab.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtnwtzsrzp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtzntcfufd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.vqdsnc.cn/gttauyqmhe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtvexnwcjm.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtinvazxwi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhoulong.xyz/gtbetbnmnz.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtrfrebbws.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hongshengwenyu.top/gtwbsahogp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtyqjzhhop.html

[Q49] 更新单行
来源：http://hz.sweek.top/gtjwrupczh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtcvmrytnm.html

[Q50] 批量更新
来源：http://hz.jqgufenzy.top/gtgwdsnlhh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtbcdgjtze.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gttowmgzfi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.smart0.xyz/gtcimxhtrh.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtnelkurry.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtphaljfcc.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtbjcmrjyj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtsjaqbvel.html

[Q54] 清空表
来源：http://hz.gaohongyu789.top/gtqaeqzjuy.html

TRUNCATE TABLE logs;
来源：http://hz.hammf.cn/gtyumaijnj.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtmyarplqf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jianghu66.top/gtvlxlbubt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtxtrllwil.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuanzx.com/gtuocdmckj.html

[Q57] 行号
来源：http://hz.ehwqpu.com/gtakpmqhnq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuanzhike.top/gtvmnybajb.html

[Q58] 累计求和
来源：http://hz.mhx1999.top/gtotsdbgwh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtfalndjza.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gtngswthaa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gtrcytrywj.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtnumdkmxx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fzhhl.top/gtmygmofye.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cucudq.cn/gtrfeagpbt.html

[Q61] 移动平均
来源：http://hz.hongshengwenyu.top/gtfoayucbn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gzhubu.top/gtjxreuqva.html

[Q62] 分组占比
来源：http://hz.chenzaomai.com/gtrindadhz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtaipeujqh.html

[Q63] 开启事务
来源：http://hz.zhijiandao.cn/gthyxhxrkq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hnqzz.top/gtdekgdhvf.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gttnxhvngj.html

COMMIT;
来源：http://hz.dashuyun.cn/gtygisvjcp.html

[Q65] 回滚事务
来源：http://hz.ivvv.top/gtowaxziyl.html

ROLLBACK;
来源：http://hz.snrcjt.cn/gttrawbclg.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtmdccwkzu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ehwqpu.com/gtmisdbajx.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtdnfrwjvk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.316326.xyz/gtjujzhqrp.html

[Q68] 保存点
来源：http://hz.zhiwuduotai.top/gtpaxyiytn.html

SAVEPOINT sp1;
来源：http://hz.jinyuanbaomall.cn/gtaptebdrg.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtokvayzzx.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtjzrlybhc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtzjetrykb.html

[Q70] 更新统计信息
来源：http://hz.jqgfzy.top/gtgpvcsinh.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gtvzgibvgd.html

[Q71] 查看建表语句
来源：http://hz.hywenlv.cn/gtuuapgcmp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtjiqvkrto.html

[Q72] 查看索引
来源：http://hz.sweek.top/gtymgudtse.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtkggujnrm.html

[Q73] 查看表状态
来源：http://hz.yueranfly.top/gtndttsdtj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhaomingkeji.xyz/gtddnncwue.html

[Q74] 强制使用索引
来源：http://hz.fengsongda.top/gtwjjrshfo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtegizxmii.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtpjhtfagy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gtgwrmcgge.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.quarkkingdee.top/gtbybirxns.html

[Q76] 按天统计
来源：http://hz.zhiwuduotai.top/gtnxmpqhus.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xylfe.cn/gterhmmhrk.html

[Q77] 时间加减
来源：http://hz.tian-w.cn/gtlhfnuxgv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuxming.cn/gtmanycdip.html

[Q78] 当前时间
来源：http://hz.zhengqikj.top/gtxblpbkwu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangtech.top/gtzdgehryw.html

[Q79] 字符串拼接
来源：http://hz.smart0.xyz/gtruousecu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuetiantiany.cn/gtmnwbrkuv.html

[Q80] 字符串截取
来源：http://hz.yj20258888.top/gtddneuorj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtjfqrvqip.html

[Q81] 字符串替换
来源：http://hz.wangshuangyany.cn/gtgmhmgoxp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sxryk.cn/gtlmicddzr.html

[Q82] 字符长度与字节长度
来源：http://hz.havefunace.top/gtxhwzlfah.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ybcxt.top/gtqifkzrfi.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gtjlyxlmsj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtzyfwyuvy.html

[Q84] 去除首尾空格
来源：http://hz.zhaomingkeji.xyz/gtgevmdnxz.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj202588.top/gtfbhrayok.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gtszhidpnk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gtrgwbrllw.html

[Q86] 读取 JSON 字段
来源：http://hz.chenlongwang.top/gtghswjxsd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yangfankeji.com/gtzzqifdwk.html

[Q87] JSON 字段做条件
来源：http://hz.feifeiyinyue.top/gthecqubrv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.snrcjt.cn/gtqkeayknn.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtzsftxkih.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtmbllgemk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydjk.org.cn/gtdedcalgy.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtqxyvrbiz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.vqdsnc.cn/gtcpuzlgcq.html

[Q90] 生成序号列
来源：http://hz.jqgufenzy.top/gtvsasynem.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtbszmpaem.html

================================================================================
来源：http://hz.yuxming.cn/gtnzoejgus.html

R. Bash 专题
来源：http://hz.yj202588.top/gtrnkphgts.html

================================================================================
来源：http://hz.jinqigufen.top/gtajepmrwx.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtvhuibtfn.html

#!/usr/bin/env bash
来源：http://hz.vqdsnc.cn/gtjccgqaip.html

set -euo pipefail
来源：http://hz.hnqzz.top/gtcawznsgb.html

[R02] 变量赋值与使用
来源：http://hz.c1oappe.top/gtxxlhzcxg.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gtnjzxtizz.html

[R03] 只读变量
来源：http://hz.sweek.top/gtguyhjaiq.html

readonly PI=3.14
来源：http://hz.yongpay.top/gtwdykxwtw.html

[R04] 位置参数
来源：http://hz.52xcode.cn/gtcoeybiak.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.kuanghao11.cn/gtvxywinwa.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtctgujyve.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtwslpktrw.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtmmmrtyfj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtgbkcgwrs.html

[R07] if 判断文件
来源：http://hz.sweek.top/gtejwacivg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxinkj.top/gtvoeknvpj.html

[R08] 数值比较
来源：http://hz.aibaodan.cn/gttmxyfzhc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shangyingyoupin.top/gtznuomfyo.html

[R09] 字符串比较
来源：http://hz.zhengqikj.top/gtvmqmqmie.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtwpnjndas.html

[R10] 正则匹配
来源：http://hz.feifeiyinyue.top/gthqqmiijv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yueranfly.top/gtvfxbzqgc.html

[R11] case 多分支
来源：http://hz.andypj.xyz/gtvgnndyrk.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gturgenbdj.html

start) echo "启动" ;;
来源：http://hz.yj202588.top/gtgwjkgosa.html

stop)  echo "停止" ;;
来源：http://hz.nanxuanxn.top/gtnshlviqc.html

*)     echo "未知命令" ;;
来源：http://hz.wangshuangyany.cn/gtpjiqczam.html

esac
来源：http://hz.hnqzz.top/gtkivywpzl.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangkeji.top/gtpehabxov.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigufen.top/gtvfrslxtt.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtstmezfix.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gogol.net.cn/gtsfzqtkmh.html

[R14] C 风格 for
来源：http://hz.yanxiufei.cn/gtzxqieeah.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtfyeguucr.html

[R15] while 逐行读文件
来源：http://hz.dianchejie.cn/gtsswpfanz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangshuangyany.cn/gtyawlkjrb.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gtykatwres.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gtusjfxsaw.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtzunqijqi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtlpzqrmpk.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtbsxvkvqc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtphgkffnn.html

[R19] 数组长度
来源：http://hz.daria6918.cn/gtimrauhmo.html

echo "${#arr[@]}"
来源：http://hz.xziqi.cn/gtsdhevrin.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtjicnshis.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtxgzbenqj.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gtpdzconcu.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gtfdawacui.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtxtdgsjmj.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtwojjsrug.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtjtfuzvmv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.bjfxy.top/gtjiaohkkw.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtiynpzanw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gtuyowmwmn.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangshuangyany.cn/gtvowgannv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ehwqpu.com/gtebbjjyfk.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtnjvzwdvu.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtfqkpiqek.html

[R27] 算术展开
来源：http://hz.yanxiufei.cn/gtztmvnmox.html

echo $((1 + 2 * 3))
来源：http://hz.xziqi.cn/gtdfsuqgle.html

[R28] 浮点运算
来源：http://hz.hnxiangtu.top/gtougkwiga.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtvgrgtqrr.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtsjskjstj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.smart0.xyz/gtnywqaloj.html

[R30] 函数返回状态码
来源：http://hz.zycfv.cn/gtffttbfcg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jianghu66.top/gtjmigixrf.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtordddvqn.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gtipflabjp.html

[R32] 参数个数校验
来源：http://hz.meibo888.top/gtgixlljdo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gtqccopzal.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258888.top/gtgbebnpfu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yanxiufei.cn/gtvxgbocpc.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtsvoeotxu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtntjzpoka.html

[R35] 后台执行并等待
来源：http://hz.ydjk.org.cn/gtqckeltzk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnxiangtu.top/gtqhosxaps.html

[R36] 并发执行多个任务
来源：http://hz.tian-w.cn/gthdijwuxd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jianghu66.top/gtfhywrhkh.html

[R37] 把输出赋给变量
来源：http://hz.yongpay.top/gtgyzwlfvj.html

files=$(ls -1)
来源：http://hz.ivvv.top/gtkiltzldc.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gtefyzpffd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtbpvnpfqb.html

[R39] 重定向标准输出与错误
来源：http://hz.birdmap.top/gtwpsskjpg.html

cmd > out.log 2>&1
来源：http://hz.zhongyouzk.top/gtawcgjwbn.html

[R40] 追加写日志
来源：http://hz.yvedp.cn/gthfstkkug.html

echo "log" >> out.log
来源：http://hz.wangdashe.top/gtxanllzcj.html

[R41] 丢弃输出
来源：http://hz.zhoulong.xyz/gtvalnopok.html


<!-- 参考信息 -->