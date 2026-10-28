代发 wailian999

C#:   Parallel.For
来源：http://hz.yvedp.cn/gtefnfuevq.html

================================================================================
来源：http://hz.meibo888.top/gtsqbxrpsx.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gtzfbdhqsd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbgkbkeyv.html

[P01] 生成 UUID
来源：http://hz.meibo888.top/gtdobplbiq.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258.top/gteeodoyxk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gthqlzzxty.html

JS:   crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtpyxnmmkz.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtyeuuccfz.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangdashe.top/gtahusroxd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jianghu66.top/gtvyidvahd.html

Ruby: SecureRandom.uuid
来源：http://hz.gaohongyu789.top/gtmzwpokoo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.haohaochexian.top/gtcgtdmufm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.dianchejie.cn/gtmjvcxbrz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtzhqhdkhc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtlqldywxo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guowangkeji.top/gtjhgmniga.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuetiantiany.cn/gtrlsixmli.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtkzhyoiku.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tianlin.xyz/gtnyfxkmrg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yueranfly.top/gteykljqta.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aibaodan.cn/gthzyxfilg.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtcjjfygdt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gtbaqzrkhq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gttwfynimk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtdrxyzwxd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtomhhrnwb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gthztdjlvp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pycfn.com/gttnuuhtlf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuanzx.com/gtrcwoflur.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tianlin.xyz/gtgpnlapid.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtaumvgdxg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangdashe.top/gtyhplkben.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtjygymzbb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtcklkqhqg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtuocutuaj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shuidangran.top/gtfciceaqj.html

Go:   len(arr);  len(m)
来源：http://hz.c1oappe.top/gtfhdhvwly.html

Ruby: x.length;  x.size
来源：http://hz.haohaochexian.top/gtctpcqnyk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.c1oappe.top/gtubryyiae.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hywenlv.cn/gttoqihlej.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gttxhykgoj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.mhx1999.top/gtbtosydat.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhixingplan.top/gtwbpffgmb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtlthcaver.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.havefunace.top/gtxjgjglnu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cucudq.cn/gttcwglrrs.html

Ruby: a == b
来源：http://hz.yvedp.cn/gtwnlsmgzd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cqqwz.cn/gtzjcafwwg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.redwolf501.top/gtbbwrhuia.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ivvv.top/gthlopkygq.html

PHP:  if (empty($x)) {}
来源：http://hz.gotoacloud.top/gtufxwofmv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jianghu66.top/gtiqsmjyjc.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gthhblkxtm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hysaishi.cn/gthegsjzoo.html

Go:   if x == nil {}
来源：http://hz.cdnleiting.top/gtudnzzjpz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yanxiufei.cn/gtedsqosrr.html

C#:   if (x is null) {}
来源：http://hz.chenzaomai.com/gtuceettdc.html

[P07] 防抖与节流
来源：http://hz.ivvv.top/gtlqlqnuor.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuxming.cn/gtuafrykbt.html

PHP:  // 手写时间戳比较
来源：http://hz.yj202588.top/gtquhektaz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtoagammxk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtkvjojlel.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtllvqgree.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cdnleiting.top/gtjybmncvu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.kuanghao11.cn/gtbgwgxujz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gtsiwhxwke.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtpaiqwtti.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.kuanghao11.cn/gtzdgovtpd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtpcxlinjq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtbpsmvxjp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtzlhctqwo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xylfe.cn/gtqbxdjjpn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangkeji.top/gtzmmkiwlp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cashguo.top/gtmnropuhf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xylfe.cn/gtlpiyuocg.html

================================================================================
来源：http://hz.cashguo.top/gtmgrqutwc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtldfapsyw.html

================================================================================
来源：http://hz.chenzaomai.com/gtabnyugus.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gtwuytctgo.html

