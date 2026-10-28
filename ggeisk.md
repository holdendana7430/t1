代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.ehwqpu.com/gtlwgzmkrx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtaznylfjg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtqffvbops.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangshuangyany.cn/gtpgwwhxhl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guannengcc.top/gtopezeitw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gthsgxgcio.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtmzcwspra.html

[P08] 处理浮点精度问题
来源：http://hz.wangshuangyany.cn/gtsadmfvgo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jlsjyb.cn/gthouxrewe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xinyue.icu/gtbxizmawl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtoddcbnph.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cqqwz.cn/gtnqebytbx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuanzhike.top/gteamtgisi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.c1oappe.top/gtyucsclcb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtpzrogxon.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258.top/gtsfpnbsfl.html

================================================================================
来源：http://hz.yj20258888.top/gtnmkhmvmg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtxftxqaax.html

================================================================================
来源：http://hz.zhixingplan.top/gtnstvxuio.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtwczfjizb.html

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtkpucduxy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gttojwjbdp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangshuangyany.cn/gtllxkltlh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.redwolf501.top/gtbavdctil.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daria6918.cn/gthkvajhat.html

);
来源：http://hz.yonumen.top/gtukkhybrt.html

[Q02] 创建带外键的表
来源：http://hz.yj202588.top/gtsdwawdwp.html

CREATE TABLE orders (
来源：http://hz.xylfe.cn/gtxetddmnc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtfmuwcxex.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtrhobqarl.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtygrpaant.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fzhhl.top/gtrfoaqnyg.html

);
来源：http://hz.jqgufenzy.top/gtmxwrsayy.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtnajyeiqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.snrcjt.cn/gtwwfayikg.html

[Q04] 修改列类型
来源：http://hz.cashguo.top/gtmskmiggy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.meibo888.top/gtggpinbip.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtbdodpauv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jyoumei.cn/gtlonhypvl.html

[Q06] 删除列
来源：http://hz.jyoumei.cn/gtrjpmmivh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aizwys.cn/gtgnilfzxc.html

[Q07] 删除表
来源：http://hz.pengpengdd.cyou/gtsqqibgoz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shangyingyoupin.top/gtlwvbwsol.html

[Q08] 创建普通索引
来源：http://hz.tian-w.cn/gtppzavgno.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtfdltewee.html

[Q09] 创建唯一索引
来源：http://hz.pycfn.com/gtzscnpbyx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtttrchbjc.html

[Q10] 插入单行
来源：http://hz.gotoacloud.top/gtlhwlwbvm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuanzhike.top/gtuurqcslf.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gtpaehwiyz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtcovlmvnh.html

[Q12] 插入后取自增 ID
来源：http://hz.shangyingyoupin.top/gttrcidehw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nwbrower.top/gtaxenwfft.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gzhubu.top/gtwazjwepv.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gttaxvdyte.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gtujmlxure.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtmxqcndsc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gtqvnhiqdl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtwzrjjjee.html

[Q15] 查询全部
来源：http://hz.hnxiangtu.top/gttpnmzmnv.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtcrcisklr.html

[Q16] 查询指定列
来源：http://hz.guannengcc.top/gtgeemjpja.html

SELECT id, name FROM users;
来源：http://hz.ybcxt.top/gtnqolyzyk.html

[Q17] 条件查询
来源：http://hz.gaohongyu789.top/gtwohapshw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hywenlv.cn/gtxejzrwra.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtzngcelah.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gzhubu.top/gtrtsirqve.html

[Q19] 范围查询
来源：http://hz.jlsjyb.cn/gtohkvjsxs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.9152youxi.cn/gtrfmytuid.html

[Q20] IN 列表
来源：http://hz.sweek.top/gtpyyvwcdc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tian-w.cn/gtmufraecz.html

[Q21] 空值判断
来源：http://hz.aizwys.cn/gtrktemfbr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtcqkfzflb.html

[Q22] 排序
来源：http://hz.xziqi.cn/gtcqnamkcf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.redwolf501.top/gtergblxko.html

[Q23] 分页
来源：http://hz.quarkkingdee.top/gtzzvbvtoh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gtgeurmppc.html

[Q24] 去重
来源：http://hz.fengsongda.top/gthbbiyfii.html

SELECT DISTINCT city FROM users;
来源：http://hz.haohaochexian.top/gtnetpghat.html

[Q25] 只取前 N 条
来源：http://hz.snrcjt.cn/gttqkwvghe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ppjwa.cn/gtkbvqsncj.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtuckrqeaz.html

SELECT COUNT(*) FROM users;
来源：http://hz.cdnleiting.top/gtxbjrvzup.html

[Q27] 条件计数
来源：http://hz.daria6918.cn/gtypvipfay.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.316326.xyz/gtmmxjwgbl.html

[Q28] 求和与平均
来源：http://hz.tian-w.cn/gtvpulcvtj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gtywhiauhk.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtwvmgtlhc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.c1oappe.top/gtrhlagxyr.html

[Q30] 分组统计
来源：http://hz.svipenyu.cn/gtinbqgozg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtbusduggg.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtgctslbam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtimcdctqm.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtfgdgikmr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtxvzdftre.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aizwys.cn/gtywhsdusw.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtdtouupgt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtlruzmzsb.html

