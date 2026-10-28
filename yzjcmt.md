代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cqqwz.cn/gtaddxjdvs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtnlqxctua.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cqqwz.cn/gtpyoptvmq.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtnoqygvfi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenzaomai.com/gtkjxrdwod.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtqbabwvpq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ybcxt.top/gtbqgbstik.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gaohongyu789.top/gtmevmqxfq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258888.top/gtgusdbkbc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dianchejie.cn/gtdhelqtli.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtidwbcadl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj202588.top/gtgdteveow.html

================================================================================
来源：http://hz.jyoumei.cn/gtwkzbaimb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtqgtxmydg.html

================================================================================
来源：http://hz.0kj1m.cn/gtdlqhxwwb.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtrdldlrlc.html

CREATE TABLE users (
来源：http://hz.cqqwz.cn/gtcxvcrflw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtlljdgdyc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gtfezdbdvu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenlongwang.top/gtawoodfyc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtukafwpes.html

);
来源：http://hz.jinqigfzy.top/gtvpijykhr.html

[Q02] 创建带外键的表
来源：http://hz.shangyingyoupin.top/gtaxqvlcrg.html

CREATE TABLE orders (
来源：http://hz.smart0.xyz/gtiorimiwh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gthsqplihy.html

user_id INT NOT NULL,
来源：http://hz.cdnleiting.top/gtsdbrwgqf.html

amount DECIMAL(10, 2),
来源：http://hz.cdnleiting.top/gtkeyxrgun.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhoulong.xyz/gtmwlrsmmw.html

);
来源：http://hz.ehwqpu.com/gtciwommcx.html

[Q03] 增加列
来源：http://hz.gogol.net.cn/gtymzgdvtc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuetiantiany.cn/gtplayegvb.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtnlxtxppl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangdashe.top/gtdbcvykps.html

[Q05] 重命名列
来源：http://hz.sxryk.cn/gtbdjdunhh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.svipenyu.cn/gtovmyhjfm.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtxtixnftf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.havefunace.top/gtjnfrfexi.html

[Q07] 删除表
来源：http://hz.shuidangran.top/gtnilhmyqz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xylfe.cn/gtwwqiluqc.html

[Q08] 创建普通索引
来源：http://hz.wangdashe.top/gtkvnpnmxj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuanzhike.top/gthkjzxkok.html

[Q09] 创建唯一索引
来源：http://hz.52xcode.cn/gtceobtwfm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtbqevtpko.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtcrsgheyb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shuidangran.top/gtxepbyoff.html

[Q11] 一次插入多行
来源：http://hz.ywan-chungtsiang.top/gtiwdeabia.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gttwinwtaz.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gthmlxkrtd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhongyouzk.top/gtgpkndmrz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.mhx1999.top/gtcrirzrgr.html

[Q13] 忽略重复插入
来源：http://hz.xylfe.cn/gtjpefhaka.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xinyue.icu/gtdfgxcnht.html

[Q14] 存在则更新（upsert）
来源：http://hz.ehwqpu.com/gtjygksdqh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuanzx.com/gthsqqrvzx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuxming.cn/gtyzbzokse.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtjgyleuaf.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtiieapqgt.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gtsparaped.html

SELECT id, name FROM users;
来源：http://hz.nwbrower.top/gtesgbupzt.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtkstqukam.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtujgxoypw.html

[Q18] 模糊匹配
来源：http://hz.0kj1m.cn/gthyfiqhli.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ivvv.top/gtjkloujvy.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gtlrxysfsz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtiqrrtbtf.html

[Q20] IN 列表
来源：http://hz.zhixingplan.top/gtdlraqmqk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangkeji.top/gtsznrrsko.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtuhoazueg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hongshengwenyu.top/gtoanhiwui.html

[Q22] 排序
来源：http://hz.cashguo.top/gtqdqkqpab.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangtech.top/gtrleukoec.html

[Q23] 分页
来源：http://hz.tanke756.top/gtjodjhbda.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tanke756.top/gtzfyfqimx.html

