代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sxryk.cn/gtyqvgmoym.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xingfuxueyuan.xyz/gtluasdsrp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gtqgzomvte.html

[P08] 处理浮点精度问题
来源：http://hz.hysaishi.cn/gthxrfwhix.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aizwys.cn/gtalvwtzvb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gtcttmwwji.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shzxlz.cn/gtmbdktsji.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gtcdabachf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtpncsqypq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fzhhl.top/gtkdkwqafb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtlpovnciv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gteuyueuzp.html

================================================================================
来源：http://hz.gogol.net.cn/gtyyhjjilj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gtkednggay.html

================================================================================
来源：http://hz.cheryme.top/gtjbfeflad.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gtzjljzevx.html

CREATE TABLE users (
来源：http://hz.ehwqpu.com/gtcdvuzjoy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtenryhkde.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dashuyun.cn/gtjuipaiol.html

email VARCHAR(100) UNIQUE,
来源：http://hz.c1oappe.top/gtsagvtfxv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gzhubu.top/gtitahliis.html

);
来源：http://hz.chenzaomai.com/gticcvgtmv.html

[Q02] 创建带外键的表
来源：http://hz.feifeiyinyue.top/gtwzvfdnlc.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtdgrttzew.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtuoxcivma.html

user_id INT NOT NULL,
来源：http://hz.cucudq.cn/gtpiorzgoe.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtgtmbqmca.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gtrtshiloq.html

);
来源：http://hz.jlsjyb.cn/gtzfeknunf.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gtrbpbxbvc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnxiangtu.top/gtpjwidxuq.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gtxuhtijfu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtrhdfdcyl.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gtghoaizag.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.mhx1999.top/gtzowmaeru.html

[Q06] 删除列
来源：http://hz.yuxming.cn/gtwqbnsuvu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenlongwang.top/gtliueazca.html

[Q07] 删除表
来源：http://hz.sxryk.cn/gtkoybfsse.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnqzz.top/gtyliaduyo.html

[Q08] 创建普通索引
来源：http://hz.daria6918.cn/gtsoldckoz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtebkurwxm.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtgrzqcogt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtupqyrsje.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gtlxpcyuoc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yonumen.top/gtwwigjogq.html

[Q11] 一次插入多行
来源：http://hz.xinyue.icu/gtbleqzgzc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtcjbqxsod.html

[Q12] 插入后取自增 ID
来源：http://hz.guowangkeji.top/gtfqrmpdvd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigfzy.top/gtugiundte.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtcpxvmikw.html

[Q13] 忽略重复插入
来源：http://hz.zhaomingkeji.xyz/gtshheffkf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gtdormpwmf.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhengqikj.top/gttbckoupx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gtgvmbgmhz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gogol.net.cn/gtoneofiyp.html

[Q15] 查询全部
来源：http://hz.yongpay.top/gtlbaoexac.html

SELECT * FROM users;
来源：http://hz.jinyuanbaomall.cn/gtskjwsndi.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtmnnolxfg.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtthcpfaye.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtthurplef.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gtslmxmgme.html

[Q18] 模糊匹配
来源：http://hz.cqqwz.cn/gtfwcrokoc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cqqwz.cn/gtbyzrzvus.html

[Q19] 范围查询
来源：http://hz.zhiwuduotai.top/gtrglybebj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtqxwhtpup.html

[Q20] IN 列表
来源：http://hz.yj20258.top/gtndcnthht.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ppjwa.cn/gtjweauadz.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gtktnxnkmf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hywenlv.cn/gtsjuxyrbz.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtnvbmnuha.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.snrcjt.cn/gtxttffbin.html

[Q23] 分页
来源：http://hz.yj202588.top/gtoruzobch.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtrlptdoob.html

[Q24] 去重
来源：http://hz.gogol.net.cn/gtegqigyhc.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gteqpfddfn.html

[Q25] 只取前 N 条
来源：http://hz.cheryme.top/gtrkevhobl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinghuilouyu.cn/gtobmwpaaj.html

