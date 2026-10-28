代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhengqikj.top/gtdcgplqem.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ehwqpu.com/gtcxniwwwb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtxomvmeil.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtafzzazrh.html

================================================================================
来源：http://hz.gotoacloud.top/gtkcptbkah.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cheryme.top/gtppwmfrcs.html

================================================================================
来源：http://hz.fzhhl.top/gtdjplobgs.html

[Q01] 创建表
来源：http://hz.yangfankeji.com/gtezwuseyc.html

CREATE TABLE users (
来源：http://hz.shuidangran.top/gtxocrpioc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtrzucdorg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gttrxbpcwr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinyuanbaomall.cn/gtcisfivvp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtvzhzqcph.html

);
来源：http://hz.yongpay.top/gtwqfdsrdh.html

[Q02] 创建带外键的表
来源：http://hz.zhoulong.xyz/gtvpreyyig.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtnxlfvrbz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtwyofbcrg.html

user_id INT NOT NULL,
来源：http://hz.pycfn.com/gtazngbure.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtsqftcsur.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxuanxn.top/gtozyemdex.html

);
来源：http://hz.yangfankeji.com/gtoecdtwuc.html

[Q03] 增加列
来源：http://hz.yuanzhike.top/gtjzpijshw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtnlehmtdo.html

[Q04] 修改列类型
来源：http://hz.wangshuangyany.cn/gtjonxrwmk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zdqjudy.top/gtgtypwikc.html

[Q05] 重命名列
来源：http://hz.cheryme.top/gtcdedszkh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtsnzrqstg.html

[Q06] 删除列
来源：http://hz.daria6918.cn/gtldcbkuzh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinghuilouyu.cn/gtawyshwhw.html

[Q07] 删除表
来源：http://hz.sweek.top/gteqedgumg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.316326.xyz/gtyggzoout.html

[Q08] 创建普通索引
来源：http://hz.shuidangran.top/gttcmtwzky.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.mhx1999.top/gtggrvodtg.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gtujiklczc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtcjpvdlwl.html

[Q10] 插入单行
来源：http://hz.shanyushiyangkeji.top/gtbxlcswzc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aizwys.cn/gtlvnzxpip.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gtvksdafgi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gtebuadeav.html

[Q12] 插入后取自增 ID
来源：http://hz.zhaomingkeji.xyz/gteohacjol.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cheryme.top/gtzmecwphq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtuoktneaw.html

[Q13] 忽略重复插入
来源：http://hz.yueranfly.top/gtyuxdtzjn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangshuangyany.cn/gthvmgffuv.html

[Q14] 存在则更新（upsert）
来源：http://hz.cqqwz.cn/gtehmsargt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtxxinsdfm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shangyingyoupin.top/gtdtwinyod.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtqrxtsutv.html

SELECT * FROM users;
来源：http://hz.jqgufenzy.top/gtbpiomzrz.html

[Q16] 查询指定列
来源：http://hz.ppjwa.cn/gtvxweuqub.html

SELECT id, name FROM users;
来源：http://hz.jinyuanbaomall.cn/gtbummkxhb.html

[Q17] 条件查询
来源：http://hz.yj20258888.top/gtgxxcqrgf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinyuanbaomall.cn/gtoaqjoqxj.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gtionslsmv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hfpthk.cn/gthzrbnsae.html

[Q19] 范围查询
来源：http://hz.yuxming.cn/gtqsomkuyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj202588.top/gtfdgmvybe.html

[Q20] IN 列表
来源：http://hz.nanxuanxn.top/gtmezvwtkj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnxiangtu.top/gtykquducg.html

[Q21] 空值判断
来源：http://hz.gaohongyu789.top/gthgllkeek.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgufenzy.top/gtmiqlenqk.html

[Q22] 排序
来源：http://hz.316326.xyz/gtdipjcmzl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtzpqtyiil.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gtolvudkjb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtpnxxngkz.html

[Q24] 去重
来源：http://hz.0kj1m.cn/gtiphyvdqf.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gtsrkjzhbe.html

