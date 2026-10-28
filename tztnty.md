代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtjfekiocf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj20258888.top/gtuutagilb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gtrgqfnqnp.html

Ruby: // fork 块
来源：http://hz.yj20258.top/gtshovhioz.html

C#:   Parallel.For
来源：http://hz.xziqi.cn/gtyaahfuds.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjhsvcxnc.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtucknylky.html

================================================================================
来源：http://hz.havefunace.top/gtajbedqkt.html

[P01] 生成 UUID
来源：http://hz.xinyue.icu/gtoleltkwu.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtvwmydrcs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shuidangran.top/gtgkolpqna.html

JS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtppaacuyo.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtznngxvkb.html

Java: UUID.randomUUID().toString()
来源：http://hz.yongpay.top/gtmeonvcxj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtqnenyyfj.html

Ruby: SecureRandom.uuid
来源：http://hz.fengsongda.top/gtlqnzgmby.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sufxvd.cn/gtcdajdpli.html

[P02] MD5 / SHA256 摘要
来源：http://hz.mhx1999.top/gtngwtglqo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.feifeiyinyue.top/gtfhstkefy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hongshengwenyu.top/gtafdfsewj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtsbksirbg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtmwuyzbix.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.9152youxi.cn/gtwdpxfkfi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sxryk.cn/gtaefgyqau.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gtrsouhzna.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.birdmap.top/gtxgrmdnbj.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtxlnlrsim.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ppjwa.cn/gtsbytrdsm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtmucmuqnb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtmpgrenet.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtpjazbspr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.iojbl.cn/gtpacknhap.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hongshengwenyu.top/gthhfypgsw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ywan-chungtsiang.top/gtxbtirodb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtepfrfmfb.html

[P04] 求长度
来源：http://hz.bjfxy.top/gtmvyapsst.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgfzy.top/gtioobecyf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtxwvohdkp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtcpmwvagj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtycbqmces.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zdqjudy.top/gtmrhqxykm.html

Go:   len(arr);  len(m)
来源：http://hz.jiagoushi.top/gtbjasiibq.html

Ruby: x.length;  x.size
来源：http://hz.zhoulong.xyz/gtpyxcqmir.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gaohongyu789.top/gtbodilrmo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtbxevmrpn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gtwckxxhtc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtfgbyybti.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydzc1.top/gtpygtsotw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtmdilekaw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tanke756.top/gtljafxfle.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guowangkeji.top/gtewkfvydh.html

Ruby: a == b
来源：http://hz.ydzc1.top/gtdkbpizrq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gteiwswsyk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gtmizevrmm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.meibo888.top/gtosddohnm.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gtzlbfzywu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dianchejie.cn/gtergeyugb.html

TS:   if (x == null) {}
来源：http://hz.hnxiangtu.top/gthuzpupom.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtzspsathl.html

Go:   if x == nil {}
来源：http://hz.jqgufenzy.top/gtfurrpjgi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtztvabyaq.html

C#:   if (x is null) {}
来源：http://hz.hammf.cn/gtmwlqhbka.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtaatihqsp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258888.top/gtmhqdelsc.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtntdhnkld.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtywldkill.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtyuxaukvb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtzpijnlfx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ehwqpu.com/gtwofuydto.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.quarkkingdee.top/gtfygmfwsf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtsattskxw.html

[P08] 处理浮点精度问题
来源：http://hz.hysaishi.cn/gtnbumkyqo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fzhhl.top/gtxxwvtrsp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shangyingyoupin.top/gtmgioequo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtyxfthhho.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pengpengdd.cyou/gtmvsqqjju.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yueranfly.top/gtspslstmq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtiiaplthi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cdnleiting.top/gtmktuypqj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cashguo.top/gtypxqqnwa.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxonxlwnk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtkzlvebwm.html

================================================================================
来源：http://hz.hnqzz.top/gtvaldezla.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtanwrajib.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtisdgtqvb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuanzhike.top/gtnvlgauba.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtfxucykle.html

