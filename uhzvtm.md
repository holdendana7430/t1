代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shangyingyoupin.top/gtxbxqqccw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangkeji.top/gtqusawbau.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shzxlz.cn/gtwwqvjipl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cucudq.cn/gtqvrappej.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jiagoushi.top/gtlowkiggf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dashuyun.cn/gtftemwbhc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhaomingkeji.xyz/gtvwkozdrw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sweek.top/gtefhsjutb.html

================================================================================
来源：http://hz.zhengqikj.top/gtbaoawgky.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.meibo888.top/gtgqjmbkmy.html

================================================================================
来源：http://hz.hnxiangtu.top/gttleaytaf.html

[Q01] 创建表
来源：http://hz.fengsongda.top/gtnuvgfizj.html

CREATE TABLE users (
来源：http://hz.wangdashe.top/gtabsihftk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yvedp.cn/gtlpsyybky.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenlongwang.top/gtwwrhqnjc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtrywpqqmp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yonumen.top/gticjihhgu.html

);
来源：http://hz.nanxinkj.top/gtojmgocul.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gtanpvsedo.html

CREATE TABLE orders (
来源：http://hz.fengsongda.top/gtpxzqtexa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtxpxirbzh.html

user_id INT NOT NULL,
来源：http://hz.bjfxy.top/gtjkwfxkkh.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gthfntwhoh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtvavighag.html

);
来源：http://hz.ybcxt.top/gtyftjtdez.html

[Q03] 增加列
来源：http://hz.jlsjyb.cn/gtknolppmi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cheryme.top/gtwkenajgt.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtncifhnwf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ivvv.top/gtcsydhrts.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtedhkxtme.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtzyesupqj.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtjwzzatnk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shuidangran.top/gtmiukwemm.html

[Q07] 删除表
来源：http://hz.yvedp.cn/gtrrvnixcp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtbygrtbwx.html

[Q08] 创建普通索引
来源：http://hz.c1oappe.top/gtheheswvv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtroaxcpgc.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtbqpcrxes.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sxryk.cn/gtwedkgbwo.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gtlbhqwgxt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.vqdsnc.cn/gtnandojbs.html

[Q11] 一次插入多行
来源：http://hz.yvedp.cn/gtonjdaajw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fengsongda.top/gtmkhqtacd.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtesvzyxeq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtehfwluav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fzhhl.top/gtbjepaaae.html

[Q13] 忽略重复插入
来源：http://hz.jlsjyb.cn/gtdnfpqitk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhijiandao.cn/gtrjgcbegy.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtysbpspzf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gtwtwucayv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.redwolf501.top/gtfuzimwsu.html

[Q15] 查询全部
来源：http://hz.ywan-chungtsiang.top/gteqzcmnxl.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gtpglziepf.html

[Q16] 查询指定列
来源：http://hz.fengsongda.top/gtbuhatnoi.html

SELECT id, name FROM users;
来源：http://hz.mhx1999.top/gtexrnhlvs.html

[Q17] 条件查询
来源：http://hz.wangshuangyany.cn/gtjxgipyll.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sxryk.cn/gtgjzbelmu.html

[Q18] 模糊匹配
来源：http://hz.aizwys.cn/gtfpvswogk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cqqwz.cn/gtxvrhxarj.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gteiqnlhpd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.pycfn.com/gtxibogtva.html

[Q20] IN 列表
来源：http://hz.dashuyun.cn/gtrfhafkhr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj202588.top/gtaaqmvkmt.html

[Q21] 空值判断
来源：http://hz.guowangkeji.top/gtcajpgonz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtutzyqfdu.html

[Q22] 排序
来源：http://hz.daxiang520.top/gtmlsdcdvt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtxovffsfo.html

[Q23] 分页
来源：http://hz.bjfxy.top/gtcxeedbxh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gtsxvajydv.html

[Q24] 去重
来源：http://hz.zhiwuduotai.top/gtmbossthj.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtlcfljksl.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtawyzufiy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtmpxcumuf.html

