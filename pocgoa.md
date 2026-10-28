代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yongpay.top/gtemxuxfai.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtqpngsxif.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtuhougwxg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gtppxkrdsn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hongshengwenyu.top/gtffoludoc.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtwwhjagle.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtynthsglz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shuidangran.top/gtdjfoapga.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gtbamfidrt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gtjhfinzli.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenjidiqi.icu/gtrleltfrw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj202588.top/gtvdlcztmg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtvnhrwsgo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gthvowhbxk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ivvv.top/gtwfxxwxoe.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtkxxhzalb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigfzy.top/gtmwfbimft.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.guannengcc.top/gtepwnceir.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258.top/gtmwvwwafq.html

PHP:  if (empty($x)) {}
来源：http://hz.9152youxi.cn/gtxiaxpunv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuxming.cn/gtqtzecspk.html

TS:   if (x == null) {}
来源：http://hz.wangdashe.top/gtiqbtkipw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtjbjadsfm.html

Go:   if x == nil {}
来源：http://hz.birdmap.top/gtdnosstmz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sufxvd.cn/gtcrhbapcl.html

C#:   if (x is null) {}
来源：http://hz.zhengqikj.top/gtmloqnthj.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtqrlgwlwl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daxiang520.top/gtgntcxjbd.html

PHP:  // 手写时间戳比较
来源：http://hz.zhoulong.xyz/gtxgnbshwo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtyckyntrg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtvwpdcgzo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenzaomai.com/gtlaaphyqd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gttllajrgj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gttucwwvem.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxuanxn.top/gteeuekavx.html

[P08] 处理浮点精度问题
来源：http://hz.hnxiangtu.top/gtlaqhfgqu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenjidiqi.icu/gtzxheflbz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydzc1.top/gtdydhrldm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtzvqpolhz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xylfe.cn/gtbobxvfcy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jyoumei.cn/gtgcjdbjrr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtdhiistyx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.havefunace.top/gtoncgpglk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gotoacloud.top/gtzfsvvuad.html

================================================================================
来源：http://hz.xziqi.cn/gtfndsrjnb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gtsztcxstj.html

================================================================================
来源：http://hz.quarkkingdee.top/gtuznvvscw.html

[Q01] 创建表
来源：http://hz.redwolf501.top/gtnpulizpd.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gtdshslvgq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtmukafuip.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgfzy.top/gtbokajsca.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cucudq.cn/gtmbylhtry.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtqsfdpqhx.html

);
来源：http://hz.svipenyu.cn/gtxznikbvp.html

[Q02] 创建带外键的表
来源：http://hz.yuxming.cn/gtqbevvnem.html

CREATE TABLE orders (
来源：http://hz.cheryme.top/gtodtzwmjs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhongyouzk.top/gtbtqyamrz.html

user_id INT NOT NULL,
来源：http://hz.sysykeji.top/gtrmppjmpv.html

amount DECIMAL(10, 2),
来源：http://hz.gogol.net.cn/gtohkhzlex.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtxkbjmpcd.html

);
来源：http://hz.ehwqpu.com/gtgvdbqszw.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtpnjdreyt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fzhhl.top/gtyenjbaoq.html

[Q04] 修改列类型
来源：http://hz.shuidangran.top/gteooamzka.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuanzhike.top/gtizyfqxes.html

[Q05] 重命名列
来源：http://hz.aizwys.cn/gtaaunzzej.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shangyingyoupin.top/gtbnatktbn.html

[Q06] 删除列
来源：http://hz.yanxiufei.cn/gtredjftik.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258.top/gtsmlhkevj.html

[Q07] 删除表
来源：http://hz.svipenyu.cn/gtdcathxpw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenzaomai.com/gthcsnbobx.html

[Q08] 创建普通索引
来源：http://hz.nanxinkj.top/gtzxgwzoqk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtkbqitkhl.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtpnntqgbd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daria6918.cn/gtfedgmblk.html

