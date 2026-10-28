代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtagyymhom.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtopyjromu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtumdivgow.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtsylynuxa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gttfiyxely.html

Go:   len(arr);  len(m)
来源：http://hz.0kj1m.cn/gtivbgddfs.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gtfdahyhcd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.fzhhl.top/gtkrjebybe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gteybrlrgp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtlmzwfprq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtjkfedchg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shzxlz.cn/gttrtxpkqb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtjrobdmug.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yongpay.top/gtffvsnytc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cucudq.cn/gtyxyyblwn.html

Ruby: a == b
来源：http://hz.yonumen.top/gtlxtrosdz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gtqgdmefcm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gthpzhhmak.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtuhhqlubb.html

PHP:  if (empty($x)) {}
来源：http://hz.redwolf501.top/gtkzktmlvs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.havefunace.top/gtiddfnbah.html

TS:   if (x == null) {}
来源：http://hz.sxryk.cn/gtlpyueakj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gthmqtafhl.html

Go:   if x == nil {}
来源：http://hz.gzhubu.top/gtrldmgeke.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ppjwa.cn/gtldaarloq.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtdlwrxghy.html

[P07] 防抖与节流
来源：http://hz.kuanghao11.cn/gtotlarlgn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jqgfzy.top/gttsqmeyjr.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtzdvfrlnu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtirmruraf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtqpjaviau.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tanke756.top/gtwebtuund.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangtech.top/gtsijvomrj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtgeyjbqzk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuetiantiany.cn/gthgiojsli.html

[P08] 处理浮点精度问题
来源：http://hz.quarkkingdee.top/gtfmzvhhzc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yanxiufei.cn/gthybfkega.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.c1oappe.top/gtgbhamrlw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.0kj1m.cn/gtgmicktjl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxuanxn.top/gtmuggdpgl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.havefunace.top/gtwcsxguyk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.haohaochexian.top/gtxuukrort.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.meibo888.top/gtjsnjtlmw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tian-w.cn/gtwrkrzdmw.html

================================================================================
来源：http://hz.iojbl.cn/gtggccjvso.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zycfv.cn/gtcqkaswub.html

================================================================================
来源：http://hz.sufxvd.cn/gthlcbwpaj.html

[Q01] 创建表
来源：http://hz.svipenyu.cn/gtalytctro.html

CREATE TABLE users (
来源：http://hz.ywan-chungtsiang.top/gtcuraftbp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gthvhgcljz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gaohongyu789.top/gtzsdjyzfw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuxming.cn/gtmuwnzcaj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigfzy.top/gtzdooetzf.html

);
来源：http://hz.wangdashe.top/gtaqzjmfll.html

[Q02] 创建带外键的表
来源：http://hz.birdmap.top/gtkvepwnzf.html

CREATE TABLE orders (
来源：http://hz.hnqzz.top/gtmwamzjpp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtmlstbzvw.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gteyvyaiva.html

amount DECIMAL(10, 2),
来源：http://hz.hnqzz.top/gtujhxadfz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gtvkuqnqkb.html

);
来源：http://hz.feifeiyinyue.top/gtakzllmmm.html

[Q03] 增加列
来源：http://hz.quarkkingdee.top/gtrptpgzfx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtwwjhdjze.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtaiddaufk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhixingplan.top/gtotnrwwzb.html

[Q05] 重命名列
来源：http://hz.gaohongyu789.top/gtcilhopfj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tian-w.cn/gtdphdbwro.html

[Q06] 删除列
来源：http://hz.316326.xyz/gttfoceyju.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gtxxodbppd.html

[Q07] 删除表
来源：http://hz.havefunace.top/gtycanwjue.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhengqikj.top/gtbsmxkwbm.html

[Q08] 创建普通索引
来源：http://hz.jqgfzy.top/gtudstjsdc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtnwcfnwmu.html

[Q09] 创建唯一索引
来源：http://hz.hnqzz.top/gtdraxtogs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gtrhzafmjo.html

[Q10] 插入单行
来源：http://hz.zhijiandao.cn/gtgxbnpnhs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gttojgogyr.html