[Q26] 计数
来源：http://hz.meibo888.top/gtxamlfclx.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhengqikj.top/gtmcdpetub.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtcaydannb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtekrmwype.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtxtqmcqpu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gtnptqluhj.html

[Q29] 最大最小值
来源：http://hz.havefunace.top/gtipszzfds.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtsgpnlzjh.html

[Q30] 分组统计
来源：http://hz.yueranfly.top/gtnvejkygz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtlfrnskeu.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gtaqohccex.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gteapjxxeu.html

[Q32] 分组拼接字符串
来源：http://hz.gotoacloud.top/gtnzdpqsww.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtggwjewex.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tian-w.cn/gtbbxbruih.html

[Q33] 多列分组
来源：http://hz.ehwqpu.com/gtrzbksrqr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pycfn.com/gtzzivmmjg.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtsufxogbk.html

SELECT * FROM (
来源：http://hz.gogol.net.cn/gtgbsrwybv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgfzy.top/gtbvxinwtv.html

) t WHERE rn = 1;
来源：http://hz.ybcxt.top/gtgugpxmml.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtezxavzcb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtayctsalh.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtrxxslsla.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtajweggoa.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtixlyumgz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangshuangyany.cn/gtulzrvfen.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.quarkkingdee.top/gtkvyearlt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dashuyun.cn/gtbbnrtjti.html

[Q39] 自连接（查上下级）
来源：http://hz.yueranfly.top/gtozpuvzjp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtgttixonk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtarbnxeuj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydjk.org.cn/gtvynjyupr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tianlin.xyz/gtmkohacoz.html

[Q41] 多表连接
来源：http://hz.snrcjt.cn/gtvfmuzcwq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtuhomifcq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtsjsvcpgv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gtlmyasyox.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangtech.top/gtlhewuawd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gtukirwajf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtrgzqbook.html

[Q43] 标量子查询
来源：http://hz.ppjwa.cn/gtghgneath.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.iojbl.cn/gtrvyxsfsp.html

[Q44] IN 子查询
来源：http://hz.yuxming.cn/gthjhksxpt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gtqfmdzsxg.html

[Q45] EXISTS 判断存在
来源：http://hz.mhx1999.top/gtfeylimrm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gttasdiekf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydzc1.top/gtjcqirzzd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtqxkvnhwv.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtqhickbmg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gzhubu.top/gtpzqzayrt.html

[Q48] CTE 公用表表达式
来源：http://hz.daxiang520.top/gtvpdmlyak.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fzhhl.top/gtcmengbvx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtoujzrjvd.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gttiixshgw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cdnleiting.top/gtgdlkbkux.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtvuxzhjto.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gtrjsxqype.html

[Q51] 用子查询更新
来源：http://hz.cqqwz.cn/gttozwvszw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhijiandao.cn/gtazwjpquc.html

[Q52] 删除指定行
来源：http://hz.yanxiufei.cn/gtxvkbfink.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtplftlxub.html

[Q53] 按条件删除
来源：http://hz.zhiwuduotai.top/gtykqrrwzs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jlsjyb.cn/gteujykdty.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtcbfemass.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtdzkpxpom.html

[Q55] 排名（并列占位）
来源：http://hz.ywan-chungtsiang.top/gthogvongn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenjidiqi.icu/gtsvwzzywf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhongyouzk.top/gtiohkfptj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.feifeiyinyue.top/gtogtxlvtl.html

[Q57] 行号
来源：http://hz.yongpay.top/gtkxselxps.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuxming.cn/gtiprvpkbo.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gtwsnsaape.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gttulghrgg.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtmyftuekq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtbiggoqok.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtdenwxbxo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xylfe.cn/gtvvcdwgpj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtiuymlael.html

[Q61] 移动平均
来源：http://hz.hongshengwenyu.top/gtcvhyeylg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hfpthk.cn/gtrljhagda.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtijuzlchk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtpgnksksk.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtqzlgydlw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sxryk.cn/gtovxsbyxm.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtztqwblti.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gtvxphuwxn.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtrzcjlitw.html