[Q10] 插入单行
来源：http://hz.ydzc1.top/gtiqdyztym.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gtgmmeovgk.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gtklqtwwbt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.smart0.xyz/gtqfxvscos.html

[Q12] 插入后取自增 ID
来源：http://hz.ywan-chungtsiang.top/gteojdjtaq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtzylhitpp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangdashe.top/gtykmdpgdn.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtkrlnceqk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gtlghgrecs.html

[Q14] 存在则更新（upsert）
来源：http://hz.gotoacloud.top/gtthhlqpxe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sysykeji.top/gtvvbjjycp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aibaodan.cn/gtpuxalqre.html

[Q15] 查询全部
来源：http://hz.chenlongwang.top/gtivgqgkwh.html

SELECT * FROM users;
来源：http://hz.wangdashe.top/gtwssqwfhe.html

[Q16] 查询指定列
来源：http://hz.bjfxy.top/gtzycodyyn.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtdakypwie.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtjxcydhfg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtiqiiqibl.html

[Q18] 模糊匹配
来源：http://hz.yuxming.cn/gtpvjdglur.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yongpay.top/gtrdlmllsi.html

[Q19] 范围查询
来源：http://hz.nanxuanxn.top/gtpvqeggsg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ivvv.top/gtjoeqcwuz.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtjryprauy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gtimkukhlm.html

[Q21] 空值判断
来源：http://hz.sxryk.cn/gtuxhwtpvw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daria6918.cn/gtoeqezoyv.html

[Q22] 排序
来源：http://hz.yj202588.top/gtctisxysw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtlwvqltyu.html

[Q23] 分页
来源：http://hz.zdqjudy.top/gtwgkhdhbz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtnszkkrjv.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtugsarpza.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gtgvwfkpcw.html

[Q25] 只取前 N 条
来源：http://hz.hnqzz.top/gtvbthupls.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gtuccikeqi.html

[Q26] 计数
来源：http://hz.hfpthk.cn/gtunltfyyd.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtwtwvwlfa.html

[Q27] 条件计数
来源：http://hz.snrcjt.cn/gtkpmjdydj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gtkiisrief.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtxgrrtfxm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtiefdiojp.html

[Q29] 最大最小值
来源：http://hz.zhongyouzk.top/gtwtspmrnt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuetiantiany.cn/gtcpsmlwax.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtatwrvern.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtvmxropkc.html

[Q31] 分组后过滤
来源：http://hz.cqqwz.cn/gtjzgzfnwz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gogol.net.cn/gtxinqafsb.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gtgororrov.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtooywwtoo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.havefunace.top/gtwhutnioa.html

[Q33] 多列分组
来源：http://hz.yj202588.top/gthtxgdzfh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtivhfdrfd.html

[Q34] 每组取第一条
来源：http://hz.chenjidiqi.icu/gtqjmkuekx.html

SELECT * FROM (
来源：http://hz.yanxiufei.cn/gtfdnqwoex.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtvxyjutmg.html

) t WHERE rn = 1;
来源：http://hz.xuetiantiany.cn/gtjsibigib.html

[Q35] 内连接
来源：http://hz.sxryk.cn/gtuthtqmoj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gturfjjemh.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtpzwohlpj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtrwwkuwys.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtupdpfnca.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fzhhl.top/gtcbcjhvki.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.smart0.xyz/gtdzmhxfcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtclwwwzvv.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtmcqorbmb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hysaishi.cn/gtxynoobjt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gteqxgivlj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jianghu66.top/gttgsushbm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gteepekiee.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gtmyjlzeus.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtlprcizbe.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gthdghkoba.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dianchejie.cn/gtbzmwpzsp.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gtufjiupje.html

SELECT u.name, o.amount FROM users u
来源：http://hz.birdmap.top/gtmlnhvqzq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtulukpbmx.html

[Q43] 标量子查询
来源：http://hz.feifeiyinyue.top/gtddsksqju.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhaomingkeji.xyz/gtdiqaegsz.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtyvwxselh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pycfn.com/gtsaaewlou.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtnmztfyec.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gteawkihac.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zycfv.cn/gtojxrhcbv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtnzafrarw.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangtech.top/gtmntsqtdi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yangfankeji.com/gtjzkjamep.html