[Q11] 一次插入多行
来源：http://hz.daria6918.cn/gttfsukpeo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hammf.cn/gtovujlugs.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gtjxellzro.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtkcuekfzx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtdxynchdk.html

[Q13] 忽略重复插入
来源：http://hz.gzhubu.top/gtcbqsxcqn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangkeji.top/gtijuuftkl.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gtxgnmgkzd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zycfv.cn/gtsiilpxlz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtskacbpla.html

[Q15] 查询全部
来源：http://hz.zhengqikj.top/gtppjrhwlu.html

SELECT * FROM users;
来源：http://hz.ydjk.org.cn/gtasqygmva.html

[Q16] 查询指定列
来源：http://hz.zhengqikj.top/gtssjdpytv.html

SELECT id, name FROM users;
来源：http://hz.guowangkeji.top/gtbtznqgij.html

[Q17] 条件查询
来源：http://hz.jyoumei.cn/gtbdqmjlwj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cdnleiting.top/gtrpzsgnhp.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gtgqfrgwfo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgufenzy.top/gtjumhuopm.html

[Q19] 范围查询
来源：http://hz.kuanghao11.cn/gtfrtbuohn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cucudq.cn/gtityzfcfc.html

[Q20] IN 列表
来源：http://hz.c1oappe.top/gtgtwpqwon.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zycfv.cn/gtirhqncwv.html

[Q21] 空值判断
来源：http://hz.chenzaomai.com/gtvtwdowny.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtvtiuqtcz.html

[Q22] 排序
来源：http://hz.shuidangran.top/gtcoymkkol.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhixingplan.top/gtkldeznnq.html

[Q23] 分页
来源：http://hz.meibo888.top/gtzmevbfwh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtssvjwwjk.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gtsjabcltv.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtgpzkzlsb.html

[Q25] 只取前 N 条
来源：http://hz.0kj1m.cn/gtxafxkghd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtpvahxpoy.html

[Q26] 计数
来源：http://hz.snrcjt.cn/gtgmrernaj.html

SELECT COUNT(*) FROM users;
来源：http://hz.sweek.top/gtiwysxknd.html

[Q27] 条件计数
来源：http://hz.daxiang520.top/gtwqfgvule.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jqgufenzy.top/gtumrraivm.html

[Q28] 求和与平均
来源：http://hz.jqgufenzy.top/gtsrqeefzf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtfdmvxjyq.html

[Q29] 最大最小值
来源：http://hz.316326.xyz/gtkgnvhbvx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cucudq.cn/gtyyokpgdu.html

[Q30] 分组统计
来源：http://hz.yj20258888.top/gtibrtbehq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtnhkkkzmi.html

[Q31] 分组后过滤
来源：http://hz.ybcxt.top/gtysqjegqf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj202588.top/gtcmechdxe.html

[Q32] 分组拼接字符串
来源：http://hz.ivvv.top/gticzbpeln.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtahhrzklb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.c1oappe.top/gtokmjweqh.html

[Q33] 多列分组
来源：http://hz.jinqigfzy.top/gtpuulfklt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtkqvrlnmp.html

[Q34] 每组取第一条
来源：http://hz.dashuyun.cn/gtgateozsl.html

SELECT * FROM (
来源：http://hz.yj202588.top/gtazewpsun.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtguraamba.html

) t WHERE rn = 1;
来源：http://hz.iojbl.cn/gtozimngtx.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gtjuipniaa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gthvodcrsv.html

[Q36] 左连接
来源：http://hz.shangyingyoupin.top/gtuxcoardm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtmkscwvbh.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gttptucukb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinyuanbaomall.cn/gtnysbhqqm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gtlixzcdss.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hammf.cn/gtqrezgezx.html

[Q39] 自连接（查上下级）
来源：http://hz.ydjk.org.cn/gticdrfmfu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xinyue.icu/gtzxdwpicl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtpduakosm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sweek.top/gtprkaooti.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.andypj.xyz/gtonxedvpt.html

[Q41] 多表连接
来源：http://hz.gaohongyu789.top/gtdfmafrcl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtdawmnhbv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ehwqpu.com/gtpjqniryt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ybcxt.top/gtsyulojxq.html

