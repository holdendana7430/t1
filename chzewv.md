代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtzgikxopd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhengqikj.top/gtnbfnqxjr.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtuyfzqrjy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtpelvargv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtbmmayppj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtdgsfnstf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gteyhagsmo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yonumen.top/gtejvnshef.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hammf.cn/gttccnqmvg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtlmqxedjv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtysrtzwfy.html

[P04] 求长度
来源：http://hz.birdmap.top/gtmdrlvsxs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhiwuduotai.top/gtsdbtvkce.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtuarmacwi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtnmhsgtfc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gtmlqjuvfs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtcbvkbhoj.html

Go:   len(arr);  len(m)
来源：http://hz.smart0.xyz/gtvyghfudz.html

Ruby: x.length;  x.size
来源：http://hz.pycfn.com/gtijgbvvtu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jlsjyb.cn/gtdlnqorfa.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigufen.top/gtxripethd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gtmqrlmpgd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tanke756.top/gtrzcpkuos.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtzlrmoifd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtuifkvhwa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tianlin.xyz/gtbojnpxnh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnqzz.top/gtesikokvb.html

Ruby: a == b
来源：http://hz.mhx1999.top/gtahqqagjk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtafudmxak.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangtech.top/gtbdxhzpsq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yanxiufei.cn/gtbbarcmvd.html

PHP:  if (empty($x)) {}
来源：http://hz.hnqzz.top/gtxhgfdhoy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gthllkykhi.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtwrykdhoy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtegfelnyo.html

Go:   if x == nil {}
来源：http://hz.hysaishi.cn/gtvspksbel.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtwckmloqu.html

C#:   if (x is null) {}
来源：http://hz.9152youxi.cn/gtydgtpncn.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gttmrfbwct.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtmsopapiy.html

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gtryfrhzcl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtlolezfjc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtbntfvjrx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.mhx1999.top/gtehpybfud.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtxvmopnii.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gtprfpspmq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hysaishi.cn/gtigevhuwr.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtbdhdqwlz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258888.top/gtymcnjkyn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hysaishi.cn/gtboammgcy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtmettuhba.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtzqdopeco.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hongshengwenyu.top/gtlykstlgr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shuidangran.top/gtwlbdsjpu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.52xcode.cn/gtznwzsxuq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnxiangtu.top/gtosxeqxni.html

================================================================================
来源：http://hz.yonumen.top/gtzxgqirew.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.meibo888.top/gtffxugxmp.html

================================================================================
来源：http://hz.hywenlv.cn/gtzcptkhzj.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtacbgcqds.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtbwzdoqwl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtsvihepzi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtagxturep.html

email VARCHAR(100) UNIQUE,
来源：http://hz.redwolf501.top/gtwexothro.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hammf.cn/gtxzijkpwx.html

);
来源：http://hz.daria6918.cn/gtlkzpdqin.html

[Q02] 创建带外键的表
来源：http://hz.dianchejie.cn/gtzshhglfc.html

CREATE TABLE orders (
来源：http://hz.meibo888.top/gtuiqrqsel.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yvedp.cn/gtomllyxyi.html

user_id INT NOT NULL,
来源：http://hz.yueranfly.top/gtupgkgyug.html

amount DECIMAL(10, 2),
来源：http://hz.svipenyu.cn/gtsbvidndb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gteldlnuxx.html

);
来源：http://hz.hywenlv.cn/gtaiwqhtfg.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtzvkrhtkw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ehwqpu.com/gthmfzsseg.html

[Q04] 修改列类型
来源：http://hz.tian-w.cn/gtahfdhccz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtabtnloli.html

[Q05] 重命名列
来源：http://hz.jinyuanbaomall.cn/gtgrtbyyzy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtvktxagjf.html

[Q06] 删除列
来源：http://hz.gotoacloud.top/gtpaqjtzls.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhaomingkeji.xyz/gtxwwzupua.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtjoakrbue.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtgjrtwbgp.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtcjhfigxd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fengsongda.top/gtcpccibly.html

