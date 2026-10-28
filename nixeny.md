代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.feifeiyinyue.top/gtdgdocqjj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hysaishi.cn/gttayhqqkd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xylfe.cn/gtgqxcuafl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yvedp.cn/gtrxmdzjvc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hysaishi.cn/gtygcixjkz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangkeji.top/gtnmbiwmil.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jianghu66.top/gtmdmqobcb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtlilxnfoj.html

================================================================================
来源：http://hz.316326.xyz/gtiepiwlka.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangkeji.top/gtscqfxqxj.html

================================================================================
来源：http://hz.redwolf501.top/gtduubkxki.html

[Q01] 创建表
来源：http://hz.zdqjudy.top/gtvsbszfgu.html

CREATE TABLE users (
来源：http://hz.gaohongyu789.top/gtzkesncto.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtssanuffv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jlsjyb.cn/gtcffhmxvp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtomwmxhek.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.vqdsnc.cn/gtjqthrluf.html

);
来源：http://hz.jinghuilouyu.cn/gtdkglajpm.html

[Q02] 创建带外键的表
来源：http://hz.316326.xyz/gtiozawzmq.html

CREATE TABLE orders (
来源：http://hz.52xcode.cn/gtbvdnrvsq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtywcoubhe.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtrduppnos.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtuainuglg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtoieqztmv.html

);
来源：http://hz.zhongyouzk.top/gtqdvnxykt.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtarmbqjxq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydjk.org.cn/gteocbdgyo.html

[Q04] 修改列类型
来源：http://hz.ydzc1.top/gtgaufjxyv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtfvrabhlv.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtifjcimjr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtrftepkeq.html

[Q06] 删除列
来源：http://hz.tian-w.cn/gtgnjubqqh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtezvqkmuh.html

[Q07] 删除表
来源：http://hz.hysaishi.cn/gtgpnxdwrf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.andypj.xyz/gtflfjpixr.html

[Q08] 创建普通索引
来源：http://hz.yj20258.top/gtfohkrcsm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtsuhyntng.html

[Q09] 创建唯一索引
来源：http://hz.andypj.xyz/gteymeiara.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gttqrgvuga.html

[Q10] 插入单行
来源：http://hz.jlsjyb.cn/gtwgvtojbm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangdashe.top/gtmyaemqsn.html

[Q11] 一次插入多行
来源：http://hz.jiagoushi.top/gtpkxudgmw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxuanxn.top/gtudgvqsfz.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtppppeaco.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtpiyntdbq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ivvv.top/gtphvnwfox.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtlilgagea.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.c1oappe.top/gtqhrchsbj.html

[Q14] 存在则更新（upsert）
来源：http://hz.shangyingyoupin.top/gtbvwtkxdn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cashguo.top/gtmzznxoqg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gtekyjypea.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gtbfphdycc.html

SELECT * FROM users;
来源：http://hz.dashuyun.cn/gtcuffaqkb.html

[Q16] 查询指定列
来源：http://hz.jinghuilouyu.cn/gtukxuaddw.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtonvevunl.html

[Q17] 条件查询
来源：http://hz.hongshengwenyu.top/gtuqaqoqdm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtngsmlvmz.html

[Q18] 模糊匹配
来源：http://hz.pengpengdd.cyou/gtghlkipeg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xylfe.cn/gtqanousxh.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gtjlaevkkx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.9152youxi.cn/gteczzfdpc.html

[Q20] IN 列表
来源：http://hz.shzxlz.cn/gtztdpbizh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sweek.top/gtlipprrgf.html

[Q21] 空值判断
来源：http://hz.zhiwuduotai.top/gtztlrisvn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gtnhxmqoig.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtqfnwlsoh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gthiozbspj.html

[Q23] 分页
来源：http://hz.xylfe.cn/gthpfdulmj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtnipnkvgu.html

[Q24] 去重
来源：http://hz.yj20258888.top/gtkcprqdwv.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenzaomai.com/gtjpdjnxiv.html

[Q25] 只取前 N 条
来源：http://hz.zhaomingkeji.xyz/gtckvivjho.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtgbhiogth.html

[Q26] 计数
来源：http://hz.andypj.xyz/gtzegxtjkc.html

SELECT COUNT(*) FROM users;
来源：http://hz.xinyue.icu/gtkfrbybdt.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gteaybgdyk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.meibo888.top/gtxtsfpylb.html

