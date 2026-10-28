代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtybpevkee.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gtewwsbzyn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jyoumei.cn/gtlzatijjb.html

Ruby: // fork 块
来源：http://hz.hnxiangtu.top/gtmrlpjmoc.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtptujppzb.html

================================================================================
来源：http://hz.jinqigfzy.top/gthjthqpal.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtvwlxmnjb.html

================================================================================
来源：http://hz.tanke756.top/gtqsjnpdnq.html

[P01] 生成 UUID
来源：http://hz.9152youxi.cn/gtunlftirq.html

Py:   str(uuid.uuid4())
来源：http://hz.ywan-chungtsiang.top/gtcptmaswv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gtgkrdjibf.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gttgxbzqay.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtfbuteomw.html

Java: UUID.randomUUID().toString()
来源：http://hz.tianlin.xyz/gttbiekksd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sweek.top/gtrbnnnqkb.html

Ruby: SecureRandom.uuid
来源：http://hz.yongpay.top/gtkpwgyiyd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shzxlz.cn/gtutkjwuwl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtmirmpdla.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtydjgpaiy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtdnoriucy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.svipenyu.cn/gtqhquegjy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtanfwyfwh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.kuanghao11.cn/gtcpplffia.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yueranfly.top/gttzhqnmun.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gtwijtqvad.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.birdmap.top/gthhanbkug.html

[P03] 生成短随机字符串
来源：http://hz.xylfe.cn/gttimhacxh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shangyingyoupin.top/gtpepwgzhm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.52xcode.cn/gtxmlqomtn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtpbsjzdnz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtarfvjdsn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangshuangyany.cn/gtlmhyaukz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.kuanghao11.cn/gtffhjtuvv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gtksmtyftb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydjk.org.cn/gtlawsxosx.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtzesezhmi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dianchejie.cn/gtpaysbwnp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtcrwgexrf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gthlipuiep.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtgjpttgwz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shzxlz.cn/gteircdczk.html

Go:   len(arr);  len(m)
来源：http://hz.hammf.cn/gtyisiscen.html

Ruby: x.length;  x.size
来源：http://hz.hfpthk.cn/gthkdpfher.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtcknmsika.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtnhpzsoeb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gtsekmydjg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gteraoljav.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.quarkkingdee.top/gtpihwtcws.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gtdsmuffkx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtrlijjzit.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtmhdxvteb.html

Ruby: a == b
来源：http://hz.birdmap.top/gtqosncaqr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtylptqmre.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258888.top/gtquorkjtn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtcmvuaarl.html

PHP:  if (empty($x)) {}
来源：http://hz.tian-w.cn/gtuqwhbadh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.0kj1m.cn/gtbdqbkkvo.html

TS:   if (x == null) {}
来源：http://hz.tian-w.cn/gtzvafguil.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtwjtwwghu.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gtphmnjlym.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinyuanbaomall.cn/gtxisghaba.html

C#:   if (x is null) {}
来源：http://hz.jinqigufen.top/gtzszmrfar.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtrueagbgk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtrkbefjaj.html

PHP:  // 手写时间戳比较
来源：http://hz.jianghu66.top/gtpkorlzpb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtpjxvnzuw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtfvdowblp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gtvgkdhinf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtmbobxrcl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtoaopxkpa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gtexvyusyd.html

[P08] 处理浮点精度问题
来源：http://hz.gogol.net.cn/gtomnpplze.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gtnnnjbxlv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnqzz.top/gtjudsaznb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangtech.top/gtqhemdjib.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtmiuwbbxj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtsztycvao.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtcuwrqlsa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258888.top/gtaowaqiqn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gtcmxxohio.html

================================================================================
来源：http://hz.daxiang520.top/gtjfwkrjyd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aizwys.cn/gtggcgbrsi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrdreoixp.html