[Q09] 创建唯一索引
来源：http://hz.jiagoushi.top/gtswzygrng.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtzofyorjw.html

[Q10] 插入单行
来源：http://hz.jiagoushi.top/gtzxedggpy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigufen.top/gtyqzekndg.html

[Q11] 一次插入多行
来源：http://hz.sysykeji.top/gtnrykaaqs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.meibo888.top/gtwpyfwmps.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtchgefiof.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gaohongyu789.top/gtreonenak.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtrxotuoxb.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gtzqhaonwd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtcuixkwmt.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgufenzy.top/gttgeddtfv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sxryk.cn/gtgemppkmg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gthlspxtnj.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gtyzitukwm.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gtatjknvsy.html

[Q16] 查询指定列
来源：http://hz.gzhubu.top/gteuakzdwq.html

SELECT id, name FROM users;
来源：http://hz.c1oappe.top/gtpklkwwjp.html

[Q17] 条件查询
来源：http://hz.yongpay.top/gtklfgnjgn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtzcmqdcan.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtjcipeiip.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuanzx.com/gttpqpbyjx.html

[Q19] 范围查询
来源：http://hz.9152youxi.cn/gtorsvejxe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtscjiatqc.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtmzrgxjpg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gtbwpizybf.html

[Q21] 空值判断
来源：http://hz.shzxlz.cn/gtdnwdmoct.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.feifeiyinyue.top/gtvrkkowby.html

[Q22] 排序
来源：http://hz.pycfn.com/gtckozoahq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gtehhnrfth.html

[Q23] 分页
来源：http://hz.shanyushiyangkeji.top/gtailpiele.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gzhubu.top/gtofnxmcau.html

[Q24] 去重
来源：http://hz.chenlongwang.top/gtssdwqwph.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtjvxfvqax.html

[Q25] 只取前 N 条
来源：http://hz.52xcode.cn/gtqngevxbn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gtakfyocvf.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtmqcufuht.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydzc1.top/gttxhqiqeq.html

[Q27] 条件计数
来源：http://hz.zhongyouzk.top/gtuxtwkpnc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtdxgvgdio.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtxkvnhzxs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.0kj1m.cn/gtgxikoamk.html

[Q29] 最大最小值
来源：http://hz.fzhhl.top/gtugflytxc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtsywjnent.html

[Q30] 分组统计
来源：http://hz.jinyuanbaomall.cn/gtzicjdcjh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtjedthpla.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtkrzoxuek.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtikurfbhz.html

[Q32] 分组拼接字符串
来源：http://hz.snrcjt.cn/gtqqmutdek.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtxtecoduk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.snrcjt.cn/gtqxxgnnpr.html

[Q33] 多列分组
来源：http://hz.hammf.cn/gtqioqjaai.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangtech.top/gtenmumatt.html

[Q34] 每组取第一条
来源：http://hz.cucudq.cn/gtgyeazigc.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gtzheogqaj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jiagoushi.top/gtblqbdywe.html

) t WHERE rn = 1;
来源：http://hz.cdnleiting.top/gtacnjwatr.html

[Q35] 内连接
来源：http://hz.xuanzx.com/gtwesqbgnz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtlixzenqb.html

[Q36] 左连接
来源：http://hz.yangfankeji.com/gttzftapmk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.redwolf501.top/gtvmegawfd.html

[Q37] 右连接
来源：http://hz.guannengcc.top/gtdtxvzkrb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtrbyvvzym.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.svipenyu.cn/gtviqvtlmm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.0kj1m.cn/gtfebvfcnv.html

[Q39] 自连接（查上下级）
来源：http://hz.tian-w.cn/gtwyvfmsrw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangdashe.top/gtncysfcdc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtrvuhppqu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pycfn.com/gtmnplozdw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gtjcnmrfze.html

[Q41] 多表连接
来源：http://hz.cqqwz.cn/gtxcpderms.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yvedp.cn/gtqnfbcvbs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtptyajmnh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuanzhike.top/gtwuleukif.html