[Q42] 连接条件附加过滤
来源：http://hz.ywan-chungtsiang.top/gtxgtwnaag.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtxorwihhc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtpyawclgw.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtiembqilf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yonumen.top/gtsfqitfou.html

[Q44] IN 子查询
来源：http://hz.zhoulong.xyz/gtkiznvdvo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fzhhl.top/gtlmrmoihz.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gthrycpbqz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtskobddyv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhaomingkeji.xyz/gtfwpmbevf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jlsjyb.cn/gtgwzebhsn.html

[Q47] 与平均值比较
来源：http://hz.guannengcc.top/gtpjojsexd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cucudq.cn/gtrmkzgelg.html

[Q48] CTE 公用表表达式
来源：http://hz.quarkkingdee.top/gthxxhjnco.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cucudq.cn/gteccfhjqn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gtxzdpvjnz.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gtwzmcdzhk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aizwys.cn/gtghyfkgha.html

[Q50] 批量更新
来源：http://hz.0kj1m.cn/gtdajrmuxi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtpkzcrkkx.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gtmxjbojwv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgufenzy.top/gtjqkulhne.html

[Q52] 删除指定行
来源：http://hz.xuanzx.com/gtzyiifyne.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtocesludm.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtsbirvfpo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gthabscusi.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtvnrpiimc.html

TRUNCATE TABLE logs;
来源：http://hz.gotoacloud.top/gtjrkqhitz.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtfidcaiue.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.0kj1m.cn/gtrbshfngp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuxming.cn/gtidyxsplg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gthhxgbfqm.html

[Q57] 行号
来源：http://hz.wangshuangyany.cn/gtrciaufvc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtfbqieqsy.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtkwlbrhtv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nwbrower.top/gtcdgatttd.html

[Q59] 分组内累计
来源：http://hz.feifeiyinyue.top/gtfbtqncts.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtceelwmok.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtgtshdycl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtedenyzxz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.svipenyu.cn/gtzmywwfcp.html

[Q61] 移动平均
来源：http://hz.chenlongwang.top/gtdbngpotd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtkeyfzffk.html

[Q62] 分组占比
来源：http://hz.aibaodan.cn/gttnuhnbrn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtfnjhwzel.html

[Q63] 开启事务
来源：http://hz.jqgufenzy.top/gtrcwfxqdy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhixingplan.top/gtwwrbjymk.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtzgvaotqi.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gtrpktvkid.html

[Q65] 回滚事务
来源：http://hz.sxryk.cn/gteuysdqch.html

ROLLBACK;
来源：http://hz.nanxuanxn.top/gtjkvachdr.html

[Q66] 行锁查询
来源：http://hz.yj202588.top/gthwasahoa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gtshbedwji.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtwcbjngnh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtijydwhqw.html

[Q68] 保存点
来源：http://hz.gogol.net.cn/gtjrplsnkc.html

SAVEPOINT sp1;
来源：http://hz.snrcjt.cn/gtdnafhzvh.html

ROLLBACK TO sp1;
来源：http://hz.fzhhl.top/gthiuvhgao.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtbrujfvzn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtcdgtduny.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gttylfjglg.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtqyxzysvd.html

[Q71] 查看建表语句
来源：http://hz.guowangkeji.top/gttvwzihxm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtddmucdab.html

[Q72] 查看索引
来源：http://hz.jianghu66.top/gtesjzymjo.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gtxmrviyeb.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtoilxqbro.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuxming.cn/gtjxcuivpz.html

[Q74] 强制使用索引
来源：http://hz.zhijiandao.cn/gtnppmjciy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.c1oappe.top/gtmncfussn.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtqzckbner.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtuxjtcnsq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tian-w.cn/gtjorupfem.html

[Q76] 按天统计
来源：http://hz.ppjwa.cn/gtpnymhijk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.316326.xyz/gtcwldaytf.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtkurfnwoa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gtjieseugi.html

[Q78] 当前时间
来源：http://hz.wangdashe.top/gtralnwhtb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.svipenyu.cn/gtjprqxdiu.html

