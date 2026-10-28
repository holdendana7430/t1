代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cqqwz.cn/gtomirxepx.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtangebtgi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.andypj.xyz/gteoskirtt.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gtxcqhcmdg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtlqtxscls.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gtkmtfxcsm.html

[P07] 防抖与节流
来源：http://hz.yonumen.top/gtwldfkieq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtnqwiufuv.html

PHP:  // 手写时间戳比较
来源：http://hz.quarkkingdee.top/gtdkhfxotu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtwlqvscxd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtafkwqzff.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gzhubu.top/gtslysijcd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gtkitpmipe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtudfmlwxn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtyoegqbze.html

[P08] 处理浮点精度问题
来源：http://hz.hongshengwenyu.top/gtexjljzwc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shangyingyoupin.top/gtdtpxyacu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtcaisdktf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gttmgxviyz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.dashuyun.cn/gtusqlosip.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtbcgzixuf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zdqjudy.top/gtdcpvaazd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xinyue.icu/gtrnhnmfgd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gtmpmodpzs.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtlxacltek.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.feifeiyinyue.top/gtdqrkexoi.html

================================================================================
来源：http://hz.jiagoushi.top/gtwmidxgkz.html

[Q01] 创建表
来源：http://hz.dianchejie.cn/gtznmhygfm.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gthrhkifor.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtwtjtmums.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenjidiqi.icu/gtsorrdisy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.havefunace.top/gtxzcjlwbj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtuujfhydk.html

);
来源：http://hz.shanyushiyangkeji.top/gtzpzfbumg.html

[Q02] 创建带外键的表
来源：http://hz.9152youxi.cn/gtrqmgwafg.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gteyxhoidw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtxihlhmji.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtkciyhhyn.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtuayikfnc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sweek.top/gtzitkrlxh.html

);
来源：http://hz.ehwqpu.com/gtvnivmhqf.html

[Q03] 增加列
来源：http://hz.sysykeji.top/gtczcafihw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtzswefldu.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtvbcriuok.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtrqwlcphs.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtgxduesaq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dashuyun.cn/gtmyapwahg.html

[Q06] 删除列
来源：http://hz.daxiang520.top/gtjsiqfgth.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.havefunace.top/gtmajslyrh.html

[Q07] 删除表
来源：http://hz.xziqi.cn/gtydmhmqzv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.mhx1999.top/gtlfxumpxs.html

[Q08] 创建普通索引
来源：http://hz.feifeiyinyue.top/gtsukkhpif.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtewmelbro.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtugmjcvty.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtubpupzow.html

[Q10] 插入单行
来源：http://hz.316326.xyz/gtanscbwyo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtrsazmsxm.html

[Q11] 一次插入多行
来源：http://hz.gaohongyu789.top/gtyctslkgw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jiagoushi.top/gtkomzgkwo.html

[Q12] 插入后取自增 ID
来源：http://hz.jyoumei.cn/gtcysinjue.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinghuilouyu.cn/gtbrqmbwpu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtlcsqykiu.html

[Q13] 忽略重复插入
来源：http://hz.xziqi.cn/gtdgljorfc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.redwolf501.top/gtsoceorip.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtmqjsezqs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gotoacloud.top/gtjxfhahvf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hongshengwenyu.top/gtseqzxohy.html

[Q15] 查询全部
来源：http://hz.chenjidiqi.icu/gtlrzugjfb.html

SELECT * FROM users;
来源：http://hz.xinyue.icu/gtqjmxydyj.html

[Q16] 查询指定列
来源：http://hz.yj202588.top/gtosxtidgj.html

SELECT id, name FROM users;
来源：http://hz.ppjwa.cn/gtkmousvjl.html

[Q17] 条件查询
来源：http://hz.tanke756.top/gtvbvspwzv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhongyouzk.top/gtpgqbllmg.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtqxfipxbk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sufxvd.cn/gtsuzuuazh.html

[Q19] 范围查询
来源：http://hz.52xcode.cn/gtifqhmymk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cheryme.top/gtqqgtsong.html