[Q28] 求和与平均
来源：http://hz.316326.xyz/gtvvliuqmz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhengqikj.top/gtfuojqhke.html

[Q29] 最大最小值
来源：http://hz.gzhubu.top/gtvacsafhx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sxryk.cn/gtgjychbtv.html

[Q30] 分组统计
来源：http://hz.9152youxi.cn/gtqahrsyws.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtfjvfgsmm.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gttasmpmpx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.svipenyu.cn/gtnvrdjodn.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gtpoipotlx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtwtigvnyv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.feifeiyinyue.top/gtmipkfhjg.html

[Q33] 多列分组
来源：http://hz.andypj.xyz/gtoptvobjk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.havefunace.top/gtcogmthye.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtpexwhwtn.html

SELECT * FROM (
来源：http://hz.wangshuangyany.cn/gtvjgrqopc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuetiantiany.cn/gtoxydywdx.html

) t WHERE rn = 1;
来源：http://hz.xingfuxueyuan.xyz/gtzsrqituh.html

[Q35] 内连接
来源：http://hz.xingfuxueyuan.xyz/gtteocmztk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gteqtnxzew.html

[Q36] 左连接
来源：http://hz.smart0.xyz/gteprmdrhc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtkhkjeiqs.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtyhbbmnew.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gthnrkqryh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtzgjntjgb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtycaidyql.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtlvgtigqg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtaushbnea.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtcsxjoenu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtvxsegqjn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cashguo.top/gtmbijthzy.html

[Q41] 多表连接
来源：http://hz.zhaomingkeji.xyz/gtinnnoaan.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenzaomai.com/gtliobfenx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinghuilouyu.cn/gtpcsqvyrm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.mhx1999.top/gtwpeqqsko.html

[Q42] 连接条件附加过滤
来源：http://hz.ehwqpu.com/gtbrljdvlq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtduzxfhij.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtioacdzgh.html

[Q43] 标量子查询
来源：http://hz.fzhhl.top/gtrdsqhkfh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.9152youxi.cn/gtgsteiahi.html

[Q44] IN 子查询
来源：http://hz.jqgfzy.top/gtzcjdtiio.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fzhhl.top/gtsfyiliqt.html

[Q45] EXISTS 判断存在
来源：http://hz.fengsongda.top/gtdycfvbel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtninjfwdp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jianghu66.top/gtaoppkzmk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xingfuxueyuan.xyz/gtnvvvfgpb.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtqqauacsk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.feifeiyinyue.top/gtecuydcaj.html

[Q48] CTE 公用表表达式
来源：http://hz.zycfv.cn/gtknzqdqof.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gtnnqgvydy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pycfn.com/gtfyvrwiue.html

[Q49] 更新单行
来源：http://hz.kuanghao11.cn/gtqiqbdjwz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtrkuepjfw.html

[Q50] 批量更新
来源：http://hz.cucudq.cn/gtfynbhzif.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hywenlv.cn/gtmhgzqnac.html

[Q51] 用子查询更新
来源：http://hz.c1oappe.top/gtcoumsejd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtoagjjzpc.html

[Q52] 删除指定行
来源：http://hz.jqgufenzy.top/gtqlqyagag.html

DELETE FROM users WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtblltyppl.html

[Q53] 按条件删除
来源：http://hz.hfpthk.cn/gtcmwdwxyn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtmwlutnfj.html

[Q54] 清空表
来源：http://hz.ywan-chungtsiang.top/gtsxtefjwu.html

TRUNCATE TABLE logs;
来源：http://hz.zhengqikj.top/gttnmswksu.html

[Q55] 排名（并列占位）
来源：http://hz.sysykeji.top/gtgcwyldqi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtkrnxeatz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zycfv.cn/gtvbhbwzvz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.mhx1999.top/gtjhmyhapv.html

[Q57] 行号
来源：http://hz.yueranfly.top/gtrvjraeqy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258888.top/gtpeovonza.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gttpmzsvgv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhoulong.xyz/gtfqotoxyy.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtiswemjio.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gtdlqsswjp.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gteueirmqy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.c1oappe.top/gtzhdegvqe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigufen.top/gtkcaobszv.html

[Q61] 移动平均
来源：http://hz.jqgufenzy.top/gtgceyjzcg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jianghu66.top/gtjivoclnc.html

