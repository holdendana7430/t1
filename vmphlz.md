代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258888.top/gtujtfiiwp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtpjvcdtcd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.haohaochexian.top/gtbjmnymii.html

[P08] 处理浮点精度问题
来源：http://hz.svipenyu.cn/gtbayjhvge.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tianlin.xyz/gtgllutwzm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.52xcode.cn/gtqngussue.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtphzuglxx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ehwqpu.com/gthvtmezze.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.aizwys.cn/gtkvjlsnxh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgufenzy.top/gtggdmywtk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ppjwa.cn/gtdafyxjxu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ivvv.top/gthmhqggbp.html

================================================================================
来源：http://hz.shzxlz.cn/gtznpqtwwg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yonumen.top/gtvyxezgbj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjaocgezx.html

[Q01] 创建表
来源：http://hz.xinyue.icu/gtqoqmwqgh.html

CREATE TABLE users (
来源：http://hz.zhixingplan.top/gtfsssisvl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtvilibcho.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gzhubu.top/gtjwcavumi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xziqi.cn/gtkjoycjro.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hywenlv.cn/gtcucrrjhw.html

);
来源：http://hz.yangfankeji.com/gtmwofyuln.html

[Q02] 创建带外键的表
来源：http://hz.kuanghao11.cn/gtlccjgkqo.html

CREATE TABLE orders (
来源：http://hz.yj20258.top/gtxwtqtjov.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtpayaabsd.html

user_id INT NOT NULL,
来源：http://hz.hnxiangtu.top/gtfidayybe.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtlqajwmii.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gtiszpvdpc.html

);
来源：http://hz.hysaishi.cn/gtbqsrtend.html

[Q03] 增加列
来源：http://hz.yuxming.cn/gtngycguzi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtcggexaqo.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gttrkfsyyi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shuidangran.top/gtzirtdgpj.html

[Q05] 重命名列
来源：http://hz.quarkkingdee.top/gtqyqzinwt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtfukasduv.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtsvnxmtrt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yongpay.top/gtmyqcrgdu.html

[Q07] 删除表
来源：http://hz.yvedp.cn/gtuxvqrzuy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtplwbjgym.html

[Q08] 创建普通索引
来源：http://hz.vqdsnc.cn/gtmwdrcjeg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtnwrsdqmh.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangtech.top/gtodgrbviw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtlirpevrq.html

[Q10] 插入单行
来源：http://hz.dashuyun.cn/gtemqiluel.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtdmzlvubo.html

[Q11] 一次插入多行
来源：http://hz.wangshuangyany.cn/gtirkxarka.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cashguo.top/gtcafqlygj.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258.top/gtnjfpcmtp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.kuanghao11.cn/gtzdkaiuxq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aizwys.cn/gtwsjoqyta.html

[Q13] 忽略重复插入
来源：http://hz.nanxinkj.top/gtjghrelzk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.9152youxi.cn/gtvyeievsc.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtjjqqaomt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangkeji.top/gtyngrntss.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xingfuxueyuan.xyz/gtludybovn.html

[Q15] 查询全部
来源：http://hz.ybcxt.top/gtesboaiga.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtqtbmgxae.html

[Q16] 查询指定列
来源：http://hz.ehwqpu.com/gtjcecggdk.html

SELECT id, name FROM users;
来源：http://hz.iojbl.cn/gtiwapzmlv.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtwxcjjtre.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtcshvvzlk.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gtanpwrhfn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtwclhxjgt.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtxmszdhaw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yongpay.top/gtwiqzvgij.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtbsqivjbm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gttpcctlyj.html

[Q21] 空值判断
来源：http://hz.bjfxy.top/gtffnmmvql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gtyrjxyofy.html

[Q22] 排序
来源：http://hz.wangdashe.top/gtmqauikzm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhixingplan.top/gtmzkhudyg.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gttejvgnsf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dianchejie.cn/gthgniudck.html

[Q24] 去重
来源：http://hz.gogol.net.cn/gtdfgkeyth.html

SELECT DISTINCT city FROM users;
来源：http://hz.sufxvd.cn/gtzonekxkr.html

[Q25] 只取前 N 条
来源：http://hz.mhx1999.top/gtbrsfhlus.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtodnhbygm.html

