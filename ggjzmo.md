代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gtfmqwlidd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuetiantiany.cn/gtgzboobku.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guannengcc.top/gteigucktv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhoulong.xyz/gtswsgcnka.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtasvcfbuw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtpfdguzpm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gttqnvpqpf.html

Ruby: a == b
来源：http://hz.tanke756.top/gtlprsqbzk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gtujwgmvjy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangkeji.top/gtbefjcwnk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangshuangyany.cn/gtksfuwqln.html

PHP:  if (empty($x)) {}
来源：http://hz.zdqjudy.top/gtgokzreok.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhongyouzk.top/gtxedlzinh.html

TS:   if (x == null) {}
来源：http://hz.pengpengdd.cyou/gtrctvmbyo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtbzdqbflu.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gtdosxnfwu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sufxvd.cn/gthvzwpoax.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtgpqczkzx.html

[P07] 防抖与节流
来源：http://hz.wangdashe.top/gtkzmxubwc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.redwolf501.top/gtftpfgabd.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gtqblhodsd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtvydlwafr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtosyypdkt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jlsjyb.cn/gtetgvcrym.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yongpay.top/gtngzyyzsq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ivvv.top/gtpubjamzq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gtjzekopdz.html

[P08] 处理浮点精度问题
来源：http://hz.dianchejie.cn/gttsfasnsr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtmwvdbacn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tanke756.top/gtnbedxxtg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtisbjjjyz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhongyouzk.top/gthvmvdphz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.0kj1m.cn/gtduutppxq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtopuqvghr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhiwuduotai.top/gtjirwsrbb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ydzc1.top/gtelteczse.html

================================================================================
来源：http://hz.ydzc1.top/gtskasqena.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ybcxt.top/gtpdroyody.html

================================================================================
来源：http://hz.aibaodan.cn/gtoieprsdo.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtzmfttqwx.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gtgdgzpysy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtniriywgb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ybcxt.top/gtzwtjeqsp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtozenmyzs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtivdffzie.html

);
来源：http://hz.xuanzx.com/gttetzgyay.html

[Q02] 创建带外键的表
来源：http://hz.nwbrower.top/gtodthutux.html

CREATE TABLE orders (
来源：http://hz.cashguo.top/gtobwzizlq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtpimdruon.html

user_id INT NOT NULL,
来源：http://hz.andypj.xyz/gtnrtrskdr.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gtwnrbnayq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtypzifizc.html

);
来源：http://hz.mhx1999.top/gtkrjjsfga.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtdpiqtvhn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fzhhl.top/gtbmxcivxe.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtfcprmpqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhengqikj.top/gtbvamikrd.html

[Q05] 重命名列
来源：http://hz.zhongyouzk.top/gtgdokmahj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gogol.net.cn/gtxyvrlpqb.html

[Q06] 删除列
来源：http://hz.hysaishi.cn/gtfbtppqxl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gotoacloud.top/gtqnfrpnyy.html

[Q07] 删除表
来源：http://hz.pycfn.com/gtvygqglva.html

DROP TABLE IF EXISTS orders;
来源：http://hz.316326.xyz/gtkfirryor.html

[Q08] 创建普通索引
来源：http://hz.jianghu66.top/gtzcyftote.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtsofxouoy.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtzcmflmmx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtalxzfxfx.html

[Q10] 插入单行
来源：http://hz.zycfv.cn/gtsaahkhdj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gthgxltagr.html

[Q11] 一次插入多行
来源：http://hz.hongshengwenyu.top/gtqxwteivo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sweek.top/gtetxbfmcq.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtyjjhvabp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gotoacloud.top/gtqmuefikd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hysaishi.cn/gtgbrjckpj.html

[Q13] 忽略重复插入
来源：http://hz.meibo888.top/gtacybtsak.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cheryme.top/gtaymxudvz.html

[Q14] 存在则更新（upsert）
来源：http://hz.jiagoushi.top/gtwbtpzjnh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtvpnofgjb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydzc1.top/gtaxnvoahc.html

[Q15] 查询全部
来源：http://hz.cucudq.cn/gthaxsxziu.html

SELECT * FROM users;
来源：http://hz.chenlongwang.top/gtazwzwjcc.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gttxbbandv.html

SELECT id, name FROM users;
来源：http://hz.nanxuanxn.top/gtqptdnopb.html

[Q17] 条件查询
来源：http://hz.yj202588.top/gtwlvxirzp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtropxysee.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gtjdblvodf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtmmeduozm.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gthniabzbo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgfzy.top/gtqesgthsg.html

[Q20] IN 列表
来源：http://hz.haohaochexian.top/gtlbzeopas.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtpaxaihkh.html

[Q21] 空值判断
来源：http://hz.bjfxy.top/gtnmmozuit.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtkskrveol.html

[Q22] 排序
来源：http://hz.xuanzx.com/gtefpprwun.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hywenlv.cn/gtjyqdncnk.html

[Q23] 分页
来源：http://hz.hammf.cn/gtfkwptyin.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.0kj1m.cn/gtgvfbmspj.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtbyfriess.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtehtxkwqk.html