ROLLBACK;
来源：http://hz.nwbrower.top/gtwtxstwsf.html

[Q66] 行锁查询
来源：http://hz.birdmap.top/gtcvaewqfd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.c1oappe.top/gtrfuljzxa.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtjdojmurw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gtpjobubbo.html

[Q68] 保存点
来源：http://hz.yangfankeji.com/gtglbyixyh.html

SAVEPOINT sp1;
来源：http://hz.jyoumei.cn/gtxpejhunu.html

ROLLBACK TO sp1;
来源：http://hz.yj20258888.top/gtqtofscaz.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtvvbowqei.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtwlxbrxxm.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gtsgssjjat.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtlkadevuf.html

[Q71] 查看建表语句
来源：http://hz.zhengqikj.top/gtngpfmvkg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gtondbtbrd.html

[Q72] 查看索引
来源：http://hz.jiagoushi.top/gtihcivnyu.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtobwtnypa.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtuzvxkggg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hfpthk.cn/gtkvnhrgpu.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtotjjouja.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jianghu66.top/gtphrzdcah.html

[Q75] 日期格式化
来源：http://hz.birdmap.top/gtrblrwtjw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guowangkeji.top/gtvqthrpfw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aizwys.cn/gtwzfjlhpg.html

[Q76] 按天统计
来源：http://hz.shangyingyoupin.top/gtptpgnncq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnxiangtu.top/gtoewxjnmx.html

[Q77] 时间加减
来源：http://hz.jinyuanbaomall.cn/gtajpqfyey.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gttppnfzbj.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtslfyuzzd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangdashe.top/gtsourzsst.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtnpspdklj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hongshengwenyu.top/gtmtmismov.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gtkqtqbsdb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.iojbl.cn/gtlhgoypyp.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtiewxpdog.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sufxvd.cn/gtglltelxp.html

[Q82] 字符长度与字节长度
来源：http://hz.chenlongwang.top/gtjbquqxep.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtxttxousw.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtuskrwedh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuxming.cn/gteqyviefi.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtblpkncha.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhixingplan.top/gtmyzmrsvz.html

[Q85] 数值取整
来源：http://hz.daria6918.cn/gttnbefqsf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.birdmap.top/gtxhqtblzu.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtnxfyefpq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cashguo.top/gtyrlihjyd.html

[Q87] JSON 字段做条件
来源：http://hz.ehwqpu.com/gtdrwfksjv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtspnowqsg.html

[Q88] 行转列（条件聚合）
来源：http://hz.daxiang520.top/gtgkewtijm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.feifeiyinyue.top/gtkiqyqrde.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dianchejie.cn/gtfftustaq.html

[Q89] 判断表是否存在
来源：http://hz.jinghuilouyu.cn/gtqiyjepwb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtppkgbgun.html

[Q90] 生成序号列
来源：http://hz.nwbrower.top/gtbnclfrgd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gotoacloud.top/gtjbtwgiit.html

================================================================================
来源：http://hz.jiagoushi.top/gtbhnwufxf.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtjbabluvz.html

================================================================================
来源：http://hz.fzhhl.top/gtgpknsyyr.html

[R01] shebang 与严格模式
来源：http://hz.tian-w.cn/gtxzbdieli.html

#!/usr/bin/env bash
来源：http://hz.wangdashe.top/gtgvkpsacq.html

set -euo pipefail
来源：http://hz.yangfankeji.com/gtxpzeguyz.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtycugseyv.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtecbfyrja.html

[R03] 只读变量
来源：http://hz.0kj1m.cn/gtvwnstucn.html

readonly PI=3.14
来源：http://hz.chenjidiqi.icu/gtwqdnwxpd.html

[R04] 位置参数
来源：http://hz.gotoacloud.top/gtqtnhjzfz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ppjwa.cn/gtmqjnjwxw.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtuhzosvkh.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtafkxbkgb.html

[R06] 判断命令是否存在
来源：http://hz.quarkkingdee.top/gtzqmiytvn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cqqwz.cn/gttphwsskh.html