[Q48] CTE 公用表表达式
来源：http://hz.zhongyouzk.top/gtpeqbbkcq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xylfe.cn/gtcsjvdjeo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aizwys.cn/gtgtbhzmqr.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtxpcqtthz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gtpjsipzui.html

[Q50] 批量更新
来源：http://hz.cashguo.top/gtbewribxc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pycfn.com/gtcpqhsaft.html

[Q51] 用子查询更新
来源：http://hz.xylfe.cn/gtzrogxaom.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cheryme.top/gtleunefpy.html

[Q52] 删除指定行
来源：http://hz.dianchejie.cn/gtgfyrmbif.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtkojanmfh.html

[Q53] 按条件删除
来源：http://hz.316326.xyz/gtnmbcpzoi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yueranfly.top/gtulkoxpsy.html

[Q54] 清空表
来源：http://hz.zhaomingkeji.xyz/gtrfihjzzf.html

TRUNCATE TABLE logs;
来源：http://hz.cheryme.top/gtlygyniyn.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtinoryagf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhoulong.xyz/gtenwdsnzt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtxebucert.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.feifeiyinyue.top/gtzjnssvoy.html

[Q57] 行号
来源：http://hz.sufxvd.cn/gtultibbgi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxinkj.top/gtudaevkxk.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtgdlxdnaq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtqsgcuoob.html

[Q59] 分组内累计
来源：http://hz.hywenlv.cn/gtiiofazto.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gtxnzqjors.html

[Q60] 取上一行 / 下一行
来源：http://hz.0kj1m.cn/gtrknaorlm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.birdmap.top/gtncuswgoh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.mhx1999.top/gtasyjsszg.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gtjeuqgwkk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtwbgqknfa.html

[Q62] 分组占比
来源：http://hz.jianghu66.top/gtecqemjwm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtxixychkv.html

[Q63] 开启事务
来源：http://hz.jinqigufen.top/gtpzkpiboj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gtapatcxxg.html

[Q64] 提交事务
来源：http://hz.chenlongwang.top/gtmzpgvxrz.html

COMMIT;
来源：http://hz.ydzc1.top/gtxtnqmhal.html

[Q65] 回滚事务
来源：http://hz.daria6918.cn/gtvaqvskyp.html

ROLLBACK;
来源：http://hz.gaohongyu789.top/gtqrcelyco.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtilvmxawa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtosmedwrb.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtgbwsgife.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shangyingyoupin.top/gtsrcealwd.html

[Q68] 保存点
来源：http://hz.gogol.net.cn/gtxpkyvriz.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gthdehjkpb.html

ROLLBACK TO sp1;
来源：http://hz.xuetiantiany.cn/gtohindbqy.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtcwjokynk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhiwuduotai.top/gtofaoxues.html

[Q70] 更新统计信息
来源：http://hz.jyoumei.cn/gtqcsoksnx.html

ANALYZE TABLE users;
来源：http://hz.smart0.xyz/gtjayjdczv.html

[Q71] 查看建表语句
来源：http://hz.hywenlv.cn/gtprbjsxlz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuetiantiany.cn/gtwskvocnl.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtykijhhlj.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtrpudepuq.html

[Q73] 查看表状态
来源：http://hz.hfpthk.cn/gtpveozpmx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hfpthk.cn/gtkyvaxleb.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtyibuihts.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.kuanghao11.cn/gtzznfguxv.html

[Q75] 日期格式化
来源：http://hz.yuxming.cn/gtwxwnsgdr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pycfn.com/gtmmkejlpa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jianghu66.top/gtglcgqrei.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gtsnoqpgup.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zycfv.cn/gtuwomizcc.html

[Q77] 时间加减
来源：http://hz.cheryme.top/gtwbhxbcfc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gthpvrhxzj.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtluywufsv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtfzswrcih.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtjlrwltyq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pengpengdd.cyou/gtgobqbcqn.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gtckagwhkm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtrphmepqa.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtlguqdirf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtlvcypvlq.html