CREATE TABLE users (
来源：http://hz.vqdsnc.cn/gtfxttndrt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtfhsuucel.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tanke756.top/gtnlordctr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gotoacloud.top/gtcmmgilqw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sufxvd.cn/gtrtgriacz.html

);
来源：http://hz.jianghu66.top/gtfvtupovj.html

[Q02] 创建带外键的表
来源：http://hz.zhongyouzk.top/gtjkplcwlq.html

CREATE TABLE orders (
来源：http://hz.yueranfly.top/gtcpyfklae.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gthonmbcwk.html

user_id INT NOT NULL,
来源：http://hz.fzhhl.top/gtqczpsykb.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gtptngnyyg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gtzijfkdic.html

);
来源：http://hz.jqgfzy.top/gtgthbsnsi.html

[Q03] 增加列
来源：http://hz.xingfuxueyuan.xyz/gtpvvclasw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gtjqsrymbg.html

[Q04] 修改列类型
来源：http://hz.316326.xyz/gtyolsgmsn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.iojbl.cn/gtuztfbqki.html

[Q05] 重命名列
来源：http://hz.pycfn.com/gtqnojioxg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtsufalten.html

[Q06] 删除列
来源：http://hz.yanxiufei.cn/gtzsgzrnku.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuetiantiany.cn/gtqegiginn.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtiitsojel.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dianchejie.cn/gtrdppfiyh.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtflatmdxl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtacpryirw.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtmmxmzuda.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gttqdufmse.html

[Q10] 插入单行
来源：http://hz.daxiang520.top/gtlcnehhca.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cashguo.top/gtxdohljwm.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtzgxasekf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtovdvxuqg.html

[Q12] 插入后取自增 ID
来源：http://hz.sufxvd.cn/gtuksnbpau.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtwwjysekk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhixingplan.top/gtljswwoyg.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gttuveatyh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aizwys.cn/gtftuabjwp.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtanxsmtis.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yueranfly.top/gtmyifrvjg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gotoacloud.top/gtkeixrgjf.html

[Q15] 查询全部
来源：http://hz.shanyushiyangtech.top/gtbbehekat.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtretxxjqo.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gtlwtsmrga.html

SELECT id, name FROM users;
来源：http://hz.gotoacloud.top/gtrqqobnvs.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gtxwqygtml.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhaomingkeji.xyz/gtcbzmckej.html

[Q18] 模糊匹配
来源：http://hz.zycfv.cn/gtiyowodbp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtiajkwzxm.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gtxubbsxcc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gttlxkgjnu.html

[Q20] IN 列表
来源：http://hz.daria6918.cn/gtqjkijwsz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.feifeiyinyue.top/gtkippehqs.html

[Q21] 空值判断
来源：http://hz.andypj.xyz/gtahanbzmw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtflrelftt.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtzfiksekw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cqqwz.cn/gtubpjaysv.html

[Q23] 分页
来源：http://hz.ydzc1.top/gtgmwukmng.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtxkwmnoim.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtnsvfxhdc.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtflijjtpk.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangkeji.top/gthorvhoba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhijiandao.cn/gtllzaajho.html

[Q26] 计数
来源：http://hz.yj20258888.top/gtritpxjha.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuxming.cn/gtuhaxgass.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gtxvvsixwm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hywenlv.cn/gtzgnatvld.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtmiyohpeb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtxoqcyxat.html

[Q29] 最大最小值
来源：http://hz.jqgufenzy.top/gtrunohdau.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gtspydgwuq.html

[Q30] 分组统计
来源：http://hz.pycfn.com/gtowuoinhw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtisvglepc.html

[Q31] 分组后过滤
来源：http://hz.c1oappe.top/gttudtmcpc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtbodnngoc.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtfpxjgmrr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtmbmflcby.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.vqdsnc.cn/gtmacsdsgz.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtfkwvvatf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtccncqqxc.html

[Q34] 每组取第一条
来源：http://hz.zhongyouzk.top/gtatltzrnj.html

