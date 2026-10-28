代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtwopyxvpt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gtgnfkhzzq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gthnhsmbha.html

Ruby: // fork 块
来源：http://hz.wangshuangyany.cn/gtjxlyyzsu.html

C#:   Parallel.For
来源：http://hz.dianchejie.cn/gttfguctzo.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfzqgvxff.html

P. 常用工具函数
来源：http://hz.gzhubu.top/gtabtpfmpv.html

================================================================================
来源：http://hz.yonumen.top/gtkstkxvpy.html

[P01] 生成 UUID
来源：http://hz.sufxvd.cn/gtidwrptol.html

Py:   str(uuid.uuid4())
来源：http://hz.bjfxy.top/gtcrxwexmw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tian-w.cn/gtrgvwpojg.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtdzcqmxwz.html

TS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gttujwjxfz.html

Java: UUID.randomUUID().toString()
来源：http://hz.sxryk.cn/gtpshfkvqq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hysaishi.cn/gtsqqhsaey.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtxuapujhg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtealgtoqv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guowangkeji.top/gtylyjkplc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zdqjudy.top/gtxqyskdns.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.quarkkingdee.top/gtgswcwgcg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtivtfwtnt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jiagoushi.top/gtrtrtrwgn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aizwys.cn/gtuyncmgfy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtdtumgwhf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtbzocppre.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtadwbgykn.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtvsgfxbrf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gtzxinkwhp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtmscpoids.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtaycarrfc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtaefcgrsx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.svipenyu.cn/gtagoiwjpu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gthyhuwdrw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.havefunace.top/gtvenubafp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgfzy.top/gtckapyxdb.html

[P04] 求长度
来源：http://hz.shzxlz.cn/gtpiucsgjq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtimrhrokj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gthkflthbb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtacgjljhz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtozsvnymq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtxiwgkiqk.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtpugjtzca.html

Ruby: x.length;  x.size
来源：http://hz.chenlongwang.top/gtvpbjdgnr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtaahzyrel.html

[P05] 判断两个对象内容是否相等
来源：http://hz.mhx1999.top/gtkchkdwre.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gtjadmesbs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sufxvd.cn/gtrgmvwyrt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gogol.net.cn/gtovkcdxny.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtclgjsbbf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gthaiakjbz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtlpqvyxtp.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtyvvikajf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangdashe.top/gtnqnwjxwc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gticitnbwj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtsfnhwkyi.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gtrpnitwfu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yongpay.top/gtqtvwyeto.html

TS:   if (x == null) {}
来源：http://hz.dianchejie.cn/gtizkzivyi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guannengcc.top/gthcdmqyyd.html

Go:   if x == nil {}
来源：http://hz.pengpengdd.cyou/gtwlurvahy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.quarkkingdee.top/gtqxwpjryd.html

C#:   if (x is null) {}
来源：http://hz.jinqigfzy.top/gtrofkkxvr.html

[P07] 防抖与节流
来源：http://hz.shuidangran.top/gtdswhnxvm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtsvtvbtyr.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtztlkzkbx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtijhaizao.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtyqyjihwa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.redwolf501.top/gtdrnxgylz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtfxpdrxiq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gttqhvfnfq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj20258888.top/gtvpzdyvsg.html

[P08] 处理浮点精度问题
来源：http://hz.iojbl.cn/gtzkntcxkv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cdnleiting.top/gtlngubqjq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gtnouaijim.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangkeji.top/gthpyarkhv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jyoumei.cn/gthkyhuiaq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yvedp.cn/gtysscumhz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtaggxvrds.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtkuicyhas.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtbaywrpih.html

================================================================================
来源：http://hz.fzhhl.top/gtdxarcagv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yanxiufei.cn/gtxfrynbyy.html

================================================================================
来源：http://hz.andypj.xyz/gtsltrdprl.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gtbdrmtcnb.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtomalynnm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtmnnqhhvl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtwoqqgqor.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhijiandao.cn/gtnslmgzsa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangkeji.top/gtgmbaanjz.html

);
来源：http://hz.fengsongda.top/gtyoptjbko.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gtxtsdfrxe.html

CREATE TABLE orders (
来源：http://hz.chenlongwang.top/gthasxsjji.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtbsgeaohv.html

user_id INT NOT NULL,
来源：http://hz.hnqzz.top/gtfjhqrvqo.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gttlojrabj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtwkypgbkk.html

);
来源：http://hz.chenzaomai.com/gtbsvzxymd.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtxyvcsnsd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtqfjcvqfo.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtqfzqtgmn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtrzqtxhdw.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtjespgqal.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtnohynfad.html

[Q06] 删除列
来源：http://hz.cashguo.top/gttnwtjtvu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yueranfly.top/gtaoetfzum.html

[Q07] 删除表
来源：http://hz.xinyue.icu/gteybmzekw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shuidangran.top/gtrdqomuob.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtezsherag.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtsohddbxa.html

[Q09] 创建唯一索引
来源：http://hz.guowangkeji.top/gtcugwtjlb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xinyue.icu/gtjsvbtouo.html