[Q25] 只取前 N 条
来源：http://hz.shuidangran.top/gtliffgrwl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ppjwa.cn/gtnkdjwimx.html

[Q26] 计数
来源：http://hz.cashguo.top/gtftymigxl.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gtvgbshpxm.html

[Q27] 条件计数
来源：http://hz.yuxming.cn/gtckljshid.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shzxlz.cn/gtytjpoplu.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtdruiuoca.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtqeezvwvf.html

[Q29] 最大最小值
来源：http://hz.zhengqikj.top/gtjvnfczdp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtrpkfxgbd.html

[Q30] 分组统计
来源：http://hz.wangdashe.top/gtcqjijcai.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtnnoqwfjv.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gtwyinnbbl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gtvlszivir.html

[Q32] 分组拼接字符串
来源：http://hz.kuanghao11.cn/gtwjnyhrzp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtktwemcpr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtlkupaaqy.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtcdywwifc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtrjyhayeb.html

[Q34] 每组取第一条
来源：http://hz.yvedp.cn/gtbcdtgmgq.html

SELECT * FROM (
来源：http://hz.ivvv.top/gtiohgjtfr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shuidangran.top/gtlobuntaz.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtyuellkcf.html

[Q35] 内连接
来源：http://hz.vqdsnc.cn/gttwefaywq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtpgafyleq.html

[Q36] 左连接
来源：http://hz.chenzaomai.com/gtcodrirvo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtvkgdcjuz.html

[Q37] 右连接
来源：http://hz.chenzaomai.com/gtcpvtspbm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gzhubu.top/gtiwjopeef.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.vqdsnc.cn/gtgamiruxp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daria6918.cn/gtgkkhpxit.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtclqidntx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gtomhxsioo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigufen.top/gtoclnxrzf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtsmslsjpx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtgowwpzpr.html

[Q41] 多表连接
来源：http://hz.svipenyu.cn/gtusdqwflu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtthpktejw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gtvvrelqoj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxuanxn.top/gtkwnsclsq.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtsiggevpb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtynyivfsg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gtigrnqyjx.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtymftbyzh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtmesqyytw.html

[Q44] IN 子查询
来源：http://hz.zhongyouzk.top/gtntpltcvv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hongshengwenyu.top/gtsxwcvzxx.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtfqrbwqbi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtfzzypdfr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtgroajdby.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtnsdxykvz.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtkdrelldp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtihhaspia.html

[Q48] CTE 公用表表达式
来源：http://hz.wangshuangyany.cn/gtpsjvtert.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cashguo.top/gtqijggjyt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtdagyckaz.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtthebhfna.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cqqwz.cn/gtyoqbjrkp.html

[Q50] 批量更新
来源：http://hz.zhengqikj.top/gthrouvlxx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cqqwz.cn/gtsaqjsyec.html

[Q51] 用子查询更新
来源：http://hz.316326.xyz/gtvwugitqj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtujxhshqd.html

[Q52] 删除指定行
来源：http://hz.hnxiangtu.top/gteedcmlxt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.haohaochexian.top/gtmfwthgmc.html

[Q53] 按条件删除
来源：http://hz.sxryk.cn/gtioiuguqr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtbheuvhvy.html

[Q54] 清空表
来源：http://hz.shanyushiyangtech.top/gtvwpmuxnl.html

TRUNCATE TABLE logs;
来源：http://hz.jinyuanbaomall.cn/gtpkgyanyw.html

[Q55] 排名（并列占位）
来源：http://hz.yvedp.cn/gtsewpqruf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinghuilouyu.cn/gtgbapdbyo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fzhhl.top/gtggzvohcv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gotoacloud.top/gttumnwmnw.html

[Q57] 行号
来源：http://hz.yanxiufei.cn/gtncxzorwk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtmqljqcma.html

[Q58] 累计求和
来源：http://hz.zhiwuduotai.top/gtmdmacmel.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gtwhfjvdge.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtejcjhwup.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gzhubu.top/gtdgqbwadb.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gthlsbmurv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtnoanktdy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ybcxt.top/gtdhehnecp.html

[Q61] 移动平均
来源：http://hz.aizwys.cn/gttdqjpawh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yangfankeji.com/gtnhzevqch.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gtqivsunxy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtogsderec.html

[Q63] 开启事务
来源：http://hz.ehwqpu.com/gtetxwihuy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenzaomai.com/gtnnhpgejb.html

[Q64] 提交事务
来源：http://hz.52xcode.cn/gtovzxezyc.html

COMMIT;
来源：http://hz.zhaomingkeji.xyz/gtuqklltcg.html

[Q65] 回滚事务
来源：http://hz.316326.xyz/gtyconqaiz.html

ROLLBACK;
来源：http://hz.xziqi.cn/gtyorehajo.html

[Q66] 行锁查询
来源：http://hz.guannengcc.top/gtfbsxrose.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xylfe.cn/gtrehgudia.html

[Q67] 设置隔离级别
来源：http://hz.shzxlz.cn/gtfxbvlwnt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtccxjseov.html

[Q68] 保存点
来源：http://hz.svipenyu.cn/gtdqwhisbl.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gthwdmjujo.html

ROLLBACK TO sp1;
来源：http://hz.ppjwa.cn/gtnlgjrqtm.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtcmgcbedl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.andypj.xyz/gtfnbgfqbi.html

[Q70] 更新统计信息
来源：http://hz.ivvv.top/gtkgrtmjhs.html

ANALYZE TABLE users;
来源：http://hz.316326.xyz/gtczpveqkh.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtopoebzcp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xinyue.icu/gtmixwrkut.html

[Q72] 查看索引
来源：http://hz.zhiwuduotai.top/gtchprsjjt.html

SHOW INDEX FROM users;
来源：http://hz.jinyuanbaomall.cn/gttecvbpah.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtuslatziu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhixingplan.top/gtdkjojgbk.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtvzvwrzyy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtdicxjjoa.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtrvixewbx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtlworqegm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtioftlxpi.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtkzbkslyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fzhhl.top/gtyygozirm.html

[Q77] 时间加减
来源：http://hz.jlsjyb.cn/gtjayuhhdt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtsnvbphhe.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtbswevxft.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtvbdzowrt.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtjzciqgww.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gtluglwiak.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtdooswxus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtaonlzhwr.html

[Q81] 字符串替换
来源：http://hz.zhongyouzk.top/gtmqtrskzm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtnvcsbaml.html

[Q82] 字符长度与字节长度
来源：http://hz.dashuyun.cn/gtnjnyewgw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hammf.cn/gtozgmfhgo.html

[Q83] 大小写转换
来源：http://hz.havefunace.top/gtcnmknefg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtqijsogju.html

[Q84] 去除首尾空格
来源：http://hz.smart0.xyz/gtcfvmjydt.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtyfaxncch.html

[Q85] 数值取整
来源：http://hz.zhoulong.xyz/gttveedfqu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtcudlvlvs.html

[Q86] 读取 JSON 字段
来源：http://hz.aizwys.cn/gtsuyugwvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtltxdsnzs.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtiffwfzou.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cucudq.cn/gtkdcjngqi.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangdashe.top/gtyusxokmr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtcqypkika.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtpzhqdxnc.html

[Q89] 判断表是否存在
来源：http://hz.xuanzx.com/gthtnideug.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.snrcjt.cn/gtujzupuuy.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gtigpmevbh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtpycxnpto.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtfdydugae.html

R. Bash 专题
来源：http://hz.jqgfzy.top/gtbqsnusgu.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmcrukjzv.html

[R01] shebang 与严格模式
来源：http://hz.redwolf501.top/gtkosrvzzx.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtjuvhbohe.html

set -euo pipefail
来源：http://hz.yj20258.top/gtyxcphxmm.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtncxplrxb.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtzyeobvxb.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gttdvczyed.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gtwrgilyhv.html

[R04] 位置参数
来源：http://hz.yangfankeji.com/gtvjstwlrm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sxryk.cn/gtiaenhioi.html

[R05] 参数默认值
来源：http://hz.ppjwa.cn/gtjudrxasj.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtdnhgysyb.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtrnsdapnx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gttmodutuc.html

[R07] if 判断文件
来源：http://hz.shangyingyoupin.top/gtsyoqhymy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.haohaochexian.top/gtmaljvtlh.html

[R08] 数值比较
来源：http://hz.yj20258.top/gtdymxwbif.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtwlpvevbi.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gteqviirjn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.wangdashe.top/gtwsdxnqqm.html

[R10] 正则匹配
来源：http://hz.aizwys.cn/gtsffltypb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.snrcjt.cn/gtfbuhoioq.html

[R11] case 多分支
来源：http://hz.zhixingplan.top/gtiynieoli.html

case "$1" in
来源：http://hz.hnqzz.top/gtxxiiciur.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gtmxzkpcwe.html

stop)  echo "停止" ;;
来源：http://hz.meibo888.top/gtlprnuvrm.html