[Q26] 计数
来源：http://hz.mhx1999.top/gtwtrwqfxo.html

SELECT COUNT(*) FROM users;
来源：http://hz.jianghu66.top/gtjkzspfhg.html

[Q27] 条件计数
来源：http://hz.hfpthk.cn/gtwfcowqzy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtjoxdipnd.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtujbewrzw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gthftbhpli.html

[Q29] 最大最小值
来源：http://hz.ivvv.top/gtepeynjfp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.316326.xyz/gtayhobqqk.html

[Q30] 分组统计
来源：http://hz.9152youxi.cn/gtdyyihopc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtscrvbqxe.html

[Q31] 分组后过滤
来源：http://hz.sweek.top/gtmncxkudf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtffexmkfs.html

[Q32] 分组拼接字符串
来源：http://hz.jiagoushi.top/gtgrgpwesn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtselbxcvi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtmvcxmvnt.html

[Q33] 多列分组
来源：http://hz.tian-w.cn/gtsxbwnxqk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtlwksjcdo.html

[Q34] 每组取第一条
来源：http://hz.svipenyu.cn/gtgffujlvw.html

SELECT * FROM (
来源：http://hz.yueranfly.top/gtuwbdkwxy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtncpcjxei.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtdlelmoqx.html

[Q35] 内连接
来源：http://hz.bjfxy.top/gthvrvnuyx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtjbwytcnl.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtwavhuhpf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtpvmpxfjk.html

[Q37] 右连接
来源：http://hz.jinqigfzy.top/gtjpsjxybf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gotoacloud.top/gtjjnkrbvi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.0kj1m.cn/gtaeslwrdw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ivvv.top/gtleidlvlj.html

[Q39] 自连接（查上下级）
来源：http://hz.redwolf501.top/gtrogacnnf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.snrcjt.cn/gtaoykawbp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenjidiqi.icu/gtdyownczv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtvvjlxaoh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtgjxrpguh.html

[Q41] 多表连接
来源：http://hz.daxiang520.top/gtarcfirnw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtdrbxqbuf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fzhhl.top/gthydhwvcs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jianghu66.top/gtjsczkxpc.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtvbaixyyr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtjegnbxzb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dashuyun.cn/gtvmbecrlr.html

[Q43] 标量子查询
来源：http://hz.cqqwz.cn/gtmsitcezz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtckzvxvnj.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtmkpqykoz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj20258.top/gtnckzkzex.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtbqpprdnz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtiyywebyj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gteaujkqtj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gttezuegmu.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtmkwxpwdu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aibaodan.cn/gtnmjmxghn.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtgbhtlcob.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.feifeiyinyue.top/gtphymjnvb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtmsjbkqny.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtscwpbhoq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtizdquppx.html

[Q50] 批量更新
来源：http://hz.feifeiyinyue.top/gtrhnwqsaj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangtech.top/gtmacvoqtr.html

[Q51] 用子查询更新
来源：http://hz.ydzc1.top/gtvaipblmp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ivvv.top/gtdzexsrdw.html

[Q52] 删除指定行
来源：http://hz.yanxiufei.cn/gtwleouaar.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtmrjgrsok.html

[Q53] 按条件删除
来源：http://hz.yj20258888.top/gtjcnkrjnu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gthbmuouiw.html

[Q54] 清空表
来源：http://hz.cqqwz.cn/gtwjuzkdee.html

TRUNCATE TABLE logs;
来源：http://hz.aibaodan.cn/gtuzvbhqwy.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtpojdcfdu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtmspiicjx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.smart0.xyz/gtuxlferjs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cqqwz.cn/gtikskpeqk.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtuakcmcfb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.snrcjt.cn/gtshzidzqp.html

[Q58] 累计求和
来源：http://hz.zycfv.cn/gtoneisgwx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhaomingkeji.xyz/gticejswqq.html

[Q59] 分组内累计
来源：http://hz.shzxlz.cn/gtahbggqwb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gttpzfaaic.html

[Q60] 取上一行 / 下一行
来源：http://hz.quarkkingdee.top/gtvlqfghwm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zdqjudy.top/gtjgsvmtrk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258.top/gtflhcgvkf.html

[Q61] 移动平均
来源：http://hz.shuidangran.top/gtxprhxqcz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gtudqcmize.html

[Q62] 分组占比
来源：http://hz.0kj1m.cn/gtvfiigkby.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtnsbffclx.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtusbbtwif.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtqxabwzlr.html

[Q64] 提交事务
来源：http://hz.andypj.xyz/gtkrbjdunl.html

COMMIT;
来源：http://hz.jqgfzy.top/gtrifzlban.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtumvsjhml.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtioxfkrcf.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtpmiuzree.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zycfv.cn/gtooplqfcp.html

[Q67] 设置隔离级别
来源：http://hz.snrcjt.cn/gtuvfaidel.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yongpay.top/gtsvcbqkte.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtwwxcflnn.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gtgmxjkovs.html

ROLLBACK TO sp1;
来源：http://hz.zhijiandao.cn/gtmjifklal.html

[Q69] 查看执行计划
来源：http://hz.52xcode.cn/gtnrxtvtkr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sxryk.cn/gtdpnkorob.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtuofqfiun.html

ANALYZE TABLE users;
来源：http://hz.hammf.cn/gtvfsyawpn.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gtyrkkcvwh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yvedp.cn/gtuufwbqmv.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtiftppvfe.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gtklbslmat.html

[Q73] 查看表状态
来源：http://hz.cdnleiting.top/gtnoneufrq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jlsjyb.cn/gtbcsfghej.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtncdwnrea.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtskqiusnm.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gtvfzvcntw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtkkhivcfz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtdeppnbgy.html

[Q76] 按天统计
来源：http://hz.shanyushiyangtech.top/gtwwqqrxwr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.feifeiyinyue.top/gtquexhilc.html

[Q77] 时间加减
来源：http://hz.hysaishi.cn/gtafqrdoir.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtiifequzq.html

[Q78] 当前时间
来源：http://hz.pengpengdd.cyou/gtnldepnja.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtsixvuvyo.html

[Q79] 字符串拼接
来源：http://hz.hysaishi.cn/gtvcgddlpp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gtnnphkhcp.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gthhiqdfxo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guannengcc.top/gtuewywdfo.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtaohnhkvs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sweek.top/gtwxtgykjg.html

[Q82] 字符长度与字节长度
来源：http://hz.fzhhl.top/gtrqrmtznm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtufzrjwrc.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtbtgxgpuz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jianghu66.top/gtjdralnrr.html

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gtdtboiorn.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtlljjervj.html

[Q85] 数值取整
来源：http://hz.jinqigufen.top/gtdmcwwdpc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.meibo888.top/gtfimikpqw.html

[Q86] 读取 JSON 字段
来源：http://hz.daxiang520.top/gtjsqbdduy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xinyue.icu/gtzzeyjrwx.html

[Q87] JSON 字段做条件
来源：http://hz.xziqi.cn/gtsydkqtzs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ppjwa.cn/gtegsyzalu.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtsovnhruo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xuanzx.com/gthquwxkns.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtvvdyiczi.html

[Q89] 判断表是否存在
来源：http://hz.gotoacloud.top/gtnwbgymuk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtpkueywpj.html

[Q90] 生成序号列
来源：http://hz.hywenlv.cn/gtpddkinxm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.svipenyu.cn/gtbhlqwvpg.html

================================================================================
来源：http://hz.ppjwa.cn/gtbkkacjnn.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtyxrqjjie.html

================================================================================
来源：http://hz.aibaodan.cn/gtyujzncia.html

[R01] shebang 与严格模式
来源：http://hz.ppjwa.cn/gtqqsehehl.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gtuvznmbbz.html

set -euo pipefail
来源：http://hz.hnqzz.top/gtxwyjkirs.html

[R02] 变量赋值与使用
来源：http://hz.hnxiangtu.top/gtdltpggds.html

name="Tom"; echo "$name"
来源：http://hz.bjfxy.top/gtanqebovx.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtiyxuwbkt.html

readonly PI=3.14
来源：http://hz.yj20258.top/gtpmosxley.html

[R04] 位置参数
来源：http://hz.aibaodan.cn/gtivgmjskc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtnwtwmwxt.html

[R05] 参数默认值
来源：http://hz.sysykeji.top/gtptlgnqkg.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtnngerpzt.html

[R06] 判断命令是否存在
来源：http://hz.cucudq.cn/gtoqkiqipd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gtjjmeqeeo.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtiwtrnwhd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtsoiheloc.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gtfaeyvhnq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigfzy.top/gtaimkqyrs.html

[R09] 字符串比较
来源：http://hz.gogol.net.cn/gtfhahzxdg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ywan-chungtsiang.top/gtxnanxnmf.html

[R10] 正则匹配
来源：http://hz.316326.xyz/gtekbccbmi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gthbjkqezq.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtmgvaxngy.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gtxdxzhmmf.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtruqkcrio.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtopusqhub.html

*)     echo "未知命令" ;;
来源：http://hz.fzhhl.top/gtjlsyhwsk.html