[Q42] 连接条件附加过滤
来源：http://hz.yj202588.top/gtbehdyxlm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daria6918.cn/gtdiwnxsgn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.meibo888.top/gtvgmhlvge.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtwjhkssgd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xinyue.icu/gtoghnnpmr.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtemyfxata.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtborjkpzh.html

[Q45] EXISTS 判断存在
来源：http://hz.havefunace.top/gtwqhptqkv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtumtrwlkt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guowangkeji.top/gtfqypxnqu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gthzvazsgd.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gtircockdh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.svipenyu.cn/gtbcfwumib.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gttzrjmypz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhongyouzk.top/gtvtsonlpk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cucudq.cn/gtvkwwlebb.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtoksmblsc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hywenlv.cn/gtbystzsno.html

[Q50] 批量更新
来源：http://hz.hammf.cn/gtmuulbcsb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.dashuyun.cn/gtoihpchjs.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtgwgjlbwk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtdujwmaqe.html

[Q52] 删除指定行
来源：http://hz.zhaomingkeji.xyz/gtscrbuwws.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuanzhike.top/gtmzuiaiek.html

[Q53] 按条件删除
来源：http://hz.meibo888.top/gtpeacgkhx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fengsongda.top/gtqbuvladp.html

[Q54] 清空表
来源：http://hz.jinyuanbaomall.cn/gtpojfwpfn.html

TRUNCATE TABLE logs;
来源：http://hz.yuanzhike.top/gtaohushfe.html

[Q55] 排名（并列占位）
来源：http://hz.feifeiyinyue.top/gtpmfmqqel.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xylfe.cn/gtqyxcabce.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj202588.top/gtntrevcqc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgfzy.top/gtiqwygibn.html

[Q57] 行号
来源：http://hz.0kj1m.cn/gtwghfrqrl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtmwwrmceb.html

[Q58] 累计求和
来源：http://hz.zhaomingkeji.xyz/gtpgkgqqbk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuxming.cn/gtguuejydp.html

[Q59] 分组内累计
来源：http://hz.hammf.cn/gtlyiqnhuc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jiagoushi.top/gtqjdtmhyo.html

[Q60] 取上一行 / 下一行
来源：http://hz.guowangkeji.top/gtoaowhqqx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xziqi.cn/gtxedwvamz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yanxiufei.cn/gtwqesebtv.html

[Q61] 移动平均
来源：http://hz.jlsjyb.cn/gtptakndmv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtnrvrcomw.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtbqqzyiri.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtkxhawusj.html

[Q63] 开启事务
来源：http://hz.sxryk.cn/gtcdtncepr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daxiang520.top/gtoylrjyqz.html

[Q64] 提交事务
来源：http://hz.jiagoushi.top/gtrcbfkgxp.html

COMMIT;
来源：http://hz.jianghu66.top/gtpwmpkhhf.html

[Q65] 回滚事务
来源：http://hz.xinyue.icu/gttfpthtdi.html

ROLLBACK;
来源：http://hz.jianghu66.top/gtjefyrjcn.html

[Q66] 行锁查询
来源：http://hz.gotoacloud.top/gthmgovxlm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.bjfxy.top/gtgqxwqwtb.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtuywfvxag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuanzhike.top/gtlxuuqwif.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gttayycwjy.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gtyfuvexls.html

ROLLBACK TO sp1;
来源：http://hz.yj20258888.top/gtpckhpbnd.html

[Q69] 查看执行计划
来源：http://hz.jyoumei.cn/gtzvypgwry.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtcysmyqwv.html

[Q70] 更新统计信息
来源：http://hz.cheryme.top/gtjtbsewft.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtrkmhgcnb.html

[Q71] 查看建表语句
来源：http://hz.gogol.net.cn/gtpkhajydw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtsrqiorls.html

[Q72] 查看索引
来源：http://hz.svipenyu.cn/gtqbhowxaq.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtpshtxeup.html

