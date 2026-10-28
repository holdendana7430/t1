代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jiagoushi.top/gtdmzoxzti.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhijiandao.cn/gtxjxwmqoe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gtseivjwpv.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtgzmupvbw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenlongwang.top/gtitwzdnvw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtxngnyhdf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dianchejie.cn/gtmbduupcf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxinkj.top/gthlyfccyg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gttwiplpuy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hongshengwenyu.top/gtmnxjtcqb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydzc1.top/gtjuwpywix.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.mhx1999.top/gtkzvwgrso.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqqmbnumf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtikfboafn.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtkztrbsvu.html

[Q01] 创建表
来源：http://hz.yj202588.top/gtfotvvnnl.html

CREATE TABLE users (
来源：http://hz.nwbrower.top/gtwmcigodz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtsxjiatmi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtmogykcog.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtxxtwwzyb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtumdubram.html

);
来源：http://hz.shzxlz.cn/gtqbhzough.html

[Q02] 创建带外键的表
来源：http://hz.wangshuangyany.cn/gtbsdrzcdw.html

CREATE TABLE orders (
来源：http://hz.hysaishi.cn/gtyztkyfsp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtvkmwkurp.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtxjzawtvr.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtugvjhlaf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.haohaochexian.top/gtrgiaulbj.html

);
来源：http://hz.haohaochexian.top/gtoccwxilw.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtkipfpwlt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.mhx1999.top/gtrzsdrnvs.html

[Q04] 修改列类型
来源：http://hz.redwolf501.top/gtzfreoijk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtqbhgkqkr.html

[Q05] 重命名列
来源：http://hz.zycfv.cn/gtnhmqtkqi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtsspenhoo.html

[Q06] 删除列
来源：http://hz.zhiwuduotai.top/gtnxowtakd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hongshengwenyu.top/gtuqicrzzk.html

[Q07] 删除表
来源：http://hz.chenlongwang.top/gtlqdajgky.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gthmooqlsx.html

[Q08] 创建普通索引
来源：http://hz.tanke756.top/gtenrnchmb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.mhx1999.top/gtgzldosny.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtzbpmekwr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yueranfly.top/gthsngebwb.html

[Q10] 插入单行
来源：http://hz.chenlongwang.top/gtbgzpbmtw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtttswdutl.html

[Q11] 一次插入多行
来源：http://hz.chenzaomai.com/gtrrudqwmu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenlongwang.top/gtfecmojkj.html

[Q12] 插入后取自增 ID
来源：http://hz.sweek.top/gthlfeqymd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gogol.net.cn/gtwijyywdq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.redwolf501.top/gtffyxbljn.html

[Q13] 忽略重复插入
来源：http://hz.xziqi.cn/gtgqapmveo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zycfv.cn/gtqghaupon.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtouxojjfk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ybcxt.top/gtxpsnmylw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhoulong.xyz/gtszxzpirw.html

[Q15] 查询全部
来源：http://hz.zhengqikj.top/gtvnpbyuav.html

SELECT * FROM users;
来源：http://hz.yanxiufei.cn/gtragqmjvy.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtyoxmxuan.html

SELECT id, name FROM users;
来源：http://hz.gotoacloud.top/gtjcgosflz.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtnijrqmyi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gtxdyfixgf.html

[Q18] 模糊匹配
来源：http://hz.sysykeji.top/gtfnonkcgy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gthqmcdhvi.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gtglesywzs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.pengpengdd.cyou/gtnkavbyso.html

[Q20] IN 列表
来源：http://hz.jlsjyb.cn/gtjtocxqer.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.meibo888.top/gtngtjbfwx.html

[Q21] 空值判断
来源：http://hz.nanxuanxn.top/gtvxtbzwaf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ybcxt.top/gtyshmlgov.html

[Q22] 排序
来源：http://hz.daria6918.cn/gtuynnbvte.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangkeji.top/gtbdccwpda.html

[Q23] 分页
来源：http://hz.havefunace.top/gtpevwavwf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtgmatrqbj.html