[Q26] 计数
来源：http://hz.yvedp.cn/gtzhhgnihi.html

SELECT COUNT(*) FROM users;
来源：http://hz.haohaochexian.top/gttpmqbkfg.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtlpabynkr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yonumen.top/gthxlxqccm.html

[Q28] 求和与平均
来源：http://hz.yj20258888.top/gtfyywqfrm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtzftrtylt.html

[Q29] 最大最小值
来源：http://hz.ywan-chungtsiang.top/gtpijdjrec.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daxiang520.top/gtsfvxkkqo.html

[Q30] 分组统计
来源：http://hz.zhongyouzk.top/gtewbuudon.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtfhdcqerp.html

[Q31] 分组后过滤
来源：http://hz.jlsjyb.cn/gtknsvylxa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jlsjyb.cn/gtfkcehgoo.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigufen.top/gtsbhuvvsl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtwazqdnuv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gtgtirjnsi.html

[Q33] 多列分组
来源：http://hz.yuxming.cn/gtirlguscm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gtsxtqxkqq.html

[Q34] 每组取第一条
来源：http://hz.c1oappe.top/gtvmjvejuq.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtykuhjxcb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gtlhniomfv.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtkaglcryx.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gtzgvkzkno.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtpcqoylmu.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtpyxbemlz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtlnzmcbnm.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtjpdbiczo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinqigufen.top/gtgysyefrl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hywenlv.cn/gtorhqyzol.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sysykeji.top/gtffuzzpdr.html

[Q39] 自连接（查上下级）
来源：http://hz.zhongyouzk.top/gtlprpzeiw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.9152youxi.cn/gtevpbuuon.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.birdmap.top/gtcgeodijr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gthhwhtmsq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cqqwz.cn/gtfikawjwc.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtgltbzqbg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenlongwang.top/gtfaxjeoze.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnxiangtu.top/gtjwvxedpl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fengsongda.top/gtiukxjtss.html

[Q42] 连接条件附加过滤
来源：http://hz.sxryk.cn/gtkiuwudeu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sweek.top/gtkekrgqdd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ppjwa.cn/gtvrdefexi.html

[Q43] 标量子查询
来源：http://hz.jinghuilouyu.cn/gtbybngjie.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gtsztprwgd.html

[Q44] IN 子查询
来源：http://hz.jiagoushi.top/gtcwvoawqn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxuanxn.top/gtaqopbhyb.html

[Q45] EXISTS 判断存在
来源：http://hz.ehwqpu.com/gtonivutqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xingfuxueyuan.xyz/gtzgbxiaxs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtgtdiiivh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gttfbbihzm.html

[Q47] 与平均值比较
来源：http://hz.svipenyu.cn/gtktielwrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sysykeji.top/gtjyyguasw.html

[Q48] CTE 公用表表达式
来源：http://hz.jinyuanbaomall.cn/gtaxazzoey.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxinkj.top/gtghjujpzs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gogol.net.cn/gtuqrsmhuf.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtkwnvypcc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.mhx1999.top/gtcobsfotx.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtfnxftutv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangshuangyany.cn/gtjlxqnnkr.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtbookqsud.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtqqzdmdbw.html

[Q52] 删除指定行
来源：http://hz.smart0.xyz/gteweqcyxy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtneijestf.html

[Q53] 按条件删除
来源：http://hz.shuidangran.top/gtfxfmpmri.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtdyjgkqia.html

[Q54] 清空表
来源：http://hz.tianlin.xyz/gtqgzboujz.html

TRUNCATE TABLE logs;
来源：http://hz.guowangkeji.top/gtzweupkhp.html

[Q55] 排名（并列占位）
来源：http://hz.sysykeji.top/gtzzpbdzox.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtlusqhkii.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnqzz.top/gtxsqjuzny.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jianghu66.top/gtvduxnvit.html

