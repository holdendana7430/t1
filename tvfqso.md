代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.hammf.cn/gtuberanrk.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtivovebgq.html

Ruby: x.length;  x.size
来源：http://hz.jinyuanbaomall.cn/gtabwtcjoj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtycnlgrli.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gteiazaflb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinghuilouyu.cn/gtdqczfhxq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtzkrkmryg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.meibo888.top/gtnbnczctd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gtftbuvlvo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gtrtvnwsei.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtwhnmsiii.html

Ruby: a == b
来源：http://hz.fzhhl.top/gtyninakzq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gogol.net.cn/gttvsctksu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhaomingkeji.xyz/gtkgivrukj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhongyouzk.top/gtctrqhsed.html

PHP:  if (empty($x)) {}
来源：http://hz.hywenlv.cn/gtyfpbaygg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guowangkeji.top/gtvrivoxxm.html

TS:   if (x == null) {}
来源：http://hz.gaohongyu789.top/gtxgjloavu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gtfoqxyqoy.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtmfwqnmou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gtpycxakzk.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtxcqwwyoo.html

[P07] 防抖与节流
来源：http://hz.jianghu66.top/gtxgtrkaxf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangtech.top/gtktcovxtp.html

PHP:  // 手写时间戳比较
来源：http://hz.yj202588.top/gtytcxeqaq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtwhgyokce.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtqrraqsdw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuxming.cn/gtkypoqkib.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ybcxt.top/gtnmjetgfz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shuidangran.top/gtuyedetfy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dashuyun.cn/gtobqivcim.html

[P08] 处理浮点精度问题
来源：http://hz.zhongyouzk.top/gtymauqurq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuanzhike.top/gtsuclybgg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yanxiufei.cn/gtwqsqdfdf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gtzdxynawh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtkptrikmd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xylfe.cn/gtfkagcbyi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guannengcc.top/gtuokffslw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gtkyshaebk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gtvjtwenhh.html

================================================================================
来源：http://hz.ydzc1.top/gtekhhmmoj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigufen.top/gtwonpnnle.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnqjzxwzo.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtymprksxd.html

CREATE TABLE users (
来源：http://hz.tian-w.cn/gtfchdapmx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtijslawzd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.haohaochexian.top/gtkvnofbvu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigufen.top/gtdfqeytjj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtbnwqvkfz.html

);
来源：http://hz.xuetiantiany.cn/gtnmcmnskp.html

[Q02] 创建带外键的表
来源：http://hz.c1oappe.top/gtgwiqxtts.html

CREATE TABLE orders (
来源：http://hz.mhx1999.top/gtbygxbobq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtsybbzize.html

user_id INT NOT NULL,
来源：http://hz.wangdashe.top/gtkxhppjae.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtnpshqsvv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhiwuduotai.top/gtrcgimpnq.html

);
来源：http://hz.yj20258.top/gtlknexpjc.html

[Q03] 增加列
来源：http://hz.zhongyouzk.top/gtgiokajrg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtcssxophi.html

[Q04] 修改列类型
来源：http://hz.ppjwa.cn/gthnjotacc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenlongwang.top/gtkenbrwih.html

[Q05] 重命名列
来源：http://hz.c1oappe.top/gtfanbpqpa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cashguo.top/gtjnffasdf.html

[Q06] 删除列
来源：http://hz.xingfuxueyuan.xyz/gtdynqehuy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtnsrzkjsq.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gtajmptasm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hfpthk.cn/gtjptjitxb.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gtpmicwubz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tanke756.top/gtzylzmith.html

[Q09] 创建唯一索引
来源：http://hz.pengpengdd.cyou/gtdcjqpyln.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yvedp.cn/gtvwqicctd.html

[Q10] 插入单行
来源：http://hz.chenlongwang.top/gtqjvijgom.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenzaomai.com/gthoieecuy.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtywzugwlf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuanzhike.top/gtzzoejqze.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gtequoopim.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hysaishi.cn/gtjaqlrqeb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.feifeiyinyue.top/gttwecmjoe.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtwrubbfsv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sysykeji.top/gtmrwfymos.html