[Q24] 去重
来源：http://hz.havefunace.top/gtavtlkcar.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydjk.org.cn/gtsvbhjdln.html

[Q25] 只取前 N 条
来源：http://hz.daxiang520.top/gttsxuvpjh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtwvwhhkgj.html

[Q26] 计数
来源：http://hz.52xcode.cn/gtzdsnuyck.html

SELECT COUNT(*) FROM users;
来源：http://hz.dianchejie.cn/gtmxkkkbzy.html

[Q27] 条件计数
来源：http://hz.jiagoushi.top/gtazfzosol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhixingplan.top/gtxieivbjl.html

[Q28] 求和与平均
来源：http://hz.sufxvd.cn/gtudeakgzh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydjk.org.cn/gtdbjpplbz.html

[Q29] 最大最小值
来源：http://hz.jlsjyb.cn/gtjndxjnlp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.c1oappe.top/gtqyqbsmiu.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtlmrgkmnr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtmmclhmlb.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gtroqcsfaq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenzaomai.com/gtfqprrzgl.html

[Q32] 分组拼接字符串
来源：http://hz.ehwqpu.com/gtczwjkcsq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtxlbkoqvf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtozeqzqdf.html

[Q33] 多列分组
来源：http://hz.yonumen.top/gthcxjgpyj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yangfankeji.com/gtoxqkzdrx.html

[Q34] 每组取第一条
来源：http://hz.jianghu66.top/gtztdckzwh.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtlwyakrjx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangdashe.top/gtwcpwlmoa.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtrsrhfvns.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtpglwajrm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtlmxebjjo.html

[Q36] 左连接
来源：http://hz.zhiwuduotai.top/gtuskjoalw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtttpclrfo.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtseluycbl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangshuangyany.cn/gtjzcjuvpk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yonumen.top/gtrutzrrch.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtrfkyvgul.html

[Q39] 自连接（查上下级）
来源：http://hz.guannengcc.top/gtwpadplqk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cashguo.top/gtygrgjfog.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhixingplan.top/gtkbbwmrji.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.vqdsnc.cn/gtwluevwwm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangtech.top/gtvevmlflo.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gtjojfectm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.redwolf501.top/gtynzbywwg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangkeji.top/gtrlnjvibm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fengsongda.top/gtggoenmyk.html

[Q42] 连接条件附加过滤
来源：http://hz.cashguo.top/gtlemnlmtd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhongyouzk.top/gtouwmzqhc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtupbdadyd.html

[Q43] 标量子查询
来源：http://hz.sweek.top/gtmrdrncuj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.bjfxy.top/gtmqitxngk.html

[Q44] IN 子查询
来源：http://hz.jinqigufen.top/gtannocsjo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenlongwang.top/gtmowwkwps.html

[Q45] EXISTS 判断存在
来源：http://hz.jyoumei.cn/gtjkbmzawk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gtsajwnbsz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gtccakfhya.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtvdeiqktv.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtwospixma.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtpinaxpzv.html

[Q48] CTE 公用表表达式
来源：http://hz.iojbl.cn/gtwmpjvolp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.bjfxy.top/gtsafznvxn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtuoykzleu.html

[Q49] 更新单行
来源：http://hz.jinqigufen.top/gtawgykqgr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gtnhmomepb.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtcobifyel.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuanzx.com/gthwiekvda.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gtmafoiklo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sysykeji.top/gtsmzxxciq.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtcvbssxxj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.smart0.xyz/gtqzderfsu.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtujpdodjo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ivvv.top/gtaxoqrkhs.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtuaihwooa.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtkvgollku.html

[Q55] 排名（并列占位）
来源：http://hz.kuanghao11.cn/gtrdjhcqrk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtcpgaroqj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yongpay.top/gtelbfztld.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangdashe.top/gtanlcqgqp.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtperxnkej.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtbjcarxvb.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gttgpddive.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtjqywrnyv.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtulmlgssl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.smart0.xyz/gtgzeqtful.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gtnyvvjrvm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sxryk.cn/gtkxxegdkw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtfveioexo.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtcqjtftuu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtferyknwb.html