[Q10] 插入单行
来源：http://hz.fzhhl.top/gtlqbwmpfq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtaetdoddj.html

[Q11] 一次插入多行
来源：http://hz.ybcxt.top/gtlwsjxqdq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xziqi.cn/gtfuqyhtae.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258888.top/gtntzabqsj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtxbadvhjg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tian-w.cn/gtyzoihitn.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtxuabulcr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.haohaochexian.top/gtrxmbobfu.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtkkttrayl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hfpthk.cn/gtbwbfgozb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenlongwang.top/gthscbiezg.html

[Q15] 查询全部
来源：http://hz.jinghuilouyu.cn/gtfaiwzujl.html

SELECT * FROM users;
来源：http://hz.ivvv.top/gthpgndslh.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtnloruuhw.html

SELECT id, name FROM users;
来源：http://hz.xuetiantiany.cn/gttrccrltx.html

[Q17] 条件查询
来源：http://hz.jyoumei.cn/gtqkxeagfa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yongpay.top/gtmhsmlizj.html

[Q18] 模糊匹配
来源：http://hz.pycfn.com/gtvqcmazeh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shuidangran.top/gtitqaltjl.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtsfscyueb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtqvpkzgzd.html

[Q20] IN 列表
来源：http://hz.zdqjudy.top/gtiujnyuus.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhengqikj.top/gtjcvdmexg.html

[Q21] 空值判断
来源：http://hz.hysaishi.cn/gtpdtrycoq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shangyingyoupin.top/gtnpafqgri.html

[Q22] 排序
来源：http://hz.316326.xyz/gtpezozwdk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgufenzy.top/gtdbbstkep.html

[Q23] 分页
来源：http://hz.jyoumei.cn/gtjeowgbyu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.svipenyu.cn/gtisgadgac.html

[Q24] 去重
来源：http://hz.pengpengdd.cyou/gtowbummzj.html

SELECT DISTINCT city FROM users;
来源：http://hz.gotoacloud.top/gtuqhdbuhg.html

[Q25] 只取前 N 条
来源：http://hz.hnxiangtu.top/gteveibqwq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtuoimpgck.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtszchqrvz.html

SELECT COUNT(*) FROM users;
来源：http://hz.iojbl.cn/gtajlwpesk.html

[Q27] 条件计数
来源：http://hz.redwolf501.top/gtultlulfh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sweek.top/gtqzoscevx.html

[Q28] 求和与平均
来源：http://hz.wangdashe.top/gtescpgzre.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtcjdrujsm.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gtmmjipvzi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gttubokeej.html

[Q30] 分组统计
来源：http://hz.hfpthk.cn/gtiinkovyg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtjppencoe.html

[Q31] 分组后过滤
来源：http://hz.xingfuxueyuan.xyz/gtjduyjygq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtjvjentdx.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtxxyaexwm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtopidcdxf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtbfzvkcth.html

[Q33] 多列分组
来源：http://hz.wangshuangyany.cn/gtckigmjkg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ybcxt.top/gtbreitlyk.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtlrsiblin.html

SELECT * FROM (
来源：http://hz.vqdsnc.cn/gtijwzwsjh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gteleghszo.html

) t WHERE rn = 1;
来源：http://hz.yongpay.top/gtkyvctvdr.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtkesmupsu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gthhoopoot.html

[Q36] 左连接
来源：http://hz.guannengcc.top/gttbmpqhse.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aibaodan.cn/gtnrhwtsbi.html

[Q37] 右连接
来源：http://hz.nanxinkj.top/gteodqfmml.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xinyue.icu/gtcjbcidxc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgfzy.top/gtkmujqpbs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.mhx1999.top/gtfaqsyiwi.html

[Q39] 自连接（查上下级）
来源：http://hz.ywan-chungtsiang.top/gtbvfxknil.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigufen.top/gtaykhdnbx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxinkj.top/gtugiiqqrr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hammf.cn/gtpjjqzwbt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinghuilouyu.cn/gtmnaimsrt.html

[Q41] 多表连接
来源：http://hz.jinqigfzy.top/gtbcjmyswh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hammf.cn/gtsewkpbxk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtewzpxpuo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinyuanbaomall.cn/gtnsdpbigb.html

[Q42] 连接条件附加过滤
来源：http://hz.smart0.xyz/gtsdozoqqz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gtpwfgloul.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gthjznsxcr.html

[Q43] 标量子查询
来源：http://hz.cheryme.top/gtzkxmyogp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gteaggwgut.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtufclpyef.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ywan-chungtsiang.top/gtekqcozxj.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtofptzkdd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtzyzpdbic.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sysykeji.top/gtvmixbopn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtaaigpaqt.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gtlrrqzwos.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtapfatdrz.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gtapooomnl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtmtdwwtvi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtwrxrukgx.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtaumrvbyx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj202588.top/gttjbyuiej.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtnimashtu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zdqjudy.top/gtwtexcazw.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gtsupavcor.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.c1oappe.top/gtctsdxgur.html

[Q52] 删除指定行
来源：http://hz.aizwys.cn/gtopeaqacy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.bjfxy.top/gtztrfmfbb.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtocsbdnrl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.bjfxy.top/gtwtdcgnlw.html