email VARCHAR(100) UNIQUE,
来源：http://hz.9152youxi.cn/gttgcgabzm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj202588.top/gtqmwwnbxd.html

);
来源：http://hz.havefunace.top/gtzuikdjzu.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtudcheuhv.html

CREATE TABLE orders (
来源：http://hz.shangyingyoupin.top/gtcicbrkrs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtpgerramh.html

user_id INT NOT NULL,
来源：http://hz.yanxiufei.cn/gtozooamng.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtjhvqjvpx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuanzx.com/gtvrgwlyth.html

);
来源：http://hz.9152youxi.cn/gtsuiwaayj.html

[Q03] 增加列
来源：http://hz.zhongyouzk.top/gtctprjnzg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydzc1.top/gtcyvswswh.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gttyamcxln.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sweek.top/gtblenyprc.html

[Q05] 重命名列
来源：http://hz.pengpengdd.cyou/gtahcrdeox.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtupindmdr.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtaaxnmhbt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtjyaeansa.html

[Q07] 删除表
来源：http://hz.hysaishi.cn/gtjyfncvaf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.svipenyu.cn/gtrexintvv.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gtsmwsszaq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gtzcwnyvev.html

[Q09] 创建唯一索引
来源：http://hz.guannengcc.top/gtxohdpqar.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.smart0.xyz/gtxngqzpfp.html

[Q10] 插入单行
来源：http://hz.hfpthk.cn/gtlnsqvbmy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgfzy.top/gtsxgphxme.html

[Q11] 一次插入多行
来源：http://hz.bjfxy.top/gtiyuoflav.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gzhubu.top/gthglfhqsi.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gthspldcus.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtfmowxavl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangtech.top/gtdautujar.html

[Q13] 忽略重复插入
来源：http://hz.chenlongwang.top/gtslgzmvlv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daria6918.cn/gtyrkdplkw.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtjncymxhp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gtqkaxdbqw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gtyiqdevwh.html

[Q15] 查询全部
来源：http://hz.andypj.xyz/gtstaidrzl.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtswkapwua.html

[Q16] 查询指定列
来源：http://hz.daria6918.cn/gtblipgabp.html

SELECT id, name FROM users;
来源：http://hz.ehwqpu.com/gtieewnfue.html

[Q17] 条件查询
来源：http://hz.hongshengwenyu.top/gtofydutax.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuetiantiany.cn/gtcaboxeck.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gtbnskcovt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hfpthk.cn/gteelnahgq.html

[Q19] 范围查询
来源：http://hz.snrcjt.cn/gtsntflgtj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tianlin.xyz/gtnrmnatuw.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtdqihobua.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hysaishi.cn/gtllofptxf.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtjwebdxwg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtixxhlvhp.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtkyejxkxl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sweek.top/gtddlfqhhx.html

[Q23] 分页
来源：http://hz.wangshuangyany.cn/gtjzzazqlu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtjhpwcozy.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtodlknttr.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtiteiwbnn.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtlllxxcre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zdqjudy.top/gtdpmwidkr.html

[Q26] 计数
来源：http://hz.zhoulong.xyz/gtlzswzrtd.html

SELECT COUNT(*) FROM users;
来源：http://hz.tianlin.xyz/gtilzrnynw.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gthxaexgpl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jqgufenzy.top/gtythntbjx.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gttrphxfef.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtozijnguq.html

[Q29] 最大最小值
来源：http://hz.sysykeji.top/gtcclvajjn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.smart0.xyz/gtyzybqkyg.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtoumiwfei.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtgqmmrbcb.html

[Q31] 分组后过滤
来源：http://hz.gaohongyu789.top/gtblpsbgtr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuxming.cn/gtjvuvvwqu.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gtahagdwgf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtkvsmfvpm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.andypj.xyz/gtkdnzazpz.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtjadhjczu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtpnsuujut.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtrffeobvw.html