SELECT * FROM (
来源：http://hz.316326.xyz/gtjpkdsqqt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xziqi.cn/gtwagswyyl.html

) t WHERE rn = 1;
来源：http://hz.xingfuxueyuan.xyz/gtrxfvikwg.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gtsflvhqhw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gthcvcscnj.html

[Q36] 左连接
来源：http://hz.yonumen.top/gtaxgscphr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtbffzduid.html

[Q37] 右连接
来源：http://hz.xingfuxueyuan.xyz/gtfvmbnsfb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.vqdsnc.cn/gtvlbmxtpw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cucudq.cn/gttxeeqkqg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhoulong.xyz/gtrhtrhbtx.html

[Q39] 自连接（查上下级）
来源：http://hz.jiagoushi.top/gthzahitxf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daxiang520.top/gteczzjbyt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gtchsqiyht.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yongpay.top/gthaxgyato.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gtivpblxyw.html

[Q41] 多表连接
来源：http://hz.birdmap.top/gtxzrdpyed.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gtlfksyapb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tanke756.top/gtfulwgkdb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.c1oappe.top/gtgzseeeph.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtpaigfoqb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xylfe.cn/gtqpyqewjo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.mhx1999.top/gtkrzdewsj.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtlsacoafj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhongyouzk.top/gtjewusiga.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtwyxjdemm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhixingplan.top/gtxsjpdqog.html

[Q45] EXISTS 判断存在
来源：http://hz.ehwqpu.com/gtvfenllhp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtmvwcgskr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gtyqytzjus.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtfdzxkifx.html

[Q47] 与平均值比较
来源：http://hz.guowangkeji.top/gtmstokwmp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtsrxnuyrp.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gtspzcnmbo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtjhjjvryy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtxiqwpnwu.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtsfohlanz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.316326.xyz/gttmuygote.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtrwohvfpi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtqiixbotu.html

[Q51] 用子查询更新
来源：http://hz.jinqigfzy.top/gtpeppeviw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtpquxfkdk.html

[Q52] 删除指定行
来源：http://hz.zhaomingkeji.xyz/gtyurmfujd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gtyzhvivyo.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtcqatsqfr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gtcbwjxxrx.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gtmbxfmbnt.html

TRUNCATE TABLE logs;
来源：http://hz.redwolf501.top/gtxlxckhje.html

[Q55] 排名（并列占位）
来源：http://hz.tianlin.xyz/gtbnbfzucq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sysykeji.top/gtftmpsqqc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnxiangtu.top/gtxjlmphmx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gtuqnzhvqn.html

[Q57] 行号
来源：http://hz.havefunace.top/gtexrkkljf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258.top/gtpektvmtz.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtmxlcgddy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daria6918.cn/gtkrutuhsd.html

[Q59] 分组内累计
来源：http://hz.jyoumei.cn/gteifsxtog.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhongyouzk.top/gtlzhinxgr.html

[Q60] 取上一行 / 下一行
来源：http://hz.dianchejie.cn/gtacehjqur.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ivvv.top/gtcwvenefv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtbxatjxlm.html

[Q61] 移动平均
来源：http://hz.zdqjudy.top/gtsffhxmkx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtjpzywtai.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtkuamjghc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtajjttizo.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtsmdjeyqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cucudq.cn/gtltlknioe.html

[Q64] 提交事务
来源：http://hz.haohaochexian.top/gthjkjmljz.html

COMMIT;
来源：http://hz.yj20258888.top/gtytzshmtv.html

[Q65] 回滚事务
来源：http://hz.feifeiyinyue.top/gtzzdgghod.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtktzcjsmc.html

[Q66] 行锁查询
来源：http://hz.yvedp.cn/gtydkeumwl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guannengcc.top/gtnzyijvwr.html

[Q67] 设置隔离级别
来源：http://hz.yj202588.top/gtiqgknoeo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangkeji.top/gtuketwaif.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gtydzfsgoe.html