[Q73] 查看表状态
来源：http://hz.meibo888.top/gtuqimwpuv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgufenzy.top/gtmjxblzyo.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtnyurclqd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gotoacloud.top/gtuajovyjb.html

[Q75] 日期格式化
来源：http://hz.svipenyu.cn/gtophozaol.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtaaxypicz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenjidiqi.icu/gtpqchjayk.html

[Q76] 按天统计
来源：http://hz.shangyingyoupin.top/gtbmqlimpj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtrlspvgqe.html

[Q77] 时间加减
来源：http://hz.jinqigufen.top/gtzpaglxah.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tian-w.cn/gtuscdtddu.html

[Q78] 当前时间
来源：http://hz.dianchejie.cn/gtcqnmhhyw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ivvv.top/gtchzjwxmk.html

[Q79] 字符串拼接
来源：http://hz.fzhhl.top/gtrkiqfvuw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.bjfxy.top/gtdeenkfht.html

[Q80] 字符串截取
来源：http://hz.aizwys.cn/gtmatqfwbw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gtubadtejg.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtiuleafgm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gtpteyobyh.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtogtahexe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gttpctrpnu.html

[Q83] 大小写转换
来源：http://hz.shuidangran.top/gtitjtumpr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtrgjxukdc.html

[Q84] 去除首尾空格
来源：http://hz.ivvv.top/gtynxpozlo.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtvaeardhw.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtgnnwudqk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtmnrdckcx.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtlxmugxnu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigufen.top/gtpkjuuklh.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gttdgxytko.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtkzkkfwrr.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtpueemskw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtnpoacjxs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydjk.org.cn/gtwkzqvcrd.html

[Q89] 判断表是否存在
来源：http://hz.zhengqikj.top/gtwmhzkfcn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xziqi.cn/gtsopbuipb.html

[Q90] 生成序号列
来源：http://hz.tianlin.xyz/gtoksdjfah.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtpsddaize.html

================================================================================
来源：http://hz.guowangkeji.top/gtpmuhbcgm.html

R. Bash 专题
来源：http://hz.gzhubu.top/gtzhmtigfd.html

================================================================================
来源：http://hz.redwolf501.top/gtuvhaazhf.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtdzprmfdu.html

#!/usr/bin/env bash
来源：http://hz.guowangkeji.top/gtenzkooyz.html

set -euo pipefail
来源：http://hz.hysaishi.cn/gteafzccmd.html

[R02] 变量赋值与使用
来源：http://hz.jinqigfzy.top/gtpdfrqxjc.html

name="Tom"; echo "$name"
来源：http://hz.sxryk.cn/gtkixbgfpm.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtzfrgrqnn.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtvfkakjpb.html

[R04] 位置参数
来源：http://hz.daria6918.cn/gteucppypw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hfpthk.cn/gtocoadbbh.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtsyaubkfy.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtggmiugva.html

[R06] 判断命令是否存在
来源：http://hz.jqgfzy.top/gttxtsltwb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtjmdvphnr.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gthybqtfid.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtdrspwbab.html

[R08] 数值比较
来源：http://hz.xuetiantiany.cn/gtieimfxjb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenzaomai.com/gtrfplqotn.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gthnhfqlzu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gteresqezg.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gtjbqykixr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtmtdlbeeo.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtjwoqztxl.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtbkzfpnub.html

start) echo "启动" ;;
来源：http://hz.pengpengdd.cyou/gtljnihbal.html

stop)  echo "停止" ;;
来源：http://hz.jlsjyb.cn/gtkkmdgomk.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtudgqsjuv.html

esac
来源：http://hz.jinqigfzy.top/gtzfaaxvxo.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtgpxlydqr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtywgqknfz.html

[R13] for 计数循环
来源：http://hz.sufxvd.cn/gtbiwxzcgr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtupasgjbf.html

[R14] C 风格 for
来源：http://hz.haohaochexian.top/gtuntibqqu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtvsfsnqkd.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtepgauthw.html


<!-- 参考信息 -->