SELECT * FROM (
来源：http://hz.redwolf501.top/gtpdlnbghp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigufen.top/gtexkjxoag.html

) t WHERE rn = 1;
来源：http://hz.aibaodan.cn/gtozhuince.html

[Q35] 内连接
来源：http://hz.xingfuxueyuan.xyz/gttxoabrhs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtamjbfyug.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtpmqknooj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtrdtkfexd.html

[Q37] 右连接
来源：http://hz.cucudq.cn/gtyyznsooz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydzc1.top/gtnjbvacua.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtlgrntvat.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtpmozajlr.html

[Q39] 自连接（查上下级）
来源：http://hz.yanxiufei.cn/gtflnrcqzk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxuanxn.top/gtyylltwab.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gtlcredzdm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuetiantiany.cn/gtrjpomouw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jyoumei.cn/gtobcjphbx.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtpvdnnocq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtkiqgrvpv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtpcrtulto.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pycfn.com/gthfqtsdbo.html

[Q42] 连接条件附加过滤
来源：http://hz.yonumen.top/gtajhayvud.html

SELECT u.name, o.amount FROM users u
来源：http://hz.dashuyun.cn/gtzdpsuswq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hywenlv.cn/gtwdrdskvi.html

[Q43] 标量子查询
来源：http://hz.shangyingyoupin.top/gtyibhjusp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gtzdusdbjb.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtxdfxmhgj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daxiang520.top/gtrlzepgnm.html

[Q45] EXISTS 判断存在
来源：http://hz.xziqi.cn/gtlsliyfdm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtfnfescvy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhengqikj.top/gtrffxifja.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtekzlxysy.html

[Q47] 与平均值比较
来源：http://hz.jinqigufen.top/gtwdxlwweh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gtogzsktxl.html

[Q48] CTE 公用表表达式
来源：http://hz.0kj1m.cn/gtcortbcxv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtvuxrlkyv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinghuilouyu.cn/gtionfnqjb.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gtwemnqfbk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gtzikflaee.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gtleckyfvu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtwteybjqm.html

[Q51] 用子查询更新
来源：http://hz.gogol.net.cn/gtdhaknjnf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zycfv.cn/gtxotjymzl.html

[Q52] 删除指定行
来源：http://hz.yongpay.top/gtgdvqyfui.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gogol.net.cn/gtwatmjbtk.html

[Q53] 按条件删除
来源：http://hz.ydzc1.top/gtzmbkryzc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dianchejie.cn/gtdgxzpevp.html

[Q54] 清空表
来源：http://hz.xuetiantiany.cn/gtvlwspypp.html

TRUNCATE TABLE logs;
来源：http://hz.hongshengwenyu.top/gtswhevmwi.html

[Q55] 排名（并列占位）
来源：http://hz.hnqzz.top/gttmdnxadq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtsfamtqsg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gtsoydnxom.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tanke756.top/gtipcuzuxm.html

[Q57] 行号
来源：http://hz.yanxiufei.cn/gtkumlztta.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtecatvqjy.html

[Q58] 累计求和
来源：http://hz.wangshuangyany.cn/gtllzaptcv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtnpiifagv.html

[Q59] 分组内累计
来源：http://hz.nanxinkj.top/gtrkoqlfie.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gtohkpdaje.html

[Q60] 取上一行 / 下一行
来源：http://hz.jyoumei.cn/gtadckwmlg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnxiangtu.top/gtqbduorqk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuetiantiany.cn/gtjekrpydn.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtezmlttfv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtuqaqihjy.html

[Q62] 分组占比
来源：http://hz.yueranfly.top/gtmynehbgr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtfuikouhl.html

[Q63] 开启事务
来源：http://hz.sweek.top/gtxjdpeyhe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtaznonspr.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtveaybxxx.html