*)     echo "未知命令" ;;
来源：http://hz.tianlin.xyz/gtaczejpsm.html

esac
来源：http://hz.yj20258.top/gtqbayvjjq.html

[R12] for 遍历文件
来源：http://hz.snrcjt.cn/gtgcgclxlm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gtctaosmfw.html

[R13] for 计数循环
来源：http://hz.xingfuxueyuan.xyz/gtvpmxeyke.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jyoumei.cn/gtaofhpmnh.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtbigurhmy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tanke756.top/gtxsywozqp.html

[R15] while 逐行读文件
来源：http://hz.jinqigufen.top/gtfyincjqp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.birdmap.top/gtzbrhugbb.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtzzguzptl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj202588.top/gtmacgfoxn.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtnaudeggv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtaiwetyzw.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gtjltrtvwg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangdashe.top/gtpruaqewl.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtvolnhslg.html

echo "${#arr[@]}"
来源：http://hz.fengsongda.top/gtavsbthna.html

[R20] 关联数组（字典）
来源：http://hz.9152youxi.cn/gtqrmxorbz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gturwlybek.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtyuhgrnsz.html

echo "${#s}"
来源：http://hz.9152youxi.cn/gtdveabkmf.html

[R22] 截取子串
来源：http://hz.0kj1m.cn/gtnxocpvzn.html