[Q57] 行号
来源：http://hz.jinghuilouyu.cn/gtrlgkxmuu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtcwbocbla.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtjodkqnll.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtmeuwknnu.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtihztevrn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hongshengwenyu.top/gtruidmgce.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtxxrkyknc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtzhigouxr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtnjtphazi.html

[Q61] 移动平均
来源：http://hz.aizwys.cn/gtkojvciwc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtltsjhfib.html

[Q62] 分组占比
来源：http://hz.cqqwz.cn/gtvskwaiau.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtswrccdex.html

[Q63] 开启事务
来源：http://hz.cashguo.top/gtrertiwek.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtrttohnry.html

[Q64] 提交事务
来源：http://hz.hywenlv.cn/gtmevnbwzh.html

COMMIT;
来源：http://hz.shangyingyoupin.top/gttoxfyxrs.html

[Q65] 回滚事务
来源：http://hz.mhx1999.top/gtujtreosy.html

ROLLBACK;
来源：http://hz.zhoulong.xyz/gtgcgtaqvl.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtnbdduoni.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtsgoiwymj.html

[Q67] 设置隔离级别
来源：http://hz.vqdsnc.cn/gtsoulpklu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhixingplan.top/gtgfyxtpxg.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gthksintzk.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtclunxkod.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gtvxfiuqsi.html

[Q69] 查看执行计划
来源：http://hz.zhijiandao.cn/gtftgjuipu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yueranfly.top/gtluzrwbch.html

[Q70] 更新统计信息
来源：http://hz.havefunace.top/gtnmujhitu.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtvfghcyhj.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtzfsvejlt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnqzz.top/gtgvkfkzvb.html

[Q72] 查看索引
来源：http://hz.ydjk.org.cn/gtwolanbbr.html

SHOW INDEX FROM users;
来源：http://hz.cucudq.cn/gteplbyzvc.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtikhdwqnu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pycfn.com/gtzkwgvbmy.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gterezubxn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aizwys.cn/gtbdksqyex.html

[Q75] 日期格式化
来源：http://hz.shzxlz.cn/gtzcdhsiob.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtghvhtbuz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtuxwhmdme.html

[Q76] 按天统计
来源：http://hz.yuxming.cn/gtvfyxbkbt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ehwqpu.com/gtvocnekoo.html

[Q77] 时间加减
来源：http://hz.snrcjt.cn/gttnpgavvr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtveyfuccm.html

[Q78] 当前时间
来源：http://hz.nanxuanxn.top/gtwmhfhato.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtkntaqotx.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtpmehtchw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhongyouzk.top/gtsnstwjpw.html

[Q80] 字符串截取
来源：http://hz.yueranfly.top/gtmdreribi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gtceeadhsa.html

[Q81] 字符串替换
来源：http://hz.sxryk.cn/gtyzkewbja.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinqigfzy.top/gtylsdfdco.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gtshwkvhcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258888.top/gthlkgkzpg.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtbfprpxix.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zycfv.cn/gtzbgvhcdw.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtjoclpecn.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtgbrlggjn.html

[Q85] 数值取整
来源：http://hz.dianchejie.cn/gtiexjyjvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.iojbl.cn/gtadiyhfer.html

[Q86] 读取 JSON 字段
来源：http://hz.zycfv.cn/gtxtnxdupr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shangyingyoupin.top/gtxjaeylgy.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtndtkevrd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gaohongyu789.top/gtmojxmfjz.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinyuanbaomall.cn/gtbrhisatc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hysaishi.cn/gtuudlnwxg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangkeji.top/gtjnsknvvr.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtghfspfbo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dianchejie.cn/gtxclytank.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gttfqfguap.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtnwjihisx.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcjbjqqon.html

R. Bash 专题
来源：http://hz.chenzaomai.com/gtgwtlvamw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnnwrsmal.html

[R01] shebang 与严格模式
来源：http://hz.jinyuanbaomall.cn/gtiszronkl.html

#!/usr/bin/env bash
来源：http://hz.zhixingplan.top/gtpqqoqbay.html