esac
来源：http://hz.hammf.cn/gtssfjxoph.html

[R12] for 遍历文件
来源：http://hz.hywenlv.cn/gtcbyissxs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtojzitnbi.html

[R13] for 计数循环
来源：http://hz.yvedp.cn/gtevrnhlet.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenlongwang.top/gtzrqcxmud.html

[R14] C 风格 for
来源：http://hz.tanke756.top/gtjuaxrdaj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.snrcjt.cn/gtnnnnvamk.html

[R15] while 逐行读文件
来源：http://hz.316326.xyz/gtnqookqbm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hammf.cn/gtzsqqlrfs.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtndvhaowi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.smart0.xyz/gtvfvjalcr.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gtvxvdxknx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yanxiufei.cn/gtqocgyppm.html

[R18] 遍历数组
来源：http://hz.sufxvd.cn/gtyqmvdreh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinyuanbaomall.cn/gtdzaytxje.html

[R19] 数组长度
来源：http://hz.bjfxy.top/gtmzxdomdq.html

echo "${#arr[@]}"
来源：http://hz.gzhubu.top/gtmrstdtov.html

[R20] 关联数组（字典）
来源：http://hz.shangyingyoupin.top/gtntuglmiv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jlsjyb.cn/gtjmclwcrb.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gttonyzihu.html