[Q25] 只取前 N 条
来源：http://hz.aibaodan.cn/gtkogsywcm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258888.top/gtlyjuowwa.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtfxbdrhcy.html

SELECT COUNT(*) FROM users;
来源：http://hz.jiagoushi.top/gtgsiewgol.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtlvuajtsu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ppjwa.cn/gtvxqjqaso.html

[Q28] 求和与平均
来源：http://hz.zhongyouzk.top/gtdgczwrpt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sweek.top/gtikaovdgq.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtqggkmxww.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtjltkvoxr.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gtzcuhxapw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtplsrktpr.html

[Q31] 分组后过滤
来源：http://hz.52xcode.cn/gtgrcoawcq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.9152youxi.cn/gtfiivghwv.html

[Q32] 分组拼接字符串
来源：http://hz.cheryme.top/gtrpapvxip.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtocyaxgju.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtmibwkjsp.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtnyyytmoa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zycfv.cn/gtflyuyfhk.html

[Q34] 每组取第一条
来源：http://hz.chenjidiqi.icu/gtkznqsmsp.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtvbnrktsq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.bjfxy.top/gtbblxeelu.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtgeicpell.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtcijlpbeh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtmpglwxln.html

[Q36] 左连接
来源：http://hz.jqgfzy.top/gtabrsxwdk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtgdfbcowc.html

[Q37] 右连接
来源：http://hz.aibaodan.cn/gtxvxmnmsy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.kuanghao11.cn/gtktuhckty.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daria6918.cn/gtugitqvtj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxuanxn.top/gtjnddmewx.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gtaigqeyis.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigfzy.top/gtrgtneubj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sweek.top/gtbghgbhzi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guowangkeji.top/gtewcewbkq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258888.top/gttxcdbktv.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gtgkztmagb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pycfn.com/gturinuftn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtqflcjqlt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.andypj.xyz/gtmrqbiaxj.html

[Q42] 连接条件附加过滤
来源：http://hz.guannengcc.top/gtvgajdjje.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtjlsyqpng.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cashguo.top/gtwbwywakc.html

[Q43] 标量子查询
来源：http://hz.snrcjt.cn/gtoozeyreb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gtbpzkstwe.html

[Q44] IN 子查询
来源：http://hz.cqqwz.cn/gtjhvcthbt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtgoavwhjj.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtyqzufuli.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtzlcapoud.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xylfe.cn/gtlkzdjerr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtcjqnnupf.html

[Q47] 与平均值比较
来源：http://hz.52xcode.cn/gthcbaqgym.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtnhwrbqyc.html

[Q48] CTE 公用表表达式
来源：http://hz.vqdsnc.cn/gtslguganu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.haohaochexian.top/gtqeiefkok.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pycfn.com/gtajtflodk.html

[Q49] 更新单行
来源：http://hz.daxiang520.top/gtgfvylemw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtqgwipvaj.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gtpawyvbxj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daxiang520.top/gtgywzzddn.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gtgnpkvlnd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yangfankeji.com/gtphjiymsg.html

[Q52] 删除指定行
来源：http://hz.52xcode.cn/gtplnjmrxc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtunqcrumg.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtsiptrjrg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dashuyun.cn/gtqixkimer.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtqrihbvkj.html

TRUNCATE TABLE logs;
来源：http://hz.shangyingyoupin.top/gtxbjekfkk.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gtipuqkzii.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.redwolf501.top/gtejxwyjlr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hammf.cn/gtxrunhfyr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhengqikj.top/gtmipgrtub.html

[Q57] 行号
来源：http://hz.daxiang520.top/gteugpuwgu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gogol.net.cn/gtvkjftiht.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gterbytiyn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daria6918.cn/gtckjsubyi.html

[Q59] 分组内累计
来源：http://hz.hysaishi.cn/gtojodafst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guannengcc.top/gtjztcvhjv.html

[Q60] 取上一行 / 下一行
来源：http://hz.dashuyun.cn/gtgpfzvfwh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.smart0.xyz/gtzbwydzzv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtostlnkbo.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gtpgtsvaup.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtahwquauy.html

[Q62] 分组占比
来源：http://hz.xuanzx.com/gtmwxlwukb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtgtxhmjzr.html

[Q63] 开启事务
来源：http://hz.shanyushiyangtech.top/gtleuurwbe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtjddiwqus.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gtugfezhlf.html

COMMIT;
来源：http://hz.guannengcc.top/gtxqyjcbzn.html

[Q65] 回滚事务
来源：http://hz.svipenyu.cn/gtygaaldzp.html

ROLLBACK;
来源：http://hz.nwbrower.top/gtftbpiskh.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gtjujydnoe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gthegyltlp.html

[Q67] 设置隔离级别
来源：http://hz.sufxvd.cn/gtqjrwzsaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sysykeji.top/gtjyhgefug.html

[Q68] 保存点
来源：http://hz.guannengcc.top/gtpjyvwlya.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtueqkljsd.html