SAVEPOINT sp1;
来源：http://hz.jianghu66.top/gtduiuydvf.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtalvuabmz.html

[Q69] 查看执行计划
来源：http://hz.hammf.cn/gtsesgbgat.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zdqjudy.top/gtyttlymen.html

[Q70] 更新统计信息
来源：http://hz.gotoacloud.top/gtnqlbyyli.html

ANALYZE TABLE users;
来源：http://hz.tian-w.cn/gtgybcexwl.html

[Q71] 查看建表语句
来源：http://hz.xziqi.cn/gtozwyzmnl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtzmigtfpj.html

[Q72] 查看索引
来源：http://hz.pycfn.com/gtptgroupn.html

SHOW INDEX FROM users;
来源：http://hz.hnxiangtu.top/gtjvzwzdfr.html

[Q73] 查看表状态
来源：http://hz.0kj1m.cn/gthwjgxbax.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtxornmnsk.html

[Q74] 强制使用索引
来源：http://hz.chenlongwang.top/gtytelrovz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258888.top/gtobswwohj.html

[Q75] 日期格式化
来源：http://hz.snrcjt.cn/gtkiuprqpy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtriblqqir.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gtzywagdfs.html

[Q76] 按天统计
来源：http://hz.yuxming.cn/gtufutaonr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtgfhhcvsy.html

[Q77] 时间加减
来源：http://hz.chenlongwang.top/gtotdxppqu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xinyue.icu/gttvpfmqpr.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtrwlisdfs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtumycehio.html

[Q79] 字符串拼接
来源：http://hz.tanke756.top/gtksrvzisa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtznmxcugg.html

[Q80] 字符串截取
来源：http://hz.sysykeji.top/gtsqeacthf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtufmmlfnc.html

[Q81] 字符串替换
来源：http://hz.meibo888.top/gtjhsscwch.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtsgfsiihk.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gtbeughohm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nwbrower.top/gtkgtocvqn.html

[Q83] 大小写转换
来源：http://hz.zhongyouzk.top/gtukrleliz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtyehjdxqx.html

[Q84] 去除首尾空格
来源：http://hz.xylfe.cn/gtmecuumhi.html

SELECT TRIM(name) FROM users;
来源：http://hz.hammf.cn/gtptfpjxxs.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtpppxlzhd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtiinlkmri.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtixzgphzm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dashuyun.cn/gtlfymyafk.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtlpqusaqj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gzhubu.top/gtrbchjjsg.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gtsjzturzm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.52xcode.cn/gtrxyzzezy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtswovhize.html

[Q89] 判断表是否存在
来源：http://hz.jqgfzy.top/gtihcntelq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtwwwxomaz.html

[Q90] 生成序号列
来源：http://hz.ydjk.org.cn/gtfvufnnih.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtkjwkljfw.html

================================================================================
来源：http://hz.yj20258888.top/gtloyrprml.html

R. Bash 专题
来源：http://hz.jinqigfzy.top/gtmneapykt.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzcsbitod.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gtptgjuxyd.html

#!/usr/bin/env bash
来源：http://hz.jyoumei.cn/gtljnufbst.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtgbjbbduy.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gtjlmhlpef.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtfeoyplip.html

[R03] 只读变量
来源：http://hz.jinqigufen.top/gtqtrwnikf.html

readonly PI=3.14
来源：http://hz.jqgufenzy.top/gtdjzqhmwh.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtkqgzcnsw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hammf.cn/gtkbzbopth.html

[R05] 参数默认值
来源：http://hz.yanxiufei.cn/gtbqgmrknn.html

name="${1:-default}"
来源：http://hz.ehwqpu.com/gtbczjswqb.html

[R06] 判断命令是否存在
来源：http://hz.tianlin.xyz/gtbwpaebfn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.meibo888.top/gtwndhswpc.html

[R07] if 判断文件
来源：http://hz.xinyue.icu/gtmplalvla.html


<!-- 参考信息 -->