[Q20] IN 列表
来源：http://hz.52xcode.cn/gtdrmtblfr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zdqjudy.top/gtkjqeennh.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gtpbdknple.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.andypj.xyz/gtkiulhabh.html

[Q22] 排序
来源：http://hz.zhaomingkeji.xyz/gtpzuaiomm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnxiangtu.top/gtltovwthl.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gtefkxcvfj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shzxlz.cn/gtvecymixx.html

[Q24] 去重
来源：http://hz.gzhubu.top/gtheapvqkt.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenzaomai.com/gtdmrqxfwo.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtkisacxvr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guowangkeji.top/gtdecfxfam.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtrzkczayz.html

SELECT COUNT(*) FROM users;
来源：http://hz.haohaochexian.top/gtnfvqhayl.html

[Q27] 条件计数
来源：http://hz.cashguo.top/gthvrkknbj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhongyouzk.top/gtesnylbwe.html

[Q28] 求和与平均
来源：http://hz.birdmap.top/gtehjkdptb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gtfuhzvmwt.html

[Q29] 最大最小值
来源：http://hz.ydjk.org.cn/gtssmvsmxw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtkmcakzvo.html

[Q30] 分组统计
来源：http://hz.pengpengdd.cyou/gtqcdxzujp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtemdxhvmz.html

[Q31] 分组后过滤
来源：http://hz.kuanghao11.cn/gtbksybhqj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258888.top/gtmfhylcdx.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258.top/gtegvcuwvo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtaddqnxwe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtnbuxnuga.html

[Q33] 多列分组
来源：http://hz.cashguo.top/gttsrbztnd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenlongwang.top/gtcrochgiy.html

[Q34] 每组取第一条
来源：http://hz.sweek.top/gtpelmvwin.html

SELECT * FROM (
来源：http://hz.zhoulong.xyz/gtfrddnfsc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhijiandao.cn/gtwnlfbwlj.html

) t WHERE rn = 1;
来源：http://hz.wangdashe.top/gtbkwouqpr.html

[Q35] 内连接
来源：http://hz.wangdashe.top/gtuogpemuf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtwquldzkx.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtizgcnzto.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtelxhejpy.html

[Q37] 右连接
来源：http://hz.cucudq.cn/gtjzukloun.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shangyingyoupin.top/gtcjeafquh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.316326.xyz/gtxrajkakj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhengqikj.top/gtiwsvydye.html

[Q39] 自连接（查上下级）
来源：http://hz.haohaochexian.top/gtnnrsjetd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenjidiqi.icu/gtpototkmq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.52xcode.cn/gtpglvbyyu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gtalcrkste.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtiatkdrur.html

[Q41] 多表连接
来源：http://hz.ydjk.org.cn/gtcehuqcwz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtelmgvool.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtnvnzgbzd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.feifeiyinyue.top/gttlfkbrzh.html

[Q42] 连接条件附加过滤
来源：http://hz.zycfv.cn/gtbmzjhmod.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ppjwa.cn/gtywadwpes.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gtfgousmxv.html

[Q43] 标量子查询
来源：http://hz.ybcxt.top/gtiliqlnel.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtpqalrozb.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtethgbqaz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtvwwsucfc.html

[Q45] EXISTS 判断存在
来源：http://hz.sysykeji.top/gthmmhxopn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtzabwfflu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtfkmeezhd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtnssxkeeq.html

[Q47] 与平均值比较
来源：http://hz.ehwqpu.com/gtyjqkzskw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtcbilyywn.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtychvgnqd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtxfytkepv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuetiantiany.cn/gtorcdjejl.html

[Q49] 更新单行
来源：http://hz.zhiwuduotai.top/gtoayhyodq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtkzwaepkq.html

[Q50] 批量更新
来源：http://hz.jiagoushi.top/gtsnwcgutm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtwymfmstg.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gtykvomiwi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtmplbpgaq.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtzdscfyfr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtpkzvwztu.html