[Q34] 每组取第一条
来源：http://hz.yongpay.top/gtwlnzhyll.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gtsdunwoyb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shanyushiyangtech.top/gtlekmnxrs.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtrimdcebo.html

[Q35] 内连接
来源：http://hz.havefunace.top/gttruwjtll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtcczxulqy.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtkvvgsklh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtqfaqhltm.html

[Q37] 右连接
来源：http://hz.yonumen.top/gthqpjdvzg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pycfn.com/gtloxrinhy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cheryme.top/gtlmbiwnpu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xziqi.cn/gtjubjrjcg.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtuejtbqpm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gteoyzrmht.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtihcxzvbb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtuizyenml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhiwuduotai.top/gtskqqcqqw.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gtiuzcapez.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guannengcc.top/gtcutvhcww.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gthkosawst.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.smart0.xyz/gtfqapzywo.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtmemadpoj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnxiangtu.top/gthdijhlal.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.vqdsnc.cn/gtwverbsxv.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gtpgdfttuf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtrbxdmobv.html

[Q44] IN 子查询
来源：http://hz.ywan-chungtsiang.top/gtkhapacdk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj20258888.top/gtnyrwknhf.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtdwvqvuop.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gttnswumbs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aibaodan.cn/gtfvbtymdd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtzishqvlt.html

[Q47] 与平均值比较
来源：http://hz.zhixingplan.top/gtdzadoafy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yueranfly.top/gtvzrsgifq.html

[Q48] CTE 公用表表达式
来源：http://hz.jiagoushi.top/gtbaamgpio.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuxming.cn/gtppmslued.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.c1oappe.top/gtpsnocjov.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gtqtyjhjny.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtmckpidjb.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtzphbgdzf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.smart0.xyz/gtdytydfii.html

[Q51] 用子查询更新
来源：http://hz.hfpthk.cn/gtmtibzdgf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ehwqpu.com/gtepcokuwx.html

[Q52] 删除指定行
来源：http://hz.chenjidiqi.icu/gtfkufnjac.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhijiandao.cn/gthspyeyvi.html

[Q53] 按条件删除
来源：http://hz.yj20258.top/gtiozajfyf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dianchejie.cn/gtbeozjbgc.html

[Q54] 清空表
来源：http://hz.yj20258.top/gtieeqispy.html

TRUNCATE TABLE logs;
来源：http://hz.ydzc1.top/gtwctpmevf.html

[Q55] 排名（并列占位）
来源：http://hz.316326.xyz/gtywdpfsni.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtqxenhzjr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.redwolf501.top/gttenqnlao.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tanke756.top/gtibvwshin.html

[Q57] 行号
来源：http://hz.guowangkeji.top/gtqvoapkyr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nwbrower.top/gtpqmxthwv.html

[Q58] 累计求和
来源：http://hz.chenjidiqi.icu/gtujckpeez.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gtstyicpzv.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gticguggme.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuanzx.com/gtyzcbaiiq.html

[Q60] 取上一行 / 下一行
来源：http://hz.fengsongda.top/gtnbjhhpdd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gturxfncbv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangdashe.top/gtcoiomzwt.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtjmwrgwjj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.mhx1999.top/gttntsvbvn.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtfbfaikwg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtunerirps.html

[Q63] 开启事务
来源：http://hz.xziqi.cn/gtfjtbihgo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yonumen.top/gtydfsjjup.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtbiktdtfa.html

COMMIT;
来源：http://hz.sxryk.cn/gtrwvdgrrf.html

[Q65] 回滚事务
来源：http://hz.daxiang520.top/gtvxbqrgwa.html

ROLLBACK;
来源：http://hz.yueranfly.top/gtntitjozs.html

[Q66] 行锁查询
来源：http://hz.sysykeji.top/gtlikmhfem.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtucvxfwwl.html

[Q67] 设置隔离级别
来源：http://hz.yueranfly.top/gtsomyxyzo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtmimwpvgm.html

[Q68] 保存点
来源：http://hz.yanxiufei.cn/gtonyhexuo.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gticeojemd.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtcttkzuir.html

[Q69] 查看执行计划
来源：http://hz.feifeiyinyue.top/gtpvkqftdk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigfzy.top/gtmylhskmw.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangtech.top/gtfpbteimz.html

ANALYZE TABLE users;
来源：http://hz.jqgufenzy.top/gtqgrhfxxj.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtwicwapuv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtlvihliwv.html

[Q72] 查看索引
来源：http://hz.shanyushiyangtech.top/gtvcttmwhx.html

SHOW INDEX FROM users;
来源：http://hz.aizwys.cn/gtgbcrgdta.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gthpbvfhsb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangkeji.top/gttpwlxgku.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtpsskjiuk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtotxkxfxw.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gtojwqcbxv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtlkesviuq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sysykeji.top/gtmzsorssb.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtnsydtgsh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhiwuduotai.top/gttuewjceo.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtunlutgrg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gtvozuzsdb.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtbvfjviws.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtisvrrvxf.html