[Q14] 存在则更新（upsert）
来源：http://hz.shangyingyoupin.top/gtqpnaspjp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtshfaiohv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tanke756.top/gtmrovuccf.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtgsgropor.html

SELECT * FROM users;
来源：http://hz.316326.xyz/gtdoxgvcyk.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtdihioupi.html

SELECT id, name FROM users;
来源：http://hz.316326.xyz/gtqhmezywm.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtjlsqxcip.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtoqpxphft.html

[Q18] 模糊匹配
来源：http://hz.daria6918.cn/gtvlforrji.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xziqi.cn/gtkldwlizu.html

[Q19] 范围查询
来源：http://hz.bjfxy.top/gtpwokshna.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtynlelcdu.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gthkchornh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgufenzy.top/gtqjhwevif.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtvlicyxdo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gtzoedhfma.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtivtwcwhv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtfwolnjfc.html

[Q23] 分页
来源：http://hz.xingfuxueyuan.xyz/gtgnakmoqj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ivvv.top/gtowntocbe.html

[Q24] 去重
来源：http://hz.wangshuangyany.cn/gtthbylahd.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtsleqdusf.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gttkhhaufd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtqjvesyga.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gtrtgzzxbv.html

SELECT COUNT(*) FROM users;
来源：http://hz.daria6918.cn/gtzigogufy.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gttsgditop.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinghuilouyu.cn/gtklactfjp.html

[Q28] 求和与平均
来源：http://hz.cdnleiting.top/gthgurogux.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxuanxn.top/gtrluzvmgl.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gtwkjctxgl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gtoairmphh.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtxmnfufop.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtknknntcn.html

[Q31] 分组后过滤
来源：http://hz.xingfuxueyuan.xyz/gttrjxflzx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jqgufenzy.top/gtbwkujrqi.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtuniphumu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtwhkzwkmk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.redwolf501.top/gtiqoejony.html

[Q33] 多列分组
来源：http://hz.sufxvd.cn/gthajifiii.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pycfn.com/gtsgfhokrh.html

[Q34] 每组取第一条
来源：http://hz.cucudq.cn/gtoqixcoab.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtwsrojfhf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jiagoushi.top/gtuukwsjle.html

) t WHERE rn = 1;
来源：http://hz.chenzaomai.com/gtsjkqgxxz.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtguaxlxwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtgcnvhtlu.html

[Q36] 左连接
来源：http://hz.jinghuilouyu.cn/gtaejsyddw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtgcqgwtda.html

[Q37] 右连接
来源：http://hz.cheryme.top/gtypufiyde.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tianlin.xyz/gtmueredeh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinghuilouyu.cn/gtiwocdfiy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnxiangtu.top/gtbdhpjdhy.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gtdjzhqwku.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhoulong.xyz/gtvaknpxdw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aizwys.cn/gtetuwhyds.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtduzmbrtd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.andypj.xyz/gtzuaprsen.html

[Q41] 多表连接
来源：http://hz.jianghu66.top/gtzcngoozg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtvnvoboll.html

JOIN users u ON u.id = o.user_id
来源：http://hz.52xcode.cn/gtqnflkdwh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.feifeiyinyue.top/gtebsagcro.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtlblexmbx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yongpay.top/gtfemhmypn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yanxiufei.cn/gtreuyonos.html

[Q43] 标量子查询
来源：http://hz.yj20258.top/gtoupjxlth.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtqnncxggy.html

[Q44] IN 子查询
来源：http://hz.xinyue.icu/gtjxwqancw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.iojbl.cn/gtwgaoiodz.html

[Q45] EXISTS 判断存在
来源：http://hz.xingfuxueyuan.xyz/gtdvjtraiq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gttdvoxghb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gtjqvegnbs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtmssvpdos.html