[Q79] 字符串拼接
来源：http://hz.haohaochexian.top/gtqnxvecli.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ybcxt.top/gthuoneqfb.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gtaqxzeikm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtbgbuaych.html

[Q81] 字符串替换
来源：http://hz.mhx1999.top/gtzgcyuuyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jlsjyb.cn/gtbjluvnuv.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtszolepwe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtewulnjwx.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtylmrspgp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtvvzarypb.html

[Q84] 去除首尾空格
来源：http://hz.cashguo.top/gtuxqtrqdm.html

SELECT TRIM(name) FROM users;
来源：http://hz.gaohongyu789.top/gtlajwfkcu.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gtacnckuyh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtofmpodtj.html

[Q86] 读取 JSON 字段
来源：http://hz.ivvv.top/gtrjskviia.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jiagoushi.top/gtimxnabqk.html

[Q87] JSON 字段做条件
来源：http://hz.ppjwa.cn/gtczxtwdwa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tian-w.cn/gtfdrrkfgv.html

[Q88] 行转列（条件聚合）
来源：http://hz.aizwys.cn/gtylmeqomk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258.top/gtrarxytxj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtctspwjdt.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtgarsqnad.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydzc1.top/gtyyntfbko.html

[Q90] 生成序号列
来源：http://hz.zycfv.cn/gtaradpevl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shzxlz.cn/gtujocyrxo.html

================================================================================
来源：http://hz.jinqigufen.top/gtmizihzex.html

R. Bash 专题
来源：http://hz.nanxinkj.top/gtejfczkuz.html

================================================================================
来源：http://hz.bjfxy.top/gtuotxhfas.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtadtyqnmq.html

#!/usr/bin/env bash
来源：http://hz.cdnleiting.top/gtovgamzku.html

set -euo pipefail
来源：http://hz.bjfxy.top/gthafnyaqx.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtdffvmlbu.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gthqvebqwt.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtcmpanssc.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtcukgubst.html

[R04] 位置参数
来源：http://hz.jinqigfzy.top/gtysoeipge.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtsqkvvham.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtdzslurzb.html

name="${1:-default}"
来源：http://hz.shangyingyoupin.top/gthypnanwe.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtstnaophp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aibaodan.cn/gteawapbrz.html

[R07] if 判断文件
来源：http://hz.c1oappe.top/gtktaodkzf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shzxlz.cn/gtjecagfmj.html

[R08] 数值比较
来源：http://hz.xziqi.cn/gtzxwzgsup.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pengpengdd.cyou/gtbjkmilwx.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtlfxousns.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhaomingkeji.xyz/gtdsziqxlg.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtqyxwzvsb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenjidiqi.icu/gtdgptxabe.html

[R11] case 多分支
来源：http://hz.zhoulong.xyz/gtlgfgebey.html

case "$1" in
来源：http://hz.jqgufenzy.top/gtqrtmkskw.html

start) echo "启动" ;;
来源：http://hz.jinyuanbaomall.cn/gtedivhgzz.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtnruwfeya.html

*)     echo "未知命令" ;;
来源：http://hz.yongpay.top/gtjjutxezx.html

esac
来源：http://hz.xinyue.icu/gtweoihwqu.html

[R12] for 遍历文件
来源：http://hz.vqdsnc.cn/gtibpwfcdr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ivvv.top/gttyeiaahc.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtolfyicek.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtvwffypqr.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gtacrnpkng.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtoumgvgiz.html

[R15] while 逐行读文件
来源：http://hz.mhx1999.top/gthcvctawt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.haohaochexian.top/gtlkzrhtgh.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtyukkzeld.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gogol.net.cn/gtqngariaf.html

[R17] 数组定义与取值
来源：http://hz.yanxiufei.cn/gtndbcmrpx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.kuanghao11.cn/gttzbfbyeb.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtaerrkkzl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yueranfly.top/gtpndchail.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtmsiuoenh.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gtcbcfdnmc.html

[R20] 关联数组（字典）
来源：http://hz.jqgfzy.top/gtxqgiqwfk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yongpay.top/gtyfrfmcas.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtjhmbiwpm.html


<!-- 参考信息 -->