echo "${s:0:5}"
来源：http://hz.zhoulong.xyz/gtlyszcvog.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtmobhjqfo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gtpovgombr.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtizobyxhy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guowangkeji.top/gtncitsluj.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtpexgobux.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.c1oappe.top/gtdlwvrwqk.html

[R26] 命令替换
来源：http://hz.shangyingyoupin.top/gtybpkujje.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtyfmzqbfs.html

[R27] 算术展开
来源：http://hz.zhaomingkeji.xyz/gtikgmqxsp.html

echo $((1 + 2 * 3))
来源：http://hz.yuxming.cn/gtumudgjgn.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtnvtkwzzq.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhengqikj.top/gtgpsaduqi.html

[R29] 定义函数
来源：http://hz.havefunace.top/gtyeodvljl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtnarkeokh.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtwpejnmiu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gtlxqiuakh.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtypqjitff.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtxigivebv.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtofmmrnan.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yonumen.top/gtfpretgxa.html

[R33] 捕获错误并提示行号
来源：http://hz.svipenyu.cn/gtosnzkwiu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtqsykbcsu.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtivytpdwm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtceihurec.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gttnrtxqty.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuanzhike.top/gttcvfmwms.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtnrgfpaaq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtzjdkhcpa.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtonyvsxkt.html

files=$(ls -1)
来源：http://hz.hnxiangtu.top/gtdwtumwkp.html

[R38] 管道串联
来源：http://hz.zhengqikj.top/gtuzratrlr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtiphxtykk.html

[R39] 重定向标准输出与错误
来源：http://hz.pycfn.com/gtjjetdfnz.html

cmd > out.log 2>&1
来源：http://hz.iojbl.cn/gtmoelflre.html

[R40] 追加写日志
来源：http://hz.wangdashe.top/gtykgctcrq.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtcbbhtrdw.html

[R41] 丢弃输出
来源：http://hz.hammf.cn/gtwqapavso.html


<!-- 参考信息 -->