COMMIT;
来源：http://hz.dashuyun.cn/gtozogioeq.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtvofcruop.html

ROLLBACK;
来源：http://hz.chenlongwang.top/gtnjzxoupz.html

[Q66] 行锁查询
来源：http://hz.zycfv.cn/gtmfhhlulm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhijiandao.cn/gtdyxlrqqo.html

[Q67] 设置隔离级别
来源：http://hz.ydjk.org.cn/gtqweukzuj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinyuanbaomall.cn/gtgahzgqrs.html

[Q68] 保存点
来源：http://hz.yuxming.cn/gtvhfdvpjz.html

SAVEPOINT sp1;
来源：http://hz.dashuyun.cn/gtauekaosg.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtwuijoaps.html

[Q69] 查看执行计划
来源：http://hz.hfpthk.cn/gtoyzgycwz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hysaishi.cn/gtqfgwhuji.html

[Q70] 更新统计信息
来源：http://hz.fengsongda.top/gtbuqdlged.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtvcbsxumh.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gtycmeanvx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jianghu66.top/gtpummehka.html

[Q72] 查看索引
来源：http://hz.gotoacloud.top/gtzleixyzv.html

SHOW INDEX FROM users;
来源：http://hz.aibaodan.cn/gtandsubkf.html

[Q73] 查看表状态
来源：http://hz.ybcxt.top/gtskkifbhq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtijcgoeyr.html

[Q74] 强制使用索引
来源：http://hz.kuanghao11.cn/gtefjknkpl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sxryk.cn/gtsulkxzyc.html

[Q75] 日期格式化
来源：http://hz.0kj1m.cn/gtuwvnqjpy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtaovbpawe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtipgefstj.html

[Q76] 按天统计
来源：http://hz.mhx1999.top/gtzqadzzzy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtgexhbnvr.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtjoigwrqr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenzaomai.com/gtzstckbbh.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtoyzwgrex.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gtqktazklo.html

[Q79] 字符串拼接
来源：http://hz.yvedp.cn/gttpeqbtkb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtflrxwcrg.html

[Q80] 字符串截取
来源：http://hz.zhijiandao.cn/gtsgfjzipa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtpljoxpmn.html

[Q81] 字符串替换
来源：http://hz.wangdashe.top/gtivlmczur.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.9152youxi.cn/gtqohuaoas.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtowmgxjfw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ivvv.top/gtaqtcxkso.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtwuqjnvlx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtfzdprlvb.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gttvngoyfp.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtxwmofujn.html

[Q85] 数值取整
来源：http://hz.fengsongda.top/gthuigtvun.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtiddcedjy.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gtkstbvmbl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtpwzguwpf.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtckhhcuuw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.vqdsnc.cn/gtnyenpkbt.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gtlppeemhw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtvxhoxvgx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.svipenyu.cn/gteknwnyvz.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gtgdjbbpjb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gthwwucrnz.html

[Q90] 生成序号列
来源：http://hz.tianlin.xyz/gtrwjanmdr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtvcnqdkae.html

================================================================================
来源：http://hz.redwolf501.top/gtihhqkwhb.html

R. Bash 专题
来源：http://hz.ywan-chungtsiang.top/gtcfjixrjj.html

================================================================================
来源：http://hz.wangdashe.top/gtlmugzpfy.html

[R01] shebang 与严格模式
来源：http://hz.yj20258.top/gtzpuqdnds.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gtgxqmcyel.html

set -euo pipefail
来源：http://hz.zhoulong.xyz/gtredaaawl.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtzxommbrk.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtgjjpzwug.html

[R03] 只读变量
来源：http://hz.shangyingyoupin.top/gtykgbredn.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gtbpsnwvko.html

[R04] 位置参数
来源：http://hz.daxiang520.top/gtzmlnzvxv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtiudzixxp.html

[R05] 参数默认值
来源：http://hz.jinqigufen.top/gtvingdvin.html


<!-- 参考信息 -->