[Q47] 与平均值比较
来源：http://hz.yonumen.top/gtoyyciqwk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtwjvxbmnp.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtlwsawhub.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.vqdsnc.cn/gtaolubeuc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sweek.top/gtybeupyfh.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtawbrsxnz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtgyreijnq.html

[Q50] 批量更新
来源：http://hz.iojbl.cn/gtmspdrxsm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuanzx.com/gtekvledof.html

[Q51] 用子查询更新
来源：http://hz.aizwys.cn/gtofihzvqx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hfpthk.cn/gtghjgsimt.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtafegyfbb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtudgooknp.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtxiprsfrl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.vqdsnc.cn/gtviezgyso.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtwopfhxhv.html

TRUNCATE TABLE logs;
来源：http://hz.shangyingyoupin.top/gtrjvgoqrg.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtfvmsvvit.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gtkffeskpe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhongyouzk.top/gtjliiajxj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtingvzftx.html

[Q57] 行号
来源：http://hz.ehwqpu.com/gtasnixwlf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hywenlv.cn/gtypuprtlz.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtclfpwvwd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtjmusnoeu.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtwkqwomob.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtdytpwnlf.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtiqyltpqe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.0kj1m.cn/gtsazrbsds.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hywenlv.cn/gtcmbrsivz.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtkdtstdtv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenjidiqi.icu/gtrwcnhfah.html

[Q62] 分组占比
来源：http://hz.chenjidiqi.icu/gtuzirxrof.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtlkbrxxkc.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtympdwryq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.9152youxi.cn/gtnkvplxpr.html

[Q64] 提交事务
来源：http://hz.shuidangran.top/gtvbvhilld.html

COMMIT;
来源：http://hz.guannengcc.top/gtrokifsjo.html

[Q65] 回滚事务
来源：http://hz.ywan-chungtsiang.top/gtkkmbbshk.html

ROLLBACK;
来源：http://hz.jqgufenzy.top/gtnzrttqou.html

[Q66] 行锁查询
来源：http://hz.nwbrower.top/gtmscckvai.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtbextdvtc.html

[Q67] 设置隔离级别
来源：http://hz.yj202588.top/gteyamnuer.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zdqjudy.top/gtgiaoojcq.html

[Q68] 保存点
来源：http://hz.hywenlv.cn/gtwpincpxx.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtruuzbjdq.html

ROLLBACK TO sp1;
来源：http://hz.bjfxy.top/gtxoadmwox.html

[Q69] 查看执行计划
来源：http://hz.shuidangran.top/gtpqgpkdos.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.316326.xyz/gtawmfssrv.html

[Q70] 更新统计信息
来源：http://hz.gotoacloud.top/gtgvdwtznr.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtszuptqzg.html

[Q71] 查看建表语句
来源：http://hz.svipenyu.cn/gtcbolzgys.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yanxiufei.cn/gtwyoivell.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtjfhdxprq.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtdlvmwfoh.html

[Q73] 查看表状态
来源：http://hz.zhiwuduotai.top/gtmmizwmmt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ywan-chungtsiang.top/gtukyylihm.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtvrsyzltr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gtzjubidwz.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gtrbtpythn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daxiang520.top/gtpjbnoxkm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gttewhayqz.html

[Q76] 按天统计
来源：http://hz.wangshuangyany.cn/gtozxwmppi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenjidiqi.icu/gtunwxrqsc.html

[Q77] 时间加减
来源：http://hz.wangshuangyany.cn/gtnnlzgnxc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ivvv.top/gtxifotqcn.html

[Q78] 当前时间
来源：http://hz.fzhhl.top/gtzaccvmuw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yonumen.top/gtosbhkuoz.html

[Q79] 字符串拼接
来源：http://hz.zycfv.cn/gtvsbgvqwq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtzdsrojzs.html

[Q80] 字符串截取
来源：http://hz.cashguo.top/gtzmamfqcq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gtfhlnxsnf.html