[Q24] 去重
来源：http://hz.xuanzx.com/gtesrgrncs.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gtiqvciuko.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gttkfqnjlp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.vqdsnc.cn/gtaoljoilp.html

[Q26] 计数
来源：http://hz.sufxvd.cn/gtxwcaenmx.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gtfkaaedky.html

[Q27] 条件计数
来源：http://hz.yonumen.top/gtdeyxsexv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cheryme.top/gtjyqgmlqn.html

[Q28] 求和与平均
来源：http://hz.xuanzx.com/gtxcblrhur.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtbxzanawn.html

[Q29] 最大最小值
来源：http://hz.yangfankeji.com/gtsvvzbvlt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigufen.top/gtpffgabzq.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtaxhklekx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yangfankeji.com/gtjfdqbque.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtpnmsfshe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ybcxt.top/gtuoqupuwc.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtwfkafszt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtaczsruib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yongpay.top/gtuitfljia.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtxmsksojh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtnlmujdmz.html

[Q34] 每组取第一条
来源：http://hz.zhixingplan.top/gthrnjphax.html

SELECT * FROM (
来源：http://hz.jinqigufen.top/gtssonlzck.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yanxiufei.cn/gtxgxoayqa.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gtamokwoma.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtmeyisiqw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtpgnuhdrr.html

[Q36] 左连接
来源：http://hz.jinqigufen.top/gtmfyjoued.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtchcrfxds.html

[Q37] 右连接
来源：http://hz.hysaishi.cn/gtbgveebfp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.316326.xyz/gtmuiaoffr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtroncjoqq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gtrrmgyuaw.html

[Q39] 自连接（查上下级）
来源：http://hz.chenjidiqi.icu/gtjgwounwb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yangfankeji.com/gtsqjkpyhs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gtwhbudxey.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.52xcode.cn/gtstoxuuvy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.c1oappe.top/gtffvhubwk.html

[Q41] 多表连接
来源：http://hz.kuanghao11.cn/gtbqexkytd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtqfltlvjb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigfzy.top/gtfpmcvtos.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ehwqpu.com/gtszeudcez.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gtmtuqfkok.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258888.top/gttjaszrem.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtvhoevoic.html

[Q43] 标量子查询
来源：http://hz.daxiang520.top/gtenhfpxgq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yvedp.cn/gtbnlfwwxg.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtgfhptouq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.bjfxy.top/gtmxujvvqy.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangkeji.top/gtsozesuln.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtvcovubff.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gteigoztue.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtkqktokot.html

[Q47] 与平均值比较
来源：http://hz.xinyue.icu/gtfazjbraw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuetiantiany.cn/gtftkierqn.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigfzy.top/gtlwrhguut.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtqnskmkcs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhoulong.xyz/gtrsplzeup.html

[Q49] 更新单行
来源：http://hz.feifeiyinyue.top/gthylfatyn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gtuonegwgl.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtqqlfgjfc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jqgufenzy.top/gtrilshqzw.html

[Q51] 用子查询更新
来源：http://hz.52xcode.cn/gtezgrjxoa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.meibo888.top/gttynxqmvr.html

[Q52] 删除指定行
来源：http://hz.snrcjt.cn/gtkeelxoam.html

DELETE FROM users WHERE id = 10;
来源：http://hz.316326.xyz/gtrboojazd.html

[Q53] 按条件删除
来源：http://hz.gogol.net.cn/gtwourxpcb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtkxtpxdmn.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtzjvmydqj.html

TRUNCATE TABLE logs;
来源：http://hz.pycfn.com/gtpjxoihzc.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gthhwxmpjo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.52xcode.cn/gtqhdrepjw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.redwolf501.top/gtpfoicbzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tian-w.cn/gtkqdrtamy.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtujzxessu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yanxiufei.cn/gttqqpyxto.html

[Q58] 累计求和
来源：http://hz.0kj1m.cn/gtbcbmxfnt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pycfn.com/gtrsbeewvf.html

[Q59] 分组内累计
来源：http://hz.ybcxt.top/gttbikuidi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gthurunqop.html

[Q60] 取上一行 / 下一行
来源：http://hz.hammf.cn/gtztsodtpk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fengsongda.top/gtqwltbtjx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtdpvwetmv.html

[Q61] 移动平均
来源：http://hz.bjfxy.top/gtwukmixcx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtikgrumru.html

[Q62] 分组占比
来源：http://hz.chenlongwang.top/gtjjngsyyj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtxvvrqflw.html

[Q63] 开启事务
来源：http://hz.yj202588.top/gthpjoyjwa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtztgyyvhe.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtcfbknzmc.html

COMMIT;
来源：http://hz.zhoulong.xyz/gtuegtezlt.html

[Q65] 回滚事务
来源：http://hz.gzhubu.top/gtiugdczcz.html

ROLLBACK;
来源：http://hz.hnxiangtu.top/gtsossexwh.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtlfcardcy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtnwxgdfig.html

[Q67] 设置隔离级别
来源：http://hz.mhx1999.top/gtrqtutraq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtmrdarecw.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtnlvgkgue.html

SAVEPOINT sp1;
来源：http://hz.jlsjyb.cn/gtzulfvpmd.html

ROLLBACK TO sp1;
来源：http://hz.zhijiandao.cn/gtvlmidaqr.html

[Q69] 查看执行计划
来源：http://hz.snrcjt.cn/gtqihftpzt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnqzz.top/gtpmcbqxqg.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtmcsxakoj.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtwbmgymbz.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtrvkahwtz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jiagoushi.top/gttgatrfnl.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtahcpwhqz.html

SHOW INDEX FROM users;
来源：http://hz.zdqjudy.top/gtfbzhwfyf.html

[Q73] 查看表状态
来源：http://hz.xylfe.cn/gtpoebrldm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ywan-chungtsiang.top/gtidyrekfx.html

[Q74] 强制使用索引
来源：http://hz.jyoumei.cn/gtjasiumsc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shuidangran.top/gtvopxgbin.html

[Q75] 日期格式化
来源：http://hz.kuanghao11.cn/gtbmyxdirr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtqsdswdan.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtmvibitwj.html

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtsuxllaer.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pengpengdd.cyou/gtvslmhqql.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtsfsrkexn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhongyouzk.top/gtoemnjxgc.html

[Q78] 当前时间
来源：http://hz.ybcxt.top/gtvndhbwnq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtvvmveluf.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtzdetaogg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258888.top/gtbrdvkftg.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gtigarxtfr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shuidangran.top/gtwyulhxbz.html

[Q81] 字符串替换
来源：http://hz.xuetiantiany.cn/gtfpbqjilk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtxfquuhir.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtwyfdbgku.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hysaishi.cn/gtkqizzice.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtauecsano.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtqdqbcsxp.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtprnqrtmq.html

SELECT TRIM(name) FROM users;
来源：http://hz.52xcode.cn/gtbrihhvut.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtmwegfheb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtxaqemqnq.html

[Q86] 读取 JSON 字段
来源：http://hz.sysykeji.top/gtqgjadkmy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.andypj.xyz/gtmqsnckht.html

[Q87] JSON 字段做条件
来源：http://hz.aibaodan.cn/gtbeqeuqqf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigufen.top/gthuranvqi.html

[Q88] 行转列（条件聚合）
来源：http://hz.cashguo.top/gtjpucshdp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gttgonlakt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zdqjudy.top/gtjlekclpv.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtasmgarok.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtfgkklyvq.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gtegksjxgx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhiwuduotai.top/gtaifnfuca.html

================================================================================
来源：http://hz.yj20258888.top/gtwtovqwtt.html

R. Bash 专题
来源：http://hz.yongpay.top/gthqavutaz.html

================================================================================
来源：http://hz.yuxming.cn/gtqpczmyrp.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtloncgpuv.html

#!/usr/bin/env bash
来源：http://hz.yonumen.top/gtjnvnriix.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtbeygduli.html

[R02] 变量赋值与使用
来源：http://hz.hfpthk.cn/gtikthilzn.html

name="Tom"; echo "$name"
来源：http://hz.0kj1m.cn/gtrsstiati.html

[R03] 只读变量
来源：http://hz.jinqigufen.top/gttorimgix.html

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtrxatmrcf.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtcghldxrw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zdqjudy.top/gtytrqjnbu.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtqymbanyt.html

name="${1:-default}"
来源：http://hz.quarkkingdee.top/gtrezasukq.html

[R06] 判断命令是否存在
来源：http://hz.yj20258.top/gtoyfhyuny.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xylfe.cn/gtfymdrfrf.html

[R07] if 判断文件
来源：http://hz.c1oappe.top/gtrddualze.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhixingplan.top/gtlhrbqksm.html

[R08] 数值比较
来源：http://hz.zhaomingkeji.xyz/gtxgjidqgt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinyuanbaomall.cn/gtjqyduzhs.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gtnkilcymb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gthhheoecz.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gtohellqkl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtrwoerhco.html

[R11] case 多分支
来源：http://hz.c1oappe.top/gtjaudcvzn.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gtpqgttpqs.html

start) echo "启动" ;;
来源：http://hz.jqgufenzy.top/gtfiihvmjc.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gtahnrfair.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtghwckzlv.html