[Q62] 分组占比
来源：http://hz.gzhubu.top/gtlzsuqlcl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtcnrkjtik.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtkkyosxwr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gogol.net.cn/gtrhbazltf.html

[Q64] 提交事务
来源：http://hz.quarkkingdee.top/gtqgriajbg.html

COMMIT;
来源：http://hz.quarkkingdee.top/gtnsvtjukc.html

[Q65] 回滚事务
来源：http://hz.tianlin.xyz/gtigzyymll.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gtgllpznlf.html

[Q66] 行锁查询
来源：http://hz.zhixingplan.top/gtepwcqlpu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtfjroikda.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtvndtondl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xziqi.cn/gtdtlfxhvk.html

[Q68] 保存点
来源：http://hz.yvedp.cn/gtjhwutdol.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtndwvdtmw.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtyvxofgzz.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtaeoewnlj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtsnrfcxwz.html

[Q70] 更新统计信息
来源：http://hz.pycfn.com/gthnhwpyno.html

ANALYZE TABLE users;
来源：http://hz.andypj.xyz/gtzqcledmf.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtxhflzjzk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sxryk.cn/gtsaziwvfz.html

[Q72] 查看索引
来源：http://hz.dashuyun.cn/gtcuveepuz.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtfuvyrahs.html

[Q73] 查看表状态
来源：http://hz.bjfxy.top/gtimdhsmpd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hysaishi.cn/gtsdxyijms.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtdljigioi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sufxvd.cn/gtnnwdszzp.html

[Q75] 日期格式化
来源：http://hz.52xcode.cn/gticihzixj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtiiwclfgt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jianghu66.top/gtinasdbjj.html

[Q76] 按天统计
来源：http://hz.hywenlv.cn/gtftpdnhal.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtstwqzrzm.html

[Q77] 时间加减
来源：http://hz.cucudq.cn/gtmioeobla.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtimmuwwdf.html

[Q78] 当前时间
来源：http://hz.zhiwuduotai.top/gtbrvouwvd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gtkojaffef.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtdoquyaeu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtklpraypy.html

[Q80] 字符串截取
来源：http://hz.chenlongwang.top/gtpjstyunw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jiagoushi.top/gtycsgcjen.html

[Q81] 字符串替换
来源：http://hz.yj20258.top/gtsqynypeo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtieenhkcj.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gtqmhmmwfw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydjk.org.cn/gtcmqyvrbw.html

[Q83] 大小写转换
来源：http://hz.pengpengdd.cyou/gtojpkbzrt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cqqwz.cn/gtojnqrcpy.html

[Q84] 去除首尾空格
来源：http://hz.feifeiyinyue.top/gthenaidjh.html

SELECT TRIM(name) FROM users;
来源：http://hz.bjfxy.top/gtpnlopszd.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtsyqpsgds.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuanzhike.top/gtrbwjaqez.html

[Q86] 读取 JSON 字段
来源：http://hz.dashuyun.cn/gtcevuxnce.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gthhatweou.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtojqftjhb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cashguo.top/gtuetaqjtj.html

[Q88] 行转列（条件聚合）
来源：http://hz.tianlin.xyz/gthyfrnhdy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.snrcjt.cn/gtitdjzqfw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangtech.top/gtkcimezcw.html

[Q89] 判断表是否存在
来源：http://hz.yongpay.top/gtmkancbug.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fengsongda.top/gtilnhnapz.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtrzooyadb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.havefunace.top/gtuepqrlym.html

================================================================================
来源：http://hz.aibaodan.cn/gtlxljqvll.html

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtrsfsnycr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtxcamedih.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtvtzmxktv.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtwtngkhxy.html

set -euo pipefail
来源：http://hz.cucudq.cn/gtngykolbd.html

[R02] 变量赋值与使用
来源：http://hz.yonumen.top/gtdwsjcuxr.html

name="Tom"; echo "$name"
来源：http://hz.zhongyouzk.top/gtyfyospjw.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gtbjjmojhj.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtcfgwquxe.html

[R04] 位置参数
来源：http://hz.jqgfzy.top/gtgandcvmc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnqzz.top/gtfavfpaya.html

[R05] 参数默认值
来源：http://hz.ivvv.top/gtduetvpgq.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gticnvogpj.html