[Q54] 清空表
来源：http://hz.zdqjudy.top/gtmiormmng.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gtldtllqww.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gthjkrxlas.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hywenlv.cn/gtneylytcb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dashuyun.cn/gthgaxygbs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yangfankeji.com/gthuequmrs.html

[Q57] 行号
来源：http://hz.aizwys.cn/gtsriwmdnb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj202588.top/gtsmeitlch.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtsoxracki.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xylfe.cn/gthkiisjpx.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtnfeyituz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aibaodan.cn/gtapfwqdry.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtbihxdjvj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtthkatlcx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtfraoqsdx.html

[Q61] 移动平均
来源：http://hz.chenlongwang.top/gtqmrrvwfg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ppjwa.cn/gtrboddaob.html

[Q62] 分组占比
来源：http://hz.wangshuangyany.cn/gtcucerjvk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtltqsespd.html

[Q63] 开启事务
来源：http://hz.jinyuanbaomall.cn/gtytzqyxug.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cdnleiting.top/gtuhjzivsh.html

[Q64] 提交事务
来源：http://hz.guowangkeji.top/gtypazpibf.html

COMMIT;
来源：http://hz.yangfankeji.com/gthbtllork.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gtidisqedq.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtlgnarczn.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtlyvkjvmw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xinyue.icu/gthjewrcns.html

[Q67] 设置隔离级别
来源：http://hz.zhongyouzk.top/gtybfdwerw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtrnvjuecn.html

[Q68] 保存点
来源：http://hz.shanyushiyangtech.top/gtvzmqydkf.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtqaqmbcnm.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtxjbzhgnh.html

[Q69] 查看执行计划
来源：http://hz.zycfv.cn/gtqxkwbprn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxuanxn.top/gthvhxvbxr.html

[Q70] 更新统计信息
来源：http://hz.zhaomingkeji.xyz/gtmrlcfade.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtrscoklat.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gtgbjlzioe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gteomwyojk.html

[Q72] 查看索引
来源：http://hz.9152youxi.cn/gtspwbbxjp.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gtkflatwmi.html

[Q73] 查看表状态
来源：http://hz.jinghuilouyu.cn/gtmmrgoohg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nwbrower.top/gtwdyednow.html

[Q74] 强制使用索引
来源：http://hz.9152youxi.cn/gtgjyimjyi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtusrergah.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtgxayszhe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yanxiufei.cn/gtjkkzylsx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnxiangtu.top/gtkljmmijn.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtcltaftfp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.iojbl.cn/gtquevanyl.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gttzxhgkoc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cucudq.cn/gtctqlswfr.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtklblkwhd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhiwuduotai.top/gtbwxlcoog.html

[Q79] 字符串拼接
来源：http://hz.ydzc1.top/gtczdubrxv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hysaishi.cn/gtuivabdto.html

[Q80] 字符串截取
来源：http://hz.ybcxt.top/gtttututfa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtkwwrudoz.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtcmdctahi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hywenlv.cn/gtjwvxghir.html

[Q82] 字符长度与字节长度
来源：http://hz.zhijiandao.cn/gtobsugqft.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cashguo.top/gtwhgvoexx.html

[Q83] 大小写转换
来源：http://hz.quarkkingdee.top/gtdprpzlba.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtpcwypiwo.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtyluexvzi.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtmxslimye.html

[Q85] 数值取整
来源：http://hz.yuanzhike.top/gttzpxgolk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtkffkaotb.html

[Q86] 读取 JSON 字段
来源：http://hz.gzhubu.top/gtsekeaaok.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gaohongyu789.top/gtdikrynnx.html

[Q87] JSON 字段做条件
来源：http://hz.jlsjyb.cn/gtxbbbmxvf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtouvrjpov.html

[Q88] 行转列（条件聚合）
来源：http://hz.dashuyun.cn/gtnfehcqzt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtrlwozwyx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hfpthk.cn/gtpyhrpnxm.html

[Q89] 判断表是否存在
来源：http://hz.sysykeji.top/gtvrbkltzd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj202588.top/gtxuwhjeqp.html

[Q90] 生成序号列
来源：http://hz.wangshuangyany.cn/gtshkrwrqa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtmzyacegu.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtulezrwsr.html

R. Bash 专题
来源：http://hz.jinghuilouyu.cn/gteasmxxmi.html

================================================================================
来源：http://hz.shzxlz.cn/gtzaftmrgb.html

[R01] shebang 与严格模式
来源：http://hz.sufxvd.cn/gtrugcelmd.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtwgjovrmz.html

set -euo pipefail
来源：http://hz.ydzc1.top/gtvqgqjfgh.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtwsonhfpv.html

name="Tom"; echo "$name"
来源：http://hz.ywan-chungtsiang.top/gtglcxkmrz.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gtmzvowcqk.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gtnbupgjnz.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtvxcygciq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jyoumei.cn/gtohmcruzr.html

[R05] 参数默认值
来源：http://hz.shuidangran.top/gtzxowbkoz.html


<!-- 参考信息 -->