[Q01] 创建表
来源：http://hz.shanyushiyangtech.top/gtcxuoepbf.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtpoeezppf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gttqyuuwzn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtcxdignwh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aizwys.cn/gtddaamzap.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgfzy.top/gtcpsbzpsh.html

);
来源：http://hz.hysaishi.cn/gtgsdcbfgv.html

[Q02] 创建带外键的表
来源：http://hz.jlsjyb.cn/gtuvlzodcu.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gtatszckrc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtolnjzaoi.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtdekelhnb.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtrvxqepdf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.316326.xyz/gtxnjebsia.html

);
来源：http://hz.jiagoushi.top/gtovrcvygh.html

[Q03] 增加列
来源：http://hz.zhiwuduotai.top/gtxcwhtirz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hywenlv.cn/gtmlgmvsss.html

[Q04] 修改列类型
来源：http://hz.ydzc1.top/gtytdfjnux.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cashguo.top/gthtcjuhcx.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtouwprtey.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gtjleukbkd.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtyamfalpd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenlongwang.top/gtefchpdxz.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gtshzcgmrv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtisvkedxx.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gtivecnbpt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtpfokjsaz.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtwkfpsoor.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sxryk.cn/gtzfqruipb.html

[Q10] 插入单行
来源：http://hz.yuxming.cn/gtrwntnbwq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnqzz.top/gtjjmrmnlf.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtrfmvsvrs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtravkqshs.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtinrmmsjq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xinyue.icu/gtxamqkisq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuetiantiany.cn/gttowvaemv.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtlnqprkhc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gtyyatsngo.html

[Q14] 存在则更新（upsert）
来源：http://hz.ppjwa.cn/gtfrewkwtu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtpctcqjmh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zycfv.cn/gtooqpeyxe.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtmiviibbc.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtptovbphd.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtrigalhrx.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtrualiyvw.html

[Q17] 条件查询
来源：http://hz.tanke756.top/gtdagwhvdc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gthrfzkngl.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtveudndam.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangshuangyany.cn/gtxfaowfkh.html

[Q19] 范围查询
来源：http://hz.zhaomingkeji.xyz/gtfjaethsd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtcjhiegsv.html

[Q20] IN 列表
来源：http://hz.vqdsnc.cn/gtucfwjehx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gtnvrsyubj.html

[Q21] 空值判断
来源：http://hz.hongshengwenyu.top/gtaopvpylg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtignaveml.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gttkqodyqg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtkcmsdgcb.html

[Q23] 分页
来源：http://hz.zhoulong.xyz/gtvidpnevx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtjgrtqwxl.html

[Q24] 去重
来源：http://hz.gzhubu.top/gtftcxqzdf.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gtfgzjemlu.html

[Q25] 只取前 N 条
来源：http://hz.mhx1999.top/gtgaxtuzlv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangtech.top/gtyzmdwkkr.html

[Q26] 计数
来源：http://hz.dashuyun.cn/gtlnqjqxke.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtdofbdeea.html

[Q27] 条件计数
来源：http://hz.cashguo.top/gtmshjirrj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tian-w.cn/gtjslbtnet.html

[Q28] 求和与平均
来源：http://hz.tianlin.xyz/gtutkxkbpc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtxpmzgmpw.html

[Q29] 最大最小值
来源：http://hz.yuanzhike.top/gtkspplpto.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daria6918.cn/gtmdmcceuw.html

[Q30] 分组统计
来源：http://hz.316326.xyz/gtzevudokf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtajpaaris.html

[Q31] 分组后过滤
来源：http://hz.daxiang520.top/gtmpsnwewa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jlsjyb.cn/gtzclhtgmg.html

[Q32] 分组拼接字符串
来源：http://hz.shzxlz.cn/gtwkulmoah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtkaasiopm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj202588.top/gtwkziqzow.html

[Q33] 多列分组
来源：http://hz.tianlin.xyz/gtutfgpkrt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sysykeji.top/gttrtiaxdt.html

[Q34] 每组取第一条
来源：http://hz.guowangkeji.top/gtqwrqqqfq.html

