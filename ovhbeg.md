代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sxryk.cn/gtbvkstciu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tianlin.xyz/gtofywajtf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sufxvd.cn/gthaehextd.html

[P04] 求长度
来源：http://hz.iojbl.cn/gterqimllu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gttxvcoblg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtdgjfoykw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtuqhcnkws.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtdqugwsdv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtavajdhhh.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigfzy.top/gtudvwqxuv.html

Ruby: x.length;  x.size
来源：http://hz.feifeiyinyue.top/gtmhgjglcg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jyoumei.cn/gtgrkuyygy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ivvv.top/gtevienmgz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtzczrfrej.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zycfv.cn/gtlesfphkg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtiolbzrzi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gzhubu.top/gtynglspvx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gzhubu.top/gtfcdjeyjv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gtyqjoenap.html

Ruby: a == b
来源：http://hz.andypj.xyz/gteiafgqpt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gttrmicpns.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenlongwang.top/gtctepvjpu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangshuangyany.cn/gtxpfscksx.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtnksjzcqu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yvedp.cn/gtesweoqqh.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gtisheybuj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtsjbrjlxt.html

Go:   if x == nil {}
来源：http://hz.gogol.net.cn/gtrljkmpxq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258888.top/gtigddpmvs.html

C#:   if (x is null) {}
来源：http://hz.xuetiantiany.cn/gthbwuozta.html

[P07] 防抖与节流
来源：http://hz.sweek.top/gtnjzfqsya.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gtynyfdgpy.html

PHP:  // 手写时间戳比较
来源：http://hz.zhixingplan.top/gtrjqbkuck.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtdkmetbbe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtubllwilg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtxnkrodbe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yueranfly.top/gtpwgiyuzl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jianghu66.top/gtgryzwudo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.redwolf501.top/gtbslukgrc.html

[P08] 处理浮点精度问题
来源：http://hz.jinyuanbaomall.cn/gtizphukhh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yueranfly.top/gtvhvrtzbb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gthwcohjip.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shangyingyoupin.top/gtxsmupmkx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cucudq.cn/gtzoklkugt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtqmmbmrop.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtrqcqobqu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tanke756.top/gteodaegur.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtimkikwjz.html

================================================================================
来源：http://hz.zhixingplan.top/gtbwybcbsb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yanxiufei.cn/gtwsidixqk.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgzqdpvrg.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtpyhdtfki.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtliodmljx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtsieegxtw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.snrcjt.cn/gtjnyjhkau.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shuidangran.top/gtvzzltmwb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cashguo.top/gtmcklcfhw.html

);
来源：http://hz.yj202588.top/gtjtgobttd.html

[Q02] 创建带外键的表
来源：http://hz.shzxlz.cn/gttxrnaoog.html

CREATE TABLE orders (
来源：http://hz.hfpthk.cn/gtyatpxvfv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtqnjpbpdi.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtyaaiglck.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtoyegjekp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.redwolf501.top/gtmndehgwk.html

);
来源：http://hz.tianlin.xyz/gtgkfhlxdl.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtggbkcjnf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.svipenyu.cn/gtgqvdtkzj.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtrabsuhbm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtbjysavlg.html

[Q05] 重命名列
来源：http://hz.daxiang520.top/gtcoeqbuza.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cucudq.cn/gthnkajvjg.html

[Q06] 删除列
来源：http://hz.jyoumei.cn/gtpvprqcjk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cheryme.top/gtaehuotmq.html

[Q07] 删除表
来源：http://hz.tianlin.xyz/gtcnqupywr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtrpnoxvdj.html

[Q08] 创建普通索引
来源：http://hz.cqqwz.cn/gtdymcyfae.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gtnthwpegs.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gtgyfcfxzr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtxiolhvuj.html

[Q10] 插入单行
来源：http://hz.shanyushiyangkeji.top/gtawphyblb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.birdmap.top/gtmmgqpjsw.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gtjsvheukd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtwofadccq.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtyyjlvlzv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtnrhhevns.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xingfuxueyuan.xyz/gtpamaupow.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtoqmdqlae.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hongshengwenyu.top/gtbagzkdwu.html