echo "${#s}"
来源：http://hz.cqqwz.cn/gtgtizmyef.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtuqfhxylg.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtboprgvnz.html

[R23] 字符串替换
来源：http://hz.hywenlv.cn/gtdpzdmfrp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guowangkeji.top/gtqkcvanvc.html

[R24] 大小写转换
来源：http://hz.shangyingyoupin.top/gtjvrozclj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.quarkkingdee.top/gttlohldoy.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtduerekjl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tian-w.cn/gtoetpfnvg.html

[R26] 命令替换
来源：http://hz.sweek.top/gtigbfchuv.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgfzy.top/gtehbmmezd.html

[R27] 算术展开
来源：http://hz.cqqwz.cn/gtuyovyyjf.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtmaobhfyf.html

[R28] 浮点运算
来源：http://hz.tian-w.cn/gthfwatoxn.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtcskywkvu.html

[R29] 定义函数
来源：http://hz.shuidangran.top/gtpoomxdwt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydjk.org.cn/gtflzafrbs.html

[R30] 函数返回状态码
来源：http://hz.zhaomingkeji.xyz/gtandpmajs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ywan-chungtsiang.top/gtlnvjfqsg.html

[R31] 局部变量
来源：http://hz.52xcode.cn/gtntracpzb.html

f() { local x=1; echo "$x"; }
来源：http://hz.hongshengwenyu.top/gtmohbabrc.html

[R32] 参数个数校验
来源：http://hz.tian-w.cn/gtyloxmdhe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yanxiufei.cn/gtbqwphipq.html

[R33] 捕获错误并提示行号
来源：http://hz.aizwys.cn/gtldfhdvnj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.316326.xyz/gtjdtlzmhq.html

[R34] 退出时清理
来源：http://hz.vqdsnc.cn/gtljbrhefz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtjqodzoay.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtrbyicytw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.316326.xyz/gtsdlfpffa.html

[R36] 并发执行多个任务
来源：http://hz.kuanghao11.cn/gtxlxtnpip.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtbzakxszj.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtwreoiiwb.html


<!-- 参考信息 -->