esac
来源：http://hz.wangdashe.top/gtvsdupjoo.html

[R12] for 遍历文件
来源：http://hz.cashguo.top/gtuzoqvall.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cucudq.cn/gtjukphkbm.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtanmhdgwi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cqqwz.cn/gtpgfgchcm.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtdslmhkmb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtiwsyyfhd.html

[R15] while 逐行读文件
来源：http://hz.tanke756.top/gtptxdrsth.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.bjfxy.top/gtpjzejavj.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gteanzwaes.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtpjhrtqnm.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtdnwqimmv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jianghu66.top/gthbpzplbp.html

[R18] 遍历数组
来源：http://hz.zhongyouzk.top/gtszabmjbs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.svipenyu.cn/gtrzmysjgz.html

[R19] 数组长度
来源：http://hz.ppjwa.cn/gtpvopeync.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtfoccnugn.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gthjmrmgfr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xinyue.icu/gtklzqxiuc.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gtlnwcejfv.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gthpylavnw.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtvlgpytbg.html

echo "${s:0:5}"
来源：http://hz.sufxvd.cn/gtzmexjscr.html

[R23] 字符串替换
来源：http://hz.cqqwz.cn/gtflnnfqqe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gthqbsijhb.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtnbhsftaq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhoulong.xyz/gtgdrgivtv.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtwiezjvxk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtlghkfulp.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtpibmpdrp.html

now=$(date +%F); echo "$now"
来源：http://hz.guannengcc.top/gtzdhivowc.html

[R27] 算术展开
来源：http://hz.yongpay.top/gtosidntgt.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtkosezemh.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtdqdpugoo.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj202588.top/gtqoduxlcr.html

[R29] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtxwvnohsy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnxiangtu.top/gtibcscdxw.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtsjlqkadl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.316326.xyz/gtprpwfkyu.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtdqiyowky.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtdrznnzdx.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gtsxicdisa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jlsjyb.cn/gtrmnitfhq.html

[R33] 捕获错误并提示行号
来源：http://hz.ybcxt.top/gtgvafscqf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.iojbl.cn/gtuwygcdvo.html

[R34] 退出时清理
来源：http://hz.ydzc1.top/gtwlluowcy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtjwdzdrsa.html

[R35] 后台执行并等待
来源：http://hz.zycfv.cn/gthxliwwtx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangshuangyany.cn/gttrmlezzi.html

[R36] 并发执行多个任务
来源：http://hz.guowangkeji.top/gtlotuleel.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gogol.net.cn/gtjiubiejn.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtfbmtbcgl.html


<!-- 参考信息 -->