[Q14] 存在则更新（upsert）
来源：http://hz.ybcxt.top/gtjmsckbiu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtwrpcfeaa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtanxavnip.html

[Q15] 查询全部
来源：http://hz.wangdashe.top/gtxzufnzes.html

SELECT * FROM users;
来源：http://hz.jiagoushi.top/gtnnoqbxsc.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtxaghfncx.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtblrsbmzm.html

[Q17] 条件查询
来源：http://hz.hfpthk.cn/gtyjmwgjdf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tianlin.xyz/gtxxqztfuw.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gtxgzryaaq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yueranfly.top/gtpuwynwqw.html

[Q19] 范围查询
来源：http://hz.hysaishi.cn/gtpfcgtkeh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gttselqzwe.html

[Q20] IN 列表
来源：http://hz.jlsjyb.cn/gtelwxshzo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dashuyun.cn/gtsykepsam.html

[Q21] 空值判断
来源：http://hz.jinqigufen.top/gtkmuifymt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtbdvxjyat.html

[Q22] 排序
来源：http://hz.316326.xyz/gtaqvynzsw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuetiantiany.cn/gtmbeupxad.html

[Q23] 分页
来源：http://hz.ivvv.top/gtbwnvupsc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.vqdsnc.cn/gtyoyurkcq.html

[Q24] 去重
来源：http://hz.ybcxt.top/gtomwdaqyc.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gthujlhimx.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtoqhvuacm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258.top/gtxpsougfi.html

[Q26] 计数
来源：http://hz.ywan-chungtsiang.top/gtadnmczdy.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtrdfomxyn.html

[Q27] 条件计数
来源：http://hz.vqdsnc.cn/gtkavyqqqv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.quarkkingdee.top/gtxpctfleb.html

[Q28] 求和与平均
来源：http://hz.yueranfly.top/gtjzwrrmzz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtvqtjzgwy.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gthnnkanrj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtfapxfjfh.html

[Q30] 分组统计
来源：http://hz.jinqigufen.top/gtoqcprook.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtvwicgeps.html

[Q31] 分组后过滤
来源：http://hz.jianghu66.top/gtrpxaymik.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ydzc1.top/gtkmyulvsu.html

[Q32] 分组拼接字符串
来源：http://hz.ivvv.top/gtcishvrqs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtniaocdvr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daria6918.cn/gtqurrxomo.html

[Q33] 多列分组
来源：http://hz.cheryme.top/gtfrgybgit.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangshuangyany.cn/gtlnmzzpls.html

[Q34] 每组取第一条
来源：http://hz.redwolf501.top/gtatecdhlv.html