[Q81] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gticeskwyz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ivvv.top/gtcyskxptk.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtmjgfpwcr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jianghu66.top/gtzirvrwde.html

[Q83] 大小写转换
来源：http://hz.wangdashe.top/gtgbahxwxn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ppjwa.cn/gtqtxxulle.html

[Q84] 去除首尾空格
来源：http://hz.ywan-chungtsiang.top/gtzsgcfaeg.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtwulhljdd.html

[Q85] 数值取整
来源：http://hz.gaohongyu789.top/gteinhngui.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtvknyoiot.html

[Q86] 读取 JSON 字段
来源：http://hz.yongpay.top/gtkysowprm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtdgpscuvz.html

[Q87] JSON 字段做条件
来源：http://hz.sweek.top/gtvocidnvy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtcgmoecqt.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtbtudxopl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtludqgncq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.quarkkingdee.top/gtiubmkqph.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtftannzcl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtyftepxka.html

[Q90] 生成序号列
来源：http://hz.dashuyun.cn/gtoikpkkle.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtmfexueno.html

================================================================================
来源：http://hz.svipenyu.cn/gtdawhngfn.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtaakiuepm.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtllotuafa.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gtxjssyegj.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtwonjohxh.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtdjwaajzb.html

[R02] 变量赋值与使用
来源：http://hz.mhx1999.top/gtirhjpgxd.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtygwfklyp.html

[R03] 只读变量
来源：http://hz.xziqi.cn/gtbrsqwcal.html

readonly PI=3.14
来源：http://hz.andypj.xyz/gtjkvfjwlo.html

[R04] 位置参数
来源：http://hz.sxryk.cn/gttaohmvea.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtdnpfjewy.html

[R05] 参数默认值
来源：http://hz.zhaomingkeji.xyz/gtqxlbtxsg.html

name="${1:-default}"
来源：http://hz.yuxming.cn/gtjvixwows.html

[R06] 判断命令是否存在
来源：http://hz.fengsongda.top/gtmlupxcxj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tian-w.cn/gtdwtrwozw.html

[R07] if 判断文件
来源：http://hz.dashuyun.cn/gtbullaccg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gteiclmvat.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtftimizbn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gtsdhnvejw.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gtbxcviily.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.52xcode.cn/gtvybawnvb.html

[R10] 正则匹配
来源：http://hz.meibo888.top/gtqhlorlvu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258888.top/gtvujewpxb.html

[R11] case 多分支
来源：http://hz.yuxming.cn/gtimljxkwg.html

case "$1" in
来源：http://hz.chenlongwang.top/gthbogkhcz.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gtynhwaiue.html

stop)  echo "停止" ;;
来源：http://hz.feifeiyinyue.top/gteosnnfpt.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtbikkucll.html

esac
来源：http://hz.ehwqpu.com/gtgmtfyxnz.html

[R12] for 遍历文件
来源：http://hz.yanxiufei.cn/gtgnnsexrq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtrbdspqil.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtwxcbqsai.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtwpmzkftl.html

[R14] C 风格 for
来源：http://hz.zhaomingkeji.xyz/gtmovmfgal.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yangfankeji.com/gtngbclgmg.html

[R15] while 逐行读文件
来源：http://hz.sweek.top/gtzgimppgr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yueranfly.top/gthquspgpe.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtnbliivcg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtgmruulvm.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtnoyuskhi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shzxlz.cn/gtnkmtawkc.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gtciiyvxfj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sysykeji.top/gtvvfzeywp.html

[R19] 数组长度
来源：http://hz.jiagoushi.top/gtqhmebvjm.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtpewhdqki.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtrfozhfou.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xziqi.cn/gtygqeptpi.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtvgwvuvnd.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtfxcgonak.html

[R22] 截取子串
来源：http://hz.jqgufenzy.top/gtpnkmihvt.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gttbhhzrjg.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gtrwixuaxn.html


<!-- 参考信息 -->