[Q82] 字符长度与字节长度
来源：http://hz.andypj.xyz/gtmpdpseoc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtlbgumjbc.html

[Q83] 大小写转换
来源：http://hz.meibo888.top/gtpvfustnj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.birdmap.top/gtqyelsatx.html

[Q84] 去除首尾空格
来源：http://hz.sxryk.cn/gtcnrvlmjt.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxinkj.top/gtmdnvfcfh.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gtlqlthump.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.iojbl.cn/gtbkpyzook.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxinkj.top/gtedwezvje.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jyoumei.cn/gtnuefdono.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtyjafbmyz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cqqwz.cn/gtrdsuwhio.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtihqpsgql.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangtech.top/gtuwcwelsr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtegjmeitx.html

[Q89] 判断表是否存在
来源：http://hz.gogol.net.cn/gtrivvshtw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cashguo.top/gtkirisicv.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtrrbhuotv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.svipenyu.cn/gtuylvuhyu.html

================================================================================
来源：http://hz.cqqwz.cn/gtwqcbisdg.html

R. Bash 专题
来源：http://hz.smart0.xyz/gtlpzzapmf.html

================================================================================
来源：http://hz.fengsongda.top/gtqcdjiuun.html

[R01] shebang 与严格模式
来源：http://hz.aibaodan.cn/gttepodsrm.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtthulagmy.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtdporqyzb.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtkicyckqz.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gteokzwheo.html

[R03] 只读变量
来源：http://hz.ppjwa.cn/gtogjxinhj.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtfaqzouhq.html

[R04] 位置参数
来源：http://hz.mhx1999.top/gtteqsjcvy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gtccjzgkdz.html

[R05] 参数默认值
来源：http://hz.ydzc1.top/gteptmtnuv.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gturgilpbz.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtcveqwoch.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sysykeji.top/gthadsmjjv.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gtoxnbltsd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gtjllupzwl.html

[R08] 数值比较
来源：http://hz.xuetiantiany.cn/gtsdqowmht.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtbaibmddl.html

[R09] 字符串比较
来源：http://hz.andypj.xyz/gtremsovcl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gtxqwmjrby.html

[R10] 正则匹配
来源：http://hz.zycfv.cn/gtqbwjnags.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jiagoushi.top/gtsosttmuv.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtbecdoutn.html

case "$1" in
来源：http://hz.c1oappe.top/gtsfkmvhht.html

start) echo "启动" ;;
来源：http://hz.xuetiantiany.cn/gtsxqhystw.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gtrjiyhiqz.html

*)     echo "未知命令" ;;
来源：http://hz.hywenlv.cn/gtwtopxynr.html

esac
来源：http://hz.wangdashe.top/gtkjjougzx.html

[R12] for 遍历文件
来源：http://hz.nwbrower.top/gtwkwxqjms.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgufenzy.top/gticnimtnh.html

[R13] for 计数循环
来源：http://hz.zhaomingkeji.xyz/gtouzfswrk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtempjmuun.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gteiczixlf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.andypj.xyz/gtsnmitqkg.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtivktygsz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hammf.cn/gtwefldyax.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtqurlgiil.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtmherrsxn.html

[R17] 数组定义与取值
来源：http://hz.jqgfzy.top/gtfkwebxwp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtmdpgtsom.html

[R18] 遍历数组
来源：http://hz.zhoulong.xyz/gtwopzdlew.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yangfankeji.com/gtjenzcefn.html

[R19] 数组长度
来源：http://hz.shanyushiyangtech.top/gtwyiycakl.html

echo "${#arr[@]}"
来源：http://hz.yuanzhike.top/gteywlkvrq.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gteoxssmrl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pycfn.com/gtbuumhqbk.html

[R21] 字符串长度
来源：http://hz.shanyushiyangkeji.top/gtrbcfitvs.html


<!-- 参考信息 -->