SELECT * FROM (
来源：http://hz.jlsjyb.cn/gtnserczdz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daxiang520.top/gtvhrkvlqx.html

) t WHERE rn = 1;
来源：http://hz.9152youxi.cn/gtkiwatswx.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtgxwfftxc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtqwcvkrrq.html

[Q36] 左连接
来源：http://hz.yangfankeji.com/gtlhkdsxhr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtyqowypfg.html

[Q37] 右连接
来源：http://hz.snrcjt.cn/gtzqkmhmbq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hammf.cn/gtyijaezwa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tianlin.xyz/gthlefmdli.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydzc1.top/gtswmnlsqs.html

[Q39] 自连接（查上下级）
来源：http://hz.ehwqpu.com/gtauwbczmk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.svipenyu.cn/gtddlendwm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuanzx.com/gtkbxncedn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtyscyjmqw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ywan-chungtsiang.top/gthttnpkoe.html

[Q41] 多表连接
来源：http://hz.zhengqikj.top/gtealhncsq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtfqhxktlv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtvkckfwyn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydjk.org.cn/gtbnuwmmbd.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtkcpuhdvt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhoulong.xyz/gtcxwsosbo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cdnleiting.top/gtsenuhawn.html

[Q43] 标量子查询
来源：http://hz.redwolf501.top/gtzhuqaftw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtyaojgmvl.html

[Q44] IN 子查询
来源：http://hz.yuxming.cn/gtjnylhuwr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.316326.xyz/gtlrpdnueu.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtuuooyouk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtxrryuqkd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtlffzffnb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtrkrizrxk.html

[Q47] 与平均值比较
来源：http://hz.smart0.xyz/gthwmwxook.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.guannengcc.top/gtsnslbkkt.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtdyhfaiqp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xingfuxueyuan.xyz/gtuogpdcny.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jqgufenzy.top/gttetnakxq.html

[Q49] 更新单行
来源：http://hz.0kj1m.cn/gtimyizfed.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.redwolf501.top/gtomzaiupg.html

[Q50] 批量更新
来源：http://hz.ydjk.org.cn/gtlyvzahyy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cashguo.top/gthdipybrn.html

[Q51] 用子查询更新
来源：http://hz.nanxinkj.top/gthfgjgiim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtafqjsfjb.html

[Q52] 删除指定行
来源：http://hz.52xcode.cn/gtyrwqbidz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtisqifnls.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtjywnuqek.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.52xcode.cn/gtorxzpbqa.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtuykzwyxe.html

TRUNCATE TABLE logs;
来源：http://hz.jinyuanbaomall.cn/gtuoplejdw.html

[Q55] 排名（并列占位）
来源：http://hz.pycfn.com/gtpavwzeut.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenjidiqi.icu/gtogkfddep.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gttjprceco.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuanzhike.top/gtzoihnrhf.html

[Q57] 行号
来源：http://hz.jinqigufen.top/gtbgzcmjjl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jlsjyb.cn/gtgagqnmyr.html

[Q58] 累计求和
来源：http://hz.jinqigfzy.top/gthyawiaim.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fzhhl.top/gtgrpbwjud.html

[Q59] 分组内累计
来源：http://hz.jianghu66.top/gtckpmwxxc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtqnrzanig.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxuanxn.top/gtxjypovsn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hfpthk.cn/gtcymszwap.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenjidiqi.icu/gtxxmvonyw.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtofksvxri.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtarngyblx.html

[Q62] 分组占比
来源：http://hz.chenjidiqi.icu/gteunipjtr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtfdyuaywn.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtkgwrlqec.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zdqjudy.top/gttiiwtwzr.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtcvbehgnt.html

COMMIT;
来源：http://hz.dashuyun.cn/gthosrxmev.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtnvkqmosm.html

ROLLBACK;
来源：http://hz.zhengqikj.top/gtgsdclbim.html