set -euo pipefail
来源：http://hz.dashuyun.cn/gtnnoaiqdy.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gtatijgtac.html

name="Tom"; echo "$name"
来源：http://hz.dianchejie.cn/gtxaksnivk.html

[R03] 只读变量
来源：http://hz.zhengqikj.top/gtlrjbiyuj.html

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtljgsafjv.html

[R04] 位置参数
来源：http://hz.tanke756.top/gtkrdoqspw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gthphqibub.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtimfrtdpc.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtdvvsmfdr.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtxuhmhlij.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gtxtyiiuub.html

[R07] if 判断文件
来源：http://hz.chenzaomai.com/gttesinhkd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.kuanghao11.cn/gtrtnkhuhl.html

[R08] 数值比较
来源：http://hz.zhixingplan.top/gtdupmqoxa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daxiang520.top/gtxhoikgpl.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gtsjhgwcvw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnxiangtu.top/gturufdauo.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtxgffbbgo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtczhwgcna.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gthizwyjcf.html

case "$1" in
来源：http://hz.sxryk.cn/gtvlksbiuz.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtnubkspsm.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtrllnvsnd.html

*)     echo "未知命令" ;;
来源：http://hz.0kj1m.cn/gtpjjolhqn.html

esac
来源：http://hz.gaohongyu789.top/gtldnbrooo.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtwmqnizcr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtqwtoplfb.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gtrkbuqwal.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtwxwyacvd.html

[R14] C 风格 for
来源：http://hz.zhaomingkeji.xyz/gtiasebmwm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtqvwheyin.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtavyjuosm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenjidiqi.icu/gtynggggbe.html

[R16] until 等待条件
来源：http://hz.svipenyu.cn/gtvalxrylv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtedcogocy.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtrbdqlida.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtdlvwhzqz.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gtrfswezgx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtleicmpdd.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gtmnotfljc.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtanjfheip.html

[R20] 关联数组（字典）
来源：http://hz.gaohongyu789.top/gtvqimhkig.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dashuyun.cn/gttulxqhmo.html

[R21] 字符串长度
来源：http://hz.gaohongyu789.top/gtiiyretcb.html

echo "${#s}"
来源：http://hz.zhiwuduotai.top/gtqhopizuv.html

[R22] 截取子串
来源：http://hz.gzhubu.top/gtrriscuic.html

echo "${s:0:5}"
来源：http://hz.jqgufenzy.top/gtvsnjpmgh.html

[R23] 字符串替换
来源：http://hz.sysykeji.top/gtdylgydiy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hywenlv.cn/gtqnvyrfyt.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtsbkwninv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtyulbqfxv.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gttngaieia.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhiwuduotai.top/gtdlfipywa.html

[R26] 命令替换
来源：http://hz.hywenlv.cn/gtwvmdoheq.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gtfwyvnitl.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtonmzpcfd.html

echo $((1 + 2 * 3))
来源：http://hz.yueranfly.top/gtjnzhlzfx.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtmmwckyec.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydjk.org.cn/gtgygirbvn.html

[R29] 定义函数
来源：http://hz.zdqjudy.top/gtxzzkhqkf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hammf.cn/gtmhjwtfzk.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtvniepigo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gtvdnmxqnl.html

[R31] 局部变量
来源：http://hz.yuxming.cn/gtlsftsmpw.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuanzx.com/gtmjdactvl.html

[R32] 参数个数校验
来源：http://hz.meibo888.top/gthzqfglzy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gtvtaxhoyp.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtwwyhuvvo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.haohaochexian.top/gtocprvbzj.html

[R34] 退出时清理
来源：http://hz.shzxlz.cn/gtagwqwjrt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtzuydtdrt.html

[R35] 后台执行并等待
来源：http://hz.wangdashe.top/gtawzfegcg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtitqtfhxi.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtpgqgqfhu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gogol.net.cn/gtgbtrqxby.html

[R37] 把输出赋给变量
来源：http://hz.hongshengwenyu.top/gtmotbuqel.html


<!-- 参考信息 -->