[Q53] 按条件删除
来源：http://hz.dashuyun.cn/gtwdjtfrzg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yangfankeji.com/gtqqejrqzl.html

[Q54] 清空表
来源：http://hz.yongpay.top/gtbxwmytos.html

TRUNCATE TABLE logs;
来源：http://hz.cheryme.top/gtfpqtbxov.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigfzy.top/gtyocqomww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtzjfavvmw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yvedp.cn/gtsprngtbc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daxiang520.top/gtttyhfpru.html

[Q57] 行号
来源：http://hz.zdqjudy.top/gtoxuttvzn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtwgnjsisn.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gtplyuciim.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cdnleiting.top/gtnpbhehzy.html

[Q59] 分组内累计
来源：http://hz.sysykeji.top/gtzjiusyqi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtpfakjbgc.html

[Q60] 取上一行 / 下一行
来源：http://hz.gaohongyu789.top/gtzxnikftd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtmemnjeqv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258888.top/gteqtkalek.html

[Q61] 移动平均
来源：http://hz.quarkkingdee.top/gtzsfwqfvx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtlpojwgei.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtisrsnqdo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtqsajmwzv.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtdcpsbltu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.svipenyu.cn/gtisntmhdg.html

[Q64] 提交事务
来源：http://hz.sysykeji.top/gtaifxqrwh.html

COMMIT;
来源：http://hz.xuanzx.com/gtfxevepun.html

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtdpftnszn.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtzbqazmla.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtkadyvgri.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xziqi.cn/gtxxklbevc.html

[Q67] 设置隔离级别
来源：http://hz.ivvv.top/gtutjyvjuz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgfzy.top/gtlyydrxtu.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtgsorieow.html

SAVEPOINT sp1;
来源：http://hz.iojbl.cn/gtuwiwfkqm.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gtpktxdkfb.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtkstwtssc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.birdmap.top/gtzlzxknjd.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtmkmxzujg.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gttvwgtzcg.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtekfcztfz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtdpqlzrzt.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtipjfdrwi.html

SHOW INDEX FROM users;
来源：http://hz.zycfv.cn/gtqqxgcflo.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtbdhicvhd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtmjqlwmfy.html

[Q74] 强制使用索引
来源：http://hz.yueranfly.top/gtzzoildce.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxinkj.top/gtrvwakyxk.html

[Q75] 日期格式化
来源：http://hz.zhoulong.xyz/gtvhbpqnsl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sufxvd.cn/gtuizfurkc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtonfdrozv.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtefurozfw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhixingplan.top/gtisygbatl.html

[Q77] 时间加减
来源：http://hz.chenlongwang.top/gtdsvcownh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.c1oappe.top/gtgyvsswnh.html

[Q78] 当前时间
来源：http://hz.316326.xyz/gthlwgpgkx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangdashe.top/gttmaiptui.html

[Q79] 字符串拼接
来源：http://hz.jqgufenzy.top/gtcdeydmno.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gtyowquaaq.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gtmlfucjji.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.iojbl.cn/gtetfqwkig.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtoqjmgrje.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxinkj.top/gtvetvuhvu.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtidgglumy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtjbdukumx.html

[Q83] 大小写转换
来源：http://hz.yueranfly.top/gtopiyzxih.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.birdmap.top/gtomlsogrj.html

[Q84] 去除首尾空格
来源：http://hz.zhijiandao.cn/gtgahnorib.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtsdfdqpxt.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtndmnxcwg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gtkahctrlh.html

[Q86] 读取 JSON 字段
来源：http://hz.zhijiandao.cn/gtnyprgeip.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtziudfkrt.html

[Q87] JSON 字段做条件
来源：http://hz.shzxlz.cn/gtyrcnlyno.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtydwxpsjv.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtqtkswcjn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hongshengwenyu.top/gtwygscspq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtpinpqbdy.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtuvpcqnyf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fzhhl.top/gtxbyaujsb.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtzfraggek.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.dianchejie.cn/gtqydcymgg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtteioyscv.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtdwyhdrxo.html