[R06] 判断命令是否存在
来源：http://hz.chenzaomai.com/gtohawjdjm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.52xcode.cn/gtsucmyeot.html

[R07] if 判断文件
来源：http://hz.ywan-chungtsiang.top/gtuktnachv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.iojbl.cn/gtzbiivjnr.html

[R08] 数值比较
来源：http://hz.pycfn.com/gtcqhtjamc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtoresdmxw.html

[R09] 字符串比较
来源：http://hz.andypj.xyz/gtpcvqvapc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtuhdrulub.html

[R10] 正则匹配
来源：http://hz.snrcjt.cn/gtfptcrkah.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.andypj.xyz/gtcdjwlegm.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtkhbszbsv.html

case "$1" in
来源：http://hz.yj20258888.top/gtbyiciisj.html

start) echo "启动" ;;
来源：http://hz.yj202588.top/gtkgbokkzy.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtkccdhygr.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gtntbopwih.html

esac
来源：http://hz.pengpengdd.cyou/gtqwmzywho.html

[R12] for 遍历文件
来源：http://hz.shzxlz.cn/gtfohoqmhx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.andypj.xyz/gtjafrnwsg.html

[R13] for 计数循环
来源：http://hz.yongpay.top/gtuvyriuto.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fengsongda.top/gtyegghdes.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gtmnhhjklx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtbwgnsjov.html

[R15] while 逐行读文件
来源：http://hz.guowangkeji.top/gtpnjajdig.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.andypj.xyz/gtrrkkdvjh.html

[R16] until 等待条件
来源：http://hz.hammf.cn/gtdekmroyi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtkarvtmes.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtrtcnnscx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nanxinkj.top/gtbkvrwefg.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtnvyiktnz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtjaarohmy.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtjhcvfcgf.html

echo "${#arr[@]}"
来源：http://hz.jyoumei.cn/gtlvsdijrq.html

[R20] 关联数组（字典）
来源：http://hz.meibo888.top/gtoutzemnf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtrizvnidm.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtijljcniy.html

echo "${#s}"
来源：http://hz.hywenlv.cn/gtjyhrglbw.html

[R22] 截取子串
来源：http://hz.yueranfly.top/gtukokkqhk.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtxqlbbffl.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gtyxiqdpgp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhixingplan.top/gtxmsnhbdi.html

[R24] 大小写转换
来源：http://hz.ydzc1.top/gtywuvmomi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydjk.org.cn/gtnkwkktll.html

[R25] 去后缀 / 去前缀
来源：http://hz.pycfn.com/gtlhpsqvdc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cqqwz.cn/gterckygao.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtvbpjlhmp.html

now=$(date +%F); echo "$now"
来源：http://hz.ybcxt.top/gtpoacxpie.html

[R27] 算术展开
来源：http://hz.jinqigfzy.top/gtrlpbvewb.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtlekxsgzg.html

[R28] 浮点运算
来源：http://hz.iojbl.cn/gtbtugcspx.html

echo "scale=2; 10/3" | bc
来源：http://hz.pycfn.com/gtbqopomxx.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtnygeonxa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtbyonibky.html

[R30] 函数返回状态码
来源：http://hz.jqgfzy.top/gtqpmhscjc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtmvlfwvuu.html

[R31] 局部变量
来源：http://hz.sysykeji.top/gtvugwtfqw.html

f() { local x=1; echo "$x"; }
来源：http://hz.meibo888.top/gtemthsnyb.html

[R32] 参数个数校验
来源：http://hz.ppjwa.cn/gtphlftttx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gtlhhbxjti.html

[R33] 捕获错误并提示行号
来源：http://hz.yuanzhike.top/gtvexoumiu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gtlftcgvpj.html

[R34] 退出时清理
来源：http://hz.nanxinkj.top/gtwggjbjep.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtrjqlwfhb.html

[R35] 后台执行并等待
来源：http://hz.daxiang520.top/gtihccsebz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtuhmylptj.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtpyycnwik.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.wangshuangyany.cn/gtdzwlttyf.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gtseozmvka.html

files=$(ls -1)
来源：http://hz.feifeiyinyue.top/gtesunwdaa.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtdzdcqkfu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtyenddseo.html

[R39] 重定向标准输出与错误
来源：http://hz.yvedp.cn/gtbymbwkgn.html


<!-- 参考信息 -->