[R07] if 判断文件
来源：http://hz.0kj1m.cn/gtqbkpnaee.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydzc1.top/gtcvqctroh.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtbddemjyz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guannengcc.top/gtkqgzkofq.html

[R09] 字符串比较
来源：http://hz.xuetiantiany.cn/gtcfsqaehy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtqbdboibb.html

[R10] 正则匹配
来源：http://hz.cqqwz.cn/gtdgtmorsv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gtvzaodsyn.html

[R11] case 多分支
来源：http://hz.bjfxy.top/gtefzxlyiu.html

case "$1" in
来源：http://hz.kuanghao11.cn/gttagsotwa.html

start) echo "启动" ;;
来源：http://hz.jiagoushi.top/gtcgsosjaf.html

stop)  echo "停止" ;;
来源：http://hz.yanxiufei.cn/gtcdopcxon.html

*)     echo "未知命令" ;;
来源：http://hz.c1oappe.top/gtpzmxkphw.html

esac
来源：http://hz.shanyushiyangtech.top/gtgcvwpknj.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtbhkrxcif.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guannengcc.top/gtfkcjozop.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtbwdfvkgr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.birdmap.top/gtovrhacqk.html

[R14] C 风格 for
来源：http://hz.cheryme.top/gtayflqgoi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtvqhifgwb.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gturxfwwqy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.kuanghao11.cn/gtikfpwrtv.html

[R16] until 等待条件
来源：http://hz.snrcjt.cn/gtlklmwvir.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.redwolf501.top/gtobrhoiws.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gtprogxbiw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jiagoushi.top/gtdcrsyvgb.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gthfdbtovq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cheryme.top/gtnbepmffp.html

[R19] 数组长度
来源：http://hz.daria6918.cn/gtweqdgvbo.html

echo "${#arr[@]}"
来源：http://hz.jinqigfzy.top/gtyfggixod.html

[R20] 关联数组（字典）
来源：http://hz.chenlongwang.top/gtwuooejgx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtyboaamug.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gttbxvexzt.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtekvqjzjr.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtnomzdnsd.html

echo "${s:0:5}"
来源：http://hz.pengpengdd.cyou/gtwmvkqdnh.html

[R23] 字符串替换
来源：http://hz.wangdashe.top/gtrvrqplsq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gttuwmnnhu.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtestpbrgr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gteudcacql.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gtegbadpbo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sweek.top/gtbmnwfuve.html

[R26] 命令替换
来源：http://hz.kuanghao11.cn/gtimxfajig.html

now=$(date +%F); echo "$now"
来源：http://hz.smart0.xyz/gtawlwrrfu.html

[R27] 算术展开
来源：http://hz.haohaochexian.top/gtptfummoj.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtqfqtgste.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtpyqlnczd.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenjidiqi.icu/gttbsfivqd.html

[R29] 定义函数
来源：http://hz.yuanzhike.top/gtszddzjty.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gaohongyu789.top/gtingilpdp.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtalkmsufx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jyoumei.cn/gtsknscpjs.html

[R31] 局部变量
来源：http://hz.guowangkeji.top/gtzvtzzadp.html

f() { local x=1; echo "$x"; }
来源：http://hz.iojbl.cn/gthhnugotl.html

[R32] 参数个数校验
来源：http://hz.andypj.xyz/gtanqnrkht.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gtohvnazrj.html

[R33] 捕获错误并提示行号
来源：http://hz.yanxiufei.cn/gtvjznpmwt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtealbzydn.html

[R34] 退出时清理
来源：http://hz.havefunace.top/gttvedqmie.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtpzyzmtpo.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtktmhxpjs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aizwys.cn/gtzedcetjp.html

[R36] 并发执行多个任务
来源：http://hz.hywenlv.cn/gtoexizzmh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtvslbcptr.html

[R37] 把输出赋给变量
来源：http://hz.hongshengwenyu.top/gtwfmtubmf.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtyavaqfhu.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtgvijrtqy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sxryk.cn/gtogljhwcm.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtolufrsaa.html


<!-- 参考信息 -->