[Q62] 分组占比
来源：http://hz.xylfe.cn/gtnopiyctz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtoaezgmxx.html

[Q63] 开启事务
来源：http://hz.shangyingyoupin.top/gttqozjmlu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.316326.xyz/gtkggoadwz.html

[Q64] 提交事务
来源：http://hz.nwbrower.top/gtcnchoosh.html

COMMIT;
来源：http://hz.dianchejie.cn/gtpflqeyeo.html

[Q65] 回滚事务
来源：http://hz.52xcode.cn/gtptovcrfw.html

ROLLBACK;
来源：http://hz.yuxming.cn/gtxkovmneq.html

[Q66] 行锁查询
来源：http://hz.zhixingplan.top/gtpywlqdvk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtaeuqoqbc.html

[Q67] 设置隔离级别
来源：http://hz.hfpthk.cn/gtxvramfag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gogol.net.cn/gttulcdxth.html

[Q68] 保存点
来源：http://hz.hywenlv.cn/gtrulrzzoy.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtjrnzoeou.html

ROLLBACK TO sp1;
来源：http://hz.xuanzx.com/gtmlmixksa.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtpkokhbjo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ehwqpu.com/gtjkpxfxef.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gtetjmqlsy.html

ANALYZE TABLE users;
来源：http://hz.yj20258.top/gtvtrglomf.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtbtzzyfvg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shuidangran.top/gtlehurksw.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtssgcyids.html

SHOW INDEX FROM users;
来源：http://hz.hammf.cn/gthtjbjvyw.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtpzrstzfr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhaomingkeji.xyz/gtxumkybwa.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gtarokcend.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangtech.top/gtrrpqsmaq.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtadxspigh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtweopekbx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shangyingyoupin.top/gtityuvody.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtucytrinz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtpocktbcu.html

[Q77] 时间加减
来源：http://hz.bjfxy.top/gtvctgkzzb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtoyrcaqjs.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtivnbqxfc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gticlhbtcs.html

[Q79] 字符串拼接
来源：http://hz.zhengqikj.top/gtgjhetohw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.bjfxy.top/gtutvpnuqq.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gtinvzzwsg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhijiandao.cn/gtphpuaxzd.html

[Q81] 字符串替换
来源：http://hz.yj20258888.top/gtxeqojiaq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhiwuduotai.top/gtpaliwhqw.html

[Q82] 字符长度与字节长度
来源：http://hz.ywan-chungtsiang.top/gtkmguurbi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtvijjmdzo.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtcgyzxygo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhengqikj.top/gtcskoporh.html

[Q84] 去除首尾空格
来源：http://hz.chenlongwang.top/gtntybofjd.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigufen.top/gtuvzttqsq.html

[Q85] 数值取整
来源：http://hz.hywenlv.cn/gtujrqxllz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuanzhike.top/gthirlwghl.html

[Q86] 读取 JSON 字段
来源：http://hz.hnqzz.top/gtripmetqe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtshabaneh.html

[Q87] JSON 字段做条件
来源：http://hz.yvedp.cn/gtrbocnzti.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenlongwang.top/gtqtoolghs.html

[Q88] 行转列（条件聚合）
来源：http://hz.hongshengwenyu.top/gtfvtmgteg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.c1oappe.top/gtteysdkeq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuanzhike.top/gtdyqahdbp.html

[Q89] 判断表是否存在
来源：http://hz.nanxinkj.top/gtdjcamqlc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtattgrnqp.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtbaoacyjf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtamhqdswo.html

================================================================================
来源：http://hz.zhijiandao.cn/gthzfkmxpg.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtphsbnijk.html

================================================================================
来源：http://hz.andypj.xyz/gtruvruxrz.html

[R01] shebang 与严格模式
来源：http://hz.shzxlz.cn/gtmsupnvsd.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtfnyfebsr.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtlftgwddy.html

[R02] 变量赋值与使用
来源：http://hz.xingfuxueyuan.xyz/gtfkxlknhc.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtpxtrtoid.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gtjxzgusbg.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtjvtpwbtf.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gtrnvxgmaq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pycfn.com/gtlygqxtwt.html