================================================================================
来源：http://hz.cdnleiting.top/gtcusxjouj.html

[R01] shebang 与严格模式
来源：http://hz.andypj.xyz/gtdazhcead.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtwzmghaas.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtnapqkorm.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtrapfafcr.html

name="Tom"; echo "$name"
来源：http://hz.guowangkeji.top/gtmjfinhdi.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtsgwrrsju.html

readonly PI=3.14
来源：http://hz.ybcxt.top/gtskvdkmko.html

[R04] 位置参数
来源：http://hz.snrcjt.cn/gtvnmzgrod.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cdnleiting.top/gttrxsuxds.html

[R05] 参数默认值
来源：http://hz.jianghu66.top/gtgsthmoff.html

name="${1:-default}"
来源：http://hz.xuetiantiany.cn/gtfzctolfu.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtizatrsfs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgufenzy.top/gtkizngphj.html

[R07] if 判断文件
来源：http://hz.yuanzhike.top/gtmflvbcbn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxinkj.top/gtcrespjws.html

[R08] 数值比较
来源：http://hz.zhongyouzk.top/gtgecodvgi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtawoejipl.html

[R09] 字符串比较
来源：http://hz.dashuyun.cn/gtrgcmidpb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxuanxn.top/gtujrdpodo.html

[R10] 正则匹配
来源：http://hz.tanke756.top/gtvolllame.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigfzy.top/gtugmyxcwy.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtlifiuxlr.html

case "$1" in
来源：http://hz.9152youxi.cn/gtanxdmjzc.html

start) echo "启动" ;;
来源：http://hz.pengpengdd.cyou/gtlvqyxopt.html

stop)  echo "停止" ;;
来源：http://hz.xylfe.cn/gtfzqciqon.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtyfnqbvun.html

esac
来源：http://hz.ivvv.top/gtkhkjuyyt.html

[R12] for 遍历文件
来源：http://hz.smart0.xyz/gtnrapyfff.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gtwjrxgzrq.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtkckyxiti.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fengsongda.top/gtysxjufgi.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtidyddpgp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gtlkcgrgvy.html

[R15] while 逐行读文件
来源：http://hz.ydzc1.top/gtbvhorxvv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtdsgbetql.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtggiggodv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.smart0.xyz/gtgrdbhmsc.html

[R17] 数组定义与取值
来源：http://hz.zhixingplan.top/gtyijxdezz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tanke756.top/gthojeytbm.html

[R18] 遍历数组
来源：http://hz.c1oappe.top/gtegrfgxin.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cashguo.top/gtbbjwunhu.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtsavqndiw.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtrthvefuc.html

[R20] 关联数组（字典）
来源：http://hz.dashuyun.cn/gtnogquudu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtnpuaxghr.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtdvfyjzqy.html

echo "${#s}"
来源：http://hz.guannengcc.top/gtdgpobhhz.html

[R22] 截取子串
来源：http://hz.mhx1999.top/gtjlsggctj.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtlevfntin.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtosyrmfyc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtrmunliva.html

[R24] 大小写转换
来源：http://hz.gaohongyu789.top/gtovrulecw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtgxzqbtgh.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtpbsgwjxi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtnbsytujf.html

[R26] 命令替换
来源：http://hz.yongpay.top/gtvkhbzlcu.html

now=$(date +%F); echo "$now"
来源：http://hz.ivvv.top/gteirhlhwt.html

[R27] 算术展开
来源：http://hz.zhongyouzk.top/gthrwlncqr.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gthukcizyr.html

[R28] 浮点运算
来源：http://hz.sufxvd.cn/gtkspsyrho.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtmesjaovx.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gtykksiifd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cashguo.top/gtemzeklig.html

[R30] 函数返回状态码
来源：http://hz.yj20258888.top/gtzsfjczez.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yonumen.top/gtgpnnlqng.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gtlaqzjdwf.html


<!-- 参考信息 -->