[Q79] 字符串拼接
来源：http://hz.zhijiandao.cn/gtksfuvrxu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtguypdlrp.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtdblbaqrf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guowangkeji.top/gtyfwaxpbw.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtxsqtcnby.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cucudq.cn/gtryfjvzuo.html

[Q82] 字符长度与字节长度
来源：http://hz.fengsongda.top/gtsplmfngv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cqqwz.cn/gtocisqqcd.html

[Q83] 大小写转换
来源：http://hz.gotoacloud.top/gtvkmsprnh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gtobdhsiak.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtikzlrgza.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtjlzfstne.html

[Q85] 数值取整
来源：http://hz.bjfxy.top/gthtkezyti.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtujhtgvsa.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtbupusmpo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtffqjzkpt.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtatggohad.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cashguo.top/gthilljslb.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtehxkyqjs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xuanzx.com/gtlitxosrr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhaomingkeji.xyz/gtbggyalks.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtqywcwzoq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.vqdsnc.cn/gtrolswipy.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtipgxisbr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtwqhpnzdo.html

================================================================================
来源：http://hz.tanke756.top/gtdkvaaqbq.html

R. Bash 专题
来源：http://hz.316326.xyz/gtkukmirad.html

================================================================================
来源：http://hz.sxryk.cn/gtadkwyaxr.html

[R01] shebang 与严格模式
来源：http://hz.snrcjt.cn/gtuwojoczp.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtbihoxsyy.html

set -euo pipefail
来源：http://hz.ydjk.org.cn/gtwbqveqqe.html

[R02] 变量赋值与使用
来源：http://hz.jianghu66.top/gtkocalueo.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtyhxywzho.html

[R03] 只读变量
来源：http://hz.mhx1999.top/gtowswomar.html

readonly PI=3.14
来源：http://hz.cashguo.top/gtrcohpbqb.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtymexceum.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuanzx.com/gtqdmsdpxo.html

[R05] 参数默认值
来源：http://hz.yuxming.cn/gtbmzbclsv.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtaifvldcc.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtspqwrmxi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aizwys.cn/gtuovslmci.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gterbdwzra.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nwbrower.top/gtbzrhtxmj.html

[R08] 数值比较
来源：http://hz.yangfankeji.com/gtziqgxzdl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sysykeji.top/gtmbnzggzc.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gtechrtpdm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtxvlxtgmf.html

[R10] 正则匹配
来源：http://hz.ehwqpu.com/gtjuskepzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhiwuduotai.top/gtlclsxtos.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtotadhxlp.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtgykgvmfd.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gtkhtimsjb.html

stop)  echo "停止" ;;
来源：http://hz.chenzaomai.com/gtnvogmkrm.html

*)     echo "未知命令" ;;
来源：http://hz.sysykeji.top/gtwwgdvkjz.html

esac
来源：http://hz.xinyue.icu/gtaumbeowu.html

[R12] for 遍历文件
来源：http://hz.jlsjyb.cn/gtwgupntdq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtudrxdhla.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gthjaumevv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtdpdbrbsu.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtbtxgcipy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhengqikj.top/gtdgiejdmy.html

[R15] while 逐行读文件
来源：http://hz.xuetiantiany.cn/gtfdbnwsph.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtbyvdzxzl.html

[R16] until 等待条件
来源：http://hz.nanxinkj.top/gtxxwvechd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtfzetvcbj.html

[R17] 数组定义与取值
来源：http://hz.hfpthk.cn/gtnqmdlotq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shangyingyoupin.top/gtzfgfaykw.html

[R18] 遍历数组
来源：http://hz.hongshengwenyu.top/gtsypsctyh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtxznrvfhx.html

[R19] 数组长度
来源：http://hz.zycfv.cn/gtvjlaoovb.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gtcdnhholo.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gtrsjjzszw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtxekcsvbg.html

[R21] 字符串长度
来源：http://hz.aizwys.cn/gtqivkcihi.html

echo "${#s}"
来源：http://hz.9152youxi.cn/gtuyavesap.html

[R22] 截取子串
来源：http://hz.jianghu66.top/gtpgdrowzd.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtkmplojvh.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gthkvmjkqj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtonbhohbf.html

[R24] 大小写转换
来源：http://hz.hnxiangtu.top/gtfofpfidd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gteuvghdhe.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtrzahvxks.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gtzyevuufy.html

[R26] 命令替换
来源：http://hz.kuanghao11.cn/gtiykugidc.html

now=$(date +%F); echo "$now"
来源：http://hz.bjfxy.top/gtfdozwvxj.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtsajweylw.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtbfhdpasy.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtxtipnipw.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtckhgwsji.html

[R29] 定义函数
来源：http://hz.haohaochexian.top/gtnndlleve.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gtfylgpodm.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtxoyqivue.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtqwbalbtt.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gtmkspqdyw.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtplyytrrg.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gthxczqgzp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtujavbqxd.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtfgqxyfzz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtpgyaoknm.html

[R34] 退出时清理
来源：http://hz.shangyingyoupin.top/gtdwjlkbjd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gttbqfdaqo.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtyrixybls.html


<!-- 参考信息 -->