[R05] 参数默认值
来源：http://hz.gogol.net.cn/gtqomftuco.html

name="${1:-default}"
来源：http://hz.zycfv.cn/gtpgkckxyb.html

[R06] 判断命令是否存在
来源：http://hz.fengsongda.top/gtojyhyxto.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.iojbl.cn/gtloquefcs.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtzoicuizf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gtqsbulzkr.html

[R08] 数值比较
来源：http://hz.jinqigufen.top/gtwxcisfol.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtyyrlfwmv.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtvostdpis.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.svipenyu.cn/gtdvgkecnw.html

[R10] 正则匹配
来源：http://hz.sxryk.cn/gtbcmbhwjx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aibaodan.cn/gteygzsvfa.html

[R11] case 多分支
来源：http://hz.fengsongda.top/gttojgbbnq.html

case "$1" in
来源：http://hz.jyoumei.cn/gtpvynlwto.html

start) echo "启动" ;;
来源：http://hz.dianchejie.cn/gtzexwkfxd.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gtypzspjfu.html

*)     echo "未知命令" ;;
来源：http://hz.c1oappe.top/gtnzizbjht.html

esac
来源：http://hz.nwbrower.top/gtmpysfwkm.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtknzmevzx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cdnleiting.top/gtagfjnlpe.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtfubafvbg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gtkcsgxols.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gtjhvyczdl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtgxfhzxmo.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtgjrzvkwd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinghuilouyu.cn/gtnsqvczya.html

[R16] until 等待条件
来源：http://hz.yangfankeji.com/gtwuawxfpt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jyoumei.cn/gtwptnuahl.html

[R17] 数组定义与取值
来源：http://hz.tianlin.xyz/gtkautohrc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fzhhl.top/gtetquqitv.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtisoqvetm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtvnygpbzu.html

[R19] 数组长度
来源：http://hz.haohaochexian.top/gtsvjhyzrf.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtyhlszvvp.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtpfqtnajq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cqqwz.cn/gtbuocolqy.html

[R21] 字符串长度
来源：http://hz.cheryme.top/gtxhqzoxlo.html

echo "${#s}"
来源：http://hz.shzxlz.cn/gtfpqerqev.html

[R22] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtnouccrhr.html

echo "${s:0:5}"
来源：http://hz.yanxiufei.cn/gttbwwbxni.html

[R23] 字符串替换
来源：http://hz.jinqigufen.top/gtpcttdpvj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtcjupunpl.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtoqmaksoq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.smart0.xyz/gtsmslxykk.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxinkj.top/gtgxaccryi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtldaerqtp.html

[R26] 命令替换
来源：http://hz.316326.xyz/gtyjwuijsq.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtcheukzkt.html

[R27] 算术展开
来源：http://hz.ehwqpu.com/gtnsxefsdq.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtgwhyspsy.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtmrablicu.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtlaetdlxt.html

[R29] 定义函数
来源：http://hz.yj202588.top/gterxbyxaq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.iojbl.cn/gtznxglirw.html

[R30] 函数返回状态码
来源：http://hz.hnqzz.top/gtgsqegxju.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gthiqlcbjl.html

[R31] 局部变量
来源：http://hz.havefunace.top/gtddflxwhg.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gtjatstlag.html

[R32] 参数个数校验
来源：http://hz.smart0.xyz/gtrxomxkys.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtbjfqwwse.html

[R33] 捕获错误并提示行号
来源：http://hz.tanke756.top/gtojtdzvad.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tanke756.top/gtzyxkdurx.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtgakqcyps.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtljcujweb.html

[R35] 后台执行并等待
来源：http://hz.shzxlz.cn/gttcfvsohz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gtiiwmwzks.html

[R36] 并发执行多个任务
来源：http://hz.zhaomingkeji.xyz/gtwvslxzuo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.birdmap.top/gtxaswmvsl.html

[R37] 把输出赋给变量
来源：http://hz.guowangkeji.top/gtskfbsdhw.html


<!-- 参考信息 -->