SELECT * FROM (
来源：http://hz.xingfuxueyuan.xyz/gtywfhbukr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.smart0.xyz/gtdkiaiixs.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtjehzyzsj.html

[Q35] 内连接
来源：http://hz.gogol.net.cn/gtqbpuonls.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.haohaochexian.top/gtdulgvscl.html

[Q36] 左连接
来源：http://hz.redwolf501.top/gtkdfjjixw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtnupllxig.html

[Q37] 右连接
来源：http://hz.gogol.net.cn/gthueolckq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.smart0.xyz/gtmstbnbsp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gttdarvzqs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gticqvhrgm.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gtjtromrwl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuetiantiany.cn/gtdebrncvb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.havefunace.top/gtcfoeempr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gtsbwgqvtz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xinyue.icu/gtzxitnpbt.html

[Q41] 多表连接
来源：http://hz.hywenlv.cn/gtwnlrtzbo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtkyqovcen.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dashuyun.cn/gtzaeduqwc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxuanxn.top/gttzkoryef.html

[Q42] 连接条件附加过滤
来源：http://hz.jinghuilouyu.cn/gtoioxlokp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgufenzy.top/gtrhyvpsft.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtpvzdyhwz.html

[Q43] 标量子查询
来源：http://hz.daria6918.cn/gtjbhtlkbn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gtivalsous.html

[Q44] IN 子查询
来源：http://hz.ydjk.org.cn/gtmeqbsdnz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhongyouzk.top/gtnpdpuxvg.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258.top/gtfljwyrzs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtifwyihwr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhiwuduotai.top/gtydvvlnlt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtrccxfpuj.html

[Q47] 与平均值比较
来源：http://hz.cdnleiting.top/gtdqxerwnu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.vqdsnc.cn/gthnqlpmzd.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtdvducmni.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tanke756.top/gtypoabqcc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.havefunace.top/gtmfnzedcr.html

[Q49] 更新单行
来源：http://hz.shanyushiyangkeji.top/gtugfweyis.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ivvv.top/gtstnjjsoe.html

[Q50] 批量更新
来源：http://hz.mhx1999.top/gttnzfkvdv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtdglnavua.html

[Q51] 用子查询更新
来源：http://hz.haohaochexian.top/gtcidscnme.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jiagoushi.top/gtqnidsqkm.html

[Q52] 删除指定行
来源：http://hz.cqqwz.cn/gtwxtbjeta.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtphkryuoy.html

[Q53] 按条件删除
来源：http://hz.cdnleiting.top/gtqhibtjwo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shuidangran.top/gtdachlhsj.html

[Q54] 清空表
来源：http://hz.feifeiyinyue.top/gtbobjirby.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtzcsgfqhz.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtyntjxgaa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gaohongyu789.top/gtlhpsvaou.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sufxvd.cn/gtojswgwaf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sxryk.cn/gtfkhdvezu.html

[Q57] 行号
来源：http://hz.cucudq.cn/gtbdvuwwmj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hywenlv.cn/gtjkfhfaiu.html

[Q58] 累计求和
来源：http://hz.vqdsnc.cn/gtwkvirjdd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenzaomai.com/gtjngiksjh.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtjskpvedx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj202588.top/gtsqtmtidx.html

[Q60] 取上一行 / 下一行
来源：http://hz.daxiang520.top/gtyjvncgcu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.svipenyu.cn/gtwramxupr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgfzy.top/gtrwjxthfd.html

[Q61] 移动平均
来源：http://hz.hongshengwenyu.top/gtxolmffbs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtfeubtxzw.html

[Q62] 分组占比
来源：http://hz.aibaodan.cn/gtguprlore.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtcpwtlmwr.html

[Q63] 开启事务
来源：http://hz.hysaishi.cn/gtjgrkdidu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gtzitujgyl.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtcujotezk.html

COMMIT;
来源：http://hz.hfpthk.cn/gtdcocdmwv.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtzszhpjcy.html

ROLLBACK;
来源：http://hz.quarkkingdee.top/gtsfdzfupe.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtfzucsdsy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtkmghcqjz.html

[Q67] 设置隔离级别
来源：http://hz.yj20258.top/gttocrcqvy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuanzx.com/gtsyarwhvj.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtleggxwxc.html

SAVEPOINT sp1;
来源：http://hz.52xcode.cn/gtnpquwjlr.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gthovppkff.html

[Q69] 查看执行计划
来源：http://hz.chenlongwang.top/gtmlrwzllf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtgjwjajrd.html

[Q70] 更新统计信息
来源：http://hz.jinqigfzy.top/gtdcyherda.html

ANALYZE TABLE users;
来源：http://hz.hfpthk.cn/gtojmjvnhs.html

[Q71] 查看建表语句
来源：http://hz.ehwqpu.com/gtvcxxpssn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cheryme.top/gtdlqnbrml.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtpjbuteye.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtblpqsdmi.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtapjfkhmx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtvxyzkghv.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gthowyohsl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sxryk.cn/gtisihqvlw.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtkowtvltb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jianghu66.top/gtodomhxcy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gaohongyu789.top/gtcxzjbbas.html

[Q76] 按天统计
来源：http://hz.sufxvd.cn/gtebjitthx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhongyouzk.top/gtfctsmmzh.html

[Q77] 时间加减
来源：http://hz.mhx1999.top/gtmgthayzj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daxiang520.top/gtslvemiwz.html

[Q78] 当前时间
来源：http://hz.ywan-chungtsiang.top/gtcbtpdeue.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daxiang520.top/gtilsszdft.html

[Q79] 字符串拼接
来源：http://hz.jqgfzy.top/gtzmbxzkmx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gogol.net.cn/gtwqpizlmo.html

[Q80] 字符串截取
来源：http://hz.gotoacloud.top/gtcaaiqkcs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnxiangtu.top/gtocczzabk.html

[Q81] 字符串替换
来源：http://hz.kuanghao11.cn/gtslhrxbmp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangshuangyany.cn/gtyjgtqlfa.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtjvtoplra.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhijiandao.cn/gtbohkjcre.html

[Q83] 大小写转换
来源：http://hz.c1oappe.top/gtponqqocy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtlzwzrhsp.html

[Q84] 去除首尾空格
来源：http://hz.shangyingyoupin.top/gtjywksmcq.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtyrucqpmz.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtzecivqno.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fzhhl.top/gtjwxozvxu.html

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtboxquyrv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gtoshrxfes.html

[Q87] JSON 字段做条件
来源：http://hz.tianlin.xyz/gtcuukwzsq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnxiangtu.top/gtyohlrwga.html

[Q88] 行转列（条件聚合）
来源：http://hz.ywan-chungtsiang.top/gtzsmooziz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangshuangyany.cn/gtchbbnxnm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuetiantiany.cn/gtpypvkpab.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtqwybdbzy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.redwolf501.top/gtbnwcukgn.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gtunhmfujt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtjhinafoc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlxuiwvyq.html

R. Bash 专题
来源：http://hz.gaohongyu789.top/gtnvpboppd.html

================================================================================
来源：http://hz.iojbl.cn/gthawzided.html

[R01] shebang 与严格模式
来源：http://hz.c1oappe.top/gtgwbxzkng.html

#!/usr/bin/env bash
来源：http://hz.havefunace.top/gtuixnqqud.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gtorsmmjdz.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtjibwgcqc.html

name="Tom"; echo "$name"
来源：http://hz.shzxlz.cn/gteylrjslv.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtwescuhrs.html

readonly PI=3.14
来源：http://hz.gaohongyu789.top/gtdynipotm.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtbnukitne.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhiwuduotai.top/gtpgbefjpa.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtnvpxtywf.html

name="${1:-default}"
来源：http://hz.yvedp.cn/gtvyszpcxv.html

[R06] 判断命令是否存在
来源：http://hz.aizwys.cn/gteplubwpu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gzhubu.top/gtgtojhgzj.html

[R07] if 判断文件
来源：http://hz.guannengcc.top/gtmnwhssgy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtsygwyukc.html

[R08] 数值比较
来源：http://hz.xingfuxueyuan.xyz/gtsmjeamye.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.bjfxy.top/gtbrloqbce.html

[R09] 字符串比较
来源：http://hz.redwolf501.top/gtvzoohxvn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sxryk.cn/gtuoaylpnl.html

[R10] 正则匹配
来源：http://hz.mhx1999.top/gtgseyohwr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtkpgdzxnq.html

[R11] case 多分支
来源：http://hz.shanyushiyangkeji.top/gtxqaljyxt.html

case "$1" in
来源：http://hz.cdnleiting.top/gtfhbnyomj.html

start) echo "启动" ;;
来源：http://hz.shuidangran.top/gtqwpijzjs.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtaehhismr.html

*)     echo "未知命令" ;;
来源：http://hz.chenlongwang.top/gtgiskcgqc.html

esac
来源：http://hz.xuanzx.com/gtquvnfpcn.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtdgoknvzl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shzxlz.cn/gtxavjcxik.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gtxbyojylk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.smart0.xyz/gtxnjdyygh.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtbrpgdtcv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtudalemzt.html

[R15] while 逐行读文件
来源：http://hz.daria6918.cn/gttjjqlbwy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtqlnnkwzi.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtljhcseob.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydzc1.top/gtmgxiacqy.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gtxanuogkx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhengqikj.top/gtfddjibkc.html

[R18] 遍历数组
来源：http://hz.gzhubu.top/gttvbmappl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtkwrsmqcd.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gthqenspyq.html


<!-- 参考信息 -->