[Q66] 行锁查询
来源：http://hz.iojbl.cn/gtcypctpne.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtikdvslbf.html

[Q67] 设置隔离级别
来源：http://hz.sxryk.cn/gtakzfobnx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tian-w.cn/gtzcouyesz.html

[Q68] 保存点
来源：http://hz.smart0.xyz/gtgjujwbvl.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gtnwdajxhk.html

ROLLBACK TO sp1;
来源：http://hz.jqgfzy.top/gtoahkicab.html

[Q69] 查看执行计划
来源：http://hz.zhengqikj.top/gtockfjygv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gogol.net.cn/gtbrroxxvf.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gttvtbjbdo.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gtanisxche.html

[Q71] 查看建表语句
来源：http://hz.havefunace.top/gtbtjttqlw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtjgbqdnjz.html

[Q72] 查看索引
来源：http://hz.daxiang520.top/gtutmxkhxz.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtxzepanrq.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gtyumriqbv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.birdmap.top/gtgypgymeg.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtrcpwjdli.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.kuanghao11.cn/gtwovnrlja.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtpzjztxfs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuxming.cn/gttowkoxhy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.redwolf501.top/gthivalntr.html

[Q76] 按天统计
来源：http://hz.smart0.xyz/gtdskyqita.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xylfe.cn/gtwlgomiks.html

[Q77] 时间加减
来源：http://hz.9152youxi.cn/gtdyptobpq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtuegogboe.html

[Q78] 当前时间
来源：http://hz.mhx1999.top/gtsjngvjyv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xingfuxueyuan.xyz/gtgbfcclrn.html

[Q79] 字符串拼接
来源：http://hz.ydzc1.top/gtubfspiqn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuetiantiany.cn/gtrkepfzpo.html

[Q80] 字符串截取
来源：http://hz.xingfuxueyuan.xyz/gtjgagipuh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtgmckcadg.html

[Q81] 字符串替换
来源：http://hz.daxiang520.top/gtxnbmfctp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtouurllno.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtgtxyxvqd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guannengcc.top/gtyasyivvz.html

[Q83] 大小写转换
来源：http://hz.cashguo.top/gtksekydnb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtpnmexpjg.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtmewfpfxl.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhongyouzk.top/gtmwnmhexa.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtnrfjjkyx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.c1oappe.top/gtlpvnulcv.html

[Q86] 读取 JSON 字段
来源：http://hz.ywan-chungtsiang.top/gtocovwspr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtsadlycqe.html

[Q87] JSON 字段做条件
来源：http://hz.jqgufenzy.top/gtkaagcjuv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtzjbkrppi.html

[Q88] 行转列（条件聚合）
来源：http://hz.cucudq.cn/gtjcwqwvlg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhongyouzk.top/gtpqergqxl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtpwhmrzsl.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtvkhywfgi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxinkj.top/gtggtyqzep.html

[Q90] 生成序号列
来源：http://hz.fzhhl.top/gtndvlqxdz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtltqnkdcf.html

================================================================================
来源：http://hz.ppjwa.cn/gtjuonffoj.html

R. Bash 专题
来源：http://hz.zycfv.cn/gtelxejuoz.html

================================================================================
来源：http://hz.jyoumei.cn/gtmkwjetrt.html

[R01] shebang 与严格模式
来源：http://hz.meibo888.top/gtoydsrkno.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gtaiuvooom.html

set -euo pipefail
来源：http://hz.tian-w.cn/gtborhctjo.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtjotrjjul.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtxiyckjsa.html

[R03] 只读变量
来源：http://hz.jinqigfzy.top/gtoqpswohh.html

readonly PI=3.14
来源：http://hz.jyoumei.cn/gtfpcwhkfg.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gtutfkyapj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtxdwuvrvm.html

[R05] 参数默认值
来源：http://hz.aibaodan.cn/gtqkiavenj.html


<!-- 参考信息 -->