ROLLBACK TO sp1;
来源：http://hz.hysaishi.cn/gtsxuteesr.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtbilbenud.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.haohaochexian.top/gtecpybqcm.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtmvysmctq.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtyocbxekw.html

[Q71] 查看建表语句
来源：http://hz.gotoacloud.top/gtsxgzapif.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydzc1.top/gtulpkribw.html

[Q72] 查看索引
来源：http://hz.sufxvd.cn/gtcahlokcd.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtnmxfnogd.html

[Q73] 查看表状态
来源：http://hz.yj20258888.top/gtudhwxnzg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jianghu66.top/gtywygdvtc.html

[Q74] 强制使用索引
来源：http://hz.cqqwz.cn/gtsintoknj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtktafazzf.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtzrgrlxbd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jyoumei.cn/gthlrmyqze.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gttsiearho.html

[Q76] 按天统计
来源：http://hz.zhixingplan.top/gtrsztrdla.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtbtsppxem.html

[Q77] 时间加减
来源：http://hz.ppjwa.cn/gtqjyosjxy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangshuangyany.cn/gtwujdmeke.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtlwyqnsyi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.52xcode.cn/gtpsuzdaxl.html

[Q79] 字符串拼接
来源：http://hz.cashguo.top/gtvztearuu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gtgpprjsky.html

[Q80] 字符串截取
来源：http://hz.quarkkingdee.top/gtzhrerrvv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guowangkeji.top/gtyypuracf.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtlnpamqgd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtqwbkqqoc.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtbmobpgpa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtawdkvwsz.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtxtqurmpg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtbilqbzta.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gthohithqq.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtkkzbydeo.html

[Q85] 数值取整
来源：http://hz.sweek.top/gtqhuipbjf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtadbtcndi.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtmjlotiqu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gtqzvgenba.html

[Q87] JSON 字段做条件
来源：http://hz.jyoumei.cn/gtawuqjffk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gtfjrvhtbl.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhiwuduotai.top/gtqnygtepd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gotoacloud.top/gtwsbfqdgi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shuidangran.top/gtmgkmxlwn.html

[Q89] 判断表是否存在
来源：http://hz.nanxinkj.top/gtlvvulouc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtviktkjow.html

[Q90] 生成序号列
来源：http://hz.yangfankeji.com/gtlnxnoydv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtzzphjork.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmrunhpqu.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtzivgpkju.html

================================================================================
来源：http://hz.aizwys.cn/gtktizmmrp.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtntonaunm.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtnoxwvwxw.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gtkcoozvfj.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtvcssmlhg.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtkkjwbjfd.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtqsmsfmpy.html

readonly PI=3.14
来源：http://hz.ybcxt.top/gthapilanb.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtdcuecnde.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gtjhprpqaq.html

[R05] 参数默认值
来源：http://hz.gogol.net.cn/gtucwexcbq.html

name="${1:-default}"
来源：http://hz.yuanzhike.top/gtusxbdldq.html

[R06] 判断命令是否存在
来源：http://hz.jqgfzy.top/gtkjzheorm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.redwolf501.top/gtfdcjffnc.html

[R07] if 判断文件
来源：http://hz.yj20258.top/gtjzaqewqa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.iojbl.cn/gtchfgrmvc.html

[R08] 数值比较
来源：http://hz.hnxiangtu.top/gtbwsehpmb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ybcxt.top/gtrtteqjdu.html

[R09] 字符串比较
来源：http://hz.guowangkeji.top/gtqaenhhvj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhongyouzk.top/gtflfiqgyn.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtjvjuaheh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.havefunace.top/gthxxqarxc.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtaxdhkbvt.html

case "$1" in
来源：http://hz.zycfv.cn/gteociitia.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtkivuhgif.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtvrcpjutr.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gtfuiijxkf.html

esac
来源：http://hz.xuetiantiany.cn/gtgzwubnry.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtoniwxart.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daxiang520.top/gttcuqltzm.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gtcedhikuz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sxryk.cn/gtkzirifwf.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gtzdszygoa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtxhbkjtva.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangkeji.top/gteikzpwom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnqzz.top/gtfgsqsqvb.html

[R16] until 等待条件
来源：http://hz.yuxming.cn/gtxygcmiiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xingfuxueyuan.xyz/gtjockvzdx.html

[R17] 数组定义与取值
来源：http://hz.jyoumei.cn/gtklogzvuu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gtjmefvkwj.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtvvqilitb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxuanxn.top/gtxlgbqmta.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtgcciqtpr.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtfoipjrxk.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gtrkytohao.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtdlzdyebs.html

[R21] 字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtjyhhhkzc.html

echo "${#s}"
来源：http://hz.xingfuxueyuan.xyz/gtewdefdsa.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtesxfmzcc.html

echo "${s:0:5}"
来源：http://hz.ivvv.top/gtqntzbbjo.html

[R23] 字符串替换
来源：http://hz.9152youxi.cn/gtwobtyopu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xinyue.icu/gtanxpfwrg.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtwfrteqty.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.vqdsnc.cn/gtcrxlbarb.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtvexsauve.html


<!-- 参考信息 -->