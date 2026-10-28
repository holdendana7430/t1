代发 wailian999

[P01] 生成 UUID
来源：http://hz.nanxuanxn.top/gtjoyuerxt.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gteiteizqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yvedp.cn/gtezesmoin.html

JS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtbzgwufya.html

TS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtfxzzbely.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtbrzhmjos.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinyuanbaomall.cn/gtbygaqkxd.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtxcheponb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gthcwpsref.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgufenzy.top/gtwiqwuxiq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinghuilouyu.cn/gtyfsctbke.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gtupbmrtnl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuetiantiany.cn/gtebmdaivp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtkbtkhkll.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gtmkvrdhmr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.redwolf501.top/gtgqhkkfbb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yonumen.top/gtsjqhdkkx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtzvgryfcn.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtljswhrne.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtsbocaqcp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtwnhxnbvj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtvasvyrsy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtjxjklswq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shuidangran.top/gtqqxtpoja.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tanke756.top/gtouwyzalt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tianlin.xyz/gtixjnavhx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hfpthk.cn/gtxueeoyrz.html

[P04] 求长度
来源：http://hz.ywan-chungtsiang.top/gtmrhotexr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtxlbztbfh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtfhmsvfwk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.redwolf501.top/gtnlewykcl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtddhnkoeb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yonumen.top/gtenxzdoeo.html

Go:   len(arr);  len(m)
来源：http://hz.iojbl.cn/gtiaaclrna.html

Ruby: x.length;  x.size
来源：http://hz.wangshuangyany.cn/gteewhfkfh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yonumen.top/gturfswvau.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yangfankeji.com/gtzdcojuwc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gtwqdqvbuo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtxohjmpha.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtttalyrug.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtnvacdwoh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.snrcjt.cn/gtqhqzbuvt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtwrfuxbkt.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtoxctkstv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.meibo888.top/gtkybjakjw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtsspecdfx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgfzy.top/gtlxndjfmj.html

PHP:  if (empty($x)) {}
来源：http://hz.hammf.cn/gthkopstog.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aibaodan.cn/gtcfyrofew.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gthxsquzle.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtvtjvuxsc.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtdfwtbohx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj202588.top/gtbqxpurdv.html

C#:   if (x is null) {}
来源：http://hz.hnxiangtu.top/gtqaisodmi.html

[P07] 防抖与节流
来源：http://hz.gotoacloud.top/gtkrytzqgb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gtscfisqay.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigfzy.top/gtqwntjedt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtjvbdhyoh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtnahdcgws.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.vqdsnc.cn/gtjlvftiom.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj202588.top/gtfzwxzxsp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuanzx.com/gtmncofpcf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.pycfn.com/gtjfkmqklw.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gthouthbet.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtozyizrbr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tanke756.top/gtdvrullte.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gzhubu.top/gtofriqkdo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yueranfly.top/gtcikibvse.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zycfv.cn/gtbmbarort.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenlongwang.top/gtewjpukli.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cheryme.top/gtwowautyb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.svipenyu.cn/gtedyyovkz.html

================================================================================
来源：http://hz.316326.xyz/gtzxhlzjnl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pycfn.com/gtcannarbp.html

================================================================================
来源：http://hz.redwolf501.top/gtbuzgoyll.html

[Q01] 创建表
来源：http://hz.ywan-chungtsiang.top/gtjzxdahrm.html

CREATE TABLE users (
来源：http://hz.pengpengdd.cyou/gtpnxvulcx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtukesikss.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtmquzfhzq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sweek.top/gttbioewas.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hongshengwenyu.top/gtdqkvdixm.html

);
来源：http://hz.yanxiufei.cn/gtcnudufgx.html

[Q02] 创建带外键的表
来源：http://hz.cashguo.top/gtouswzhvg.html

CREATE TABLE orders (
来源：http://hz.pengpengdd.cyou/gtxxbqolmi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhongyouzk.top/gtvqqezrod.html

user_id INT NOT NULL,
来源：http://hz.cucudq.cn/gtosdgiwrj.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtepbcubud.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtdrrwdttl.html

);
来源：http://hz.hywenlv.cn/gtqdogmnxn.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtkxckhlgd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gtdyfnlczq.html

[Q04] 修改列类型
来源：http://hz.gaohongyu789.top/gtoxwfhjcb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sufxvd.cn/gtbpyibvli.html

[Q05] 重命名列
来源：http://hz.yueranfly.top/gtvfnjgjeq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gtewryfibd.html

[Q06] 删除列
来源：http://hz.hysaishi.cn/gtmbemloqc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jianghu66.top/gtcnncbget.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtaddrytlv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenlongwang.top/gtdspagkbu.html

[Q08] 创建普通索引
来源：http://hz.mhx1999.top/gtbrlulcyu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtajbfdlpk.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtajohxjfb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daxiang520.top/gtygbfodky.html

[Q10] 插入单行
来源：http://hz.shanyushiyangkeji.top/gtvotdwwei.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yangfankeji.com/gtacbuiuvu.html

[Q11] 一次插入多行
来源：http://hz.gzhubu.top/gtaoapwcca.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hywenlv.cn/gtwqwtmmim.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtvjoaghbi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xingfuxueyuan.xyz/gtykltxwsj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtdnzbzxwg.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gteugmtqhp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgfzy.top/gtpcqwkbsp.html

[Q14] 存在则更新（upsert）
来源：http://hz.hongshengwenyu.top/gtnazpwajv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtjbagpneu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuetiantiany.cn/gtqxbonvvc.html

[Q15] 查询全部
来源：http://hz.guannengcc.top/gtwmzdjtke.html

SELECT * FROM users;
来源：http://hz.ybcxt.top/gtryakncbk.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtcxtfqnvm.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtbzpjzptr.html

[Q17] 条件查询
来源：http://hz.sufxvd.cn/gtwdpnrgkb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtevusxecp.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtceldvxxl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangdashe.top/gtkyovauzj.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtljzlrfgt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yangfankeji.com/gtjbccfjuo.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtzjgzxhng.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenlongwang.top/gtlkmsnnbe.html

[Q21] 空值判断
来源：http://hz.tianlin.xyz/gtsoirhhzg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydjk.org.cn/gthdlhmhmk.html

[Q22] 排序
来源：http://hz.yj202588.top/gttbxxriey.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtbsysglno.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtbojikfii.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuetiantiany.cn/gtwudrnegw.html

[Q24] 去重
来源：http://hz.jlsjyb.cn/gtknfpctpb.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtclvxikju.html

[Q25] 只取前 N 条
来源：http://hz.fengsongda.top/gtewvvabid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.c1oappe.top/gtfwtkonxb.html

[Q26] 计数
来源：http://hz.52xcode.cn/gtbjagogky.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gtikheymzr.html

[Q27] 条件计数
来源：http://hz.cqqwz.cn/gtfqzzrtpa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hfpthk.cn/gtvvjhsdrr.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtjduvevvk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hywenlv.cn/gtgzkdpgtn.html

[Q29] 最大最小值
来源：http://hz.jlsjyb.cn/gtgqhmycne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnxiangtu.top/gtdgthytev.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gtcmvhjqgs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtsjwgwnsu.html

[Q31] 分组后过滤
来源：http://hz.daxiang520.top/gtleiuiumv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daxiang520.top/gtbmkwmadq.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtxccjvwod.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtyqyeczws.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuanzhike.top/gtqjkqpmwn.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtuncpnfdd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yongpay.top/gtejzatayo.html

[Q34] 每组取第一条
来源：http://hz.hammf.cn/gtyoolqbvx.html

SELECT * FROM (
来源：http://hz.cucudq.cn/gtjreuovab.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zdqjudy.top/gtiyvbxzqk.html

) t WHERE rn = 1;
来源：http://hz.hnqzz.top/gtvogwedwj.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtxxqofphg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtcpztosgt.html

[Q36] 左连接
来源：http://hz.shuidangran.top/gtliioikjb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtjwncjxds.html

[Q37] 右连接
来源：http://hz.sysykeji.top/gtvqlbuwrn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xziqi.cn/gthxxyhovf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gaohongyu789.top/gtafjhqsad.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtgcheswwk.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxinkj.top/gtgrjuldjf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gaohongyu789.top/gtczplcfld.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnxiangtu.top/gtazujnqsx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinyuanbaomall.cn/gtsachcoqa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnxiangtu.top/gtormlxfvw.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtwhrivhbx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtayhaswwq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gtoviswrus.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jyoumei.cn/gthslggzex.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtiivhepvz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yongpay.top/gtirhyhhro.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gttefthvyv.html

[Q43] 标量子查询
来源：http://hz.chenzaomai.com/gtpohghimg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hfpthk.cn/gtmophjlvl.html

[Q44] IN 子查询
来源：http://hz.xuetiantiany.cn/gtqedmrfgj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtwsexgkyn.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gtxkurlhop.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtigpzdwdv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gtupvsnhsa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtfrxikfuh.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtiiphprkd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dashuyun.cn/gthpopvkem.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtehjtlahm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuanzx.com/gtbwtzrquc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ywan-chungtsiang.top/gtrigpkwjq.html

[Q49] 更新单行
来源：http://hz.meibo888.top/gtdthhacmd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shuidangran.top/gtuxraflwk.html

[Q50] 批量更新
来源：http://hz.ywan-chungtsiang.top/gtnohurqln.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.snrcjt.cn/gtmnyadfoe.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtkdhfiohv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gtzetqhfkc.html

[Q52] 删除指定行
来源：http://hz.dianchejie.cn/gtxxlxenoj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtftfqsryy.html

[Q53] 按条件删除
来源：http://hz.cdnleiting.top/gtvqbacckt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtjhwipusd.html

[Q54] 清空表
来源：http://hz.hnxiangtu.top/gtgsiifjra.html

TRUNCATE TABLE logs;
来源：http://hz.tanke756.top/gthunkvzyg.html

[Q55] 排名（并列占位）
来源：http://hz.tian-w.cn/gtyjopjqxs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtzbqkvbnc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtnhhodvra.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shuidangran.top/gtekbyrpyq.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtaogwbbrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yongpay.top/gtzanrurua.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtylutzuey.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenjidiqi.icu/gtvxyyfhyv.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtfwetrrkb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shzxlz.cn/gtqudmzrdp.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenzaomai.com/gtwgmcahcc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtuunscxiu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yangfankeji.com/gtoxrpcadj.html

[Q61] 移动平均
来源：http://hz.sysykeji.top/gtjmwllejb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtrwpgaumd.html

[Q62] 分组占比
来源：http://hz.chenlongwang.top/gtbiixlytw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtesbbqqtm.html

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtklsxghcf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuetiantiany.cn/gtckbgtzus.html

[Q64] 提交事务
来源：http://hz.quarkkingdee.top/gttottgtuj.html

COMMIT;
来源：http://hz.jqgfzy.top/gtnkpwedet.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtvmcicsuu.html

ROLLBACK;
来源：http://hz.sufxvd.cn/gtocnyiaib.html

[Q66] 行锁查询
来源：http://hz.cucudq.cn/gtuektmatk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.0kj1m.cn/gtcehuxnum.html

[Q67] 设置隔离级别
来源：http://hz.xziqi.cn/gthlrrjtbq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtptjgtioy.html

[Q68] 保存点
来源：http://hz.c1oappe.top/gtktkzbhby.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtjuiimrka.html

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtrcxujgca.html

[Q69] 查看执行计划
来源：http://hz.svipenyu.cn/gtmfrjfmeb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xylfe.cn/gtvhwmyseh.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtvklvhcbb.html

ANALYZE TABLE users;
来源：http://hz.svipenyu.cn/gtdusxerqj.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtdadrhaas.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtqjyekbtk.html

[Q72] 查看索引
来源：http://hz.yuxming.cn/gtxtsrehxj.html

SHOW INDEX FROM users;
来源：http://hz.gaohongyu789.top/gtujcecevy.html

[Q73] 查看表状态
来源：http://hz.jinqigufen.top/gtqrwrjqqi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgufenzy.top/gtwwsdvphu.html

[Q74] 强制使用索引
来源：http://hz.aibaodan.cn/gtzemaejgk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xinyue.icu/gtpmxazafe.html

[Q75] 日期格式化
来源：http://hz.9152youxi.cn/gtjxhjydml.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xziqi.cn/gtughcqpqm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigfzy.top/gtozrsjjnc.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtrbcgfxca.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhongyouzk.top/gthdntlkez.html

[Q77] 时间加减
来源：http://hz.xylfe.cn/gteyssuwwq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cdnleiting.top/gtzrgogqav.html

[Q78] 当前时间
来源：http://hz.guowangkeji.top/gtjxacanau.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtkwgxvdle.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtyzijtggm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnxiangtu.top/gthogfezad.html

[Q80] 字符串截取
来源：http://hz.jyoumei.cn/gtjmwxwwlt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtkmdjowye.html

[Q81] 字符串替换
来源：http://hz.hnqzz.top/gtnbazqcck.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtldpsiaas.html

[Q82] 字符长度与字节长度
来源：http://hz.snrcjt.cn/gteyqxkljs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtduhlfbke.html

[Q83] 大小写转换
来源：http://hz.nanxinkj.top/gtvtfuyknt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtkcxrbrca.html

[Q84] 去除首尾空格
来源：http://hz.ehwqpu.com/gtecznwsvc.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnxiangtu.top/gtsihldojh.html

[Q85] 数值取整
来源：http://hz.sweek.top/gtksqendjo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yangfankeji.com/gtgoycbvff.html

[Q86] 读取 JSON 字段
来源：http://hz.chenzaomai.com/gtzwynynde.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhijiandao.cn/gtmwzovnvx.html

[Q87] JSON 字段做条件
来源：http://hz.hfpthk.cn/gthulxrzxj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gtcyxdgzpz.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinghuilouyu.cn/gtwktjybrb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gtqffpicuz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhoulong.xyz/gtuntvcyyi.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gtsfxieaqm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtrieahztn.html

[Q90] 生成序号列
来源：http://hz.nwbrower.top/gtsgwzanfj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jlsjyb.cn/gtvkknbcho.html

================================================================================
来源：http://hz.yuxming.cn/gtlcccywif.html

R. Bash 专题
来源：http://hz.ydzc1.top/gtzpdopsnw.html

================================================================================
来源：http://hz.xylfe.cn/gtxtbnvpwp.html

[R01] shebang 与严格模式
来源：http://hz.yueranfly.top/gtwqnxdwdz.html

#!/usr/bin/env bash
来源：http://hz.zhaomingkeji.xyz/gtzzhuchvg.html

set -euo pipefail
来源：http://hz.nanxuanxn.top/gtyvwuzgzd.html

[R02] 变量赋值与使用
来源：http://hz.hfpthk.cn/gtdmvysfmx.html

name="Tom"; echo "$name"
来源：http://hz.cqqwz.cn/gtjseenidt.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gtyhdrnlfp.html

readonly PI=3.14
来源：http://hz.xinyue.icu/gtfrczlhtf.html

[R04] 位置参数
来源：http://hz.yuxming.cn/gtmxynmfuq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.c1oappe.top/gtkjwsfwrb.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gtmbyyxyuz.html

name="${1:-default}"
来源：http://hz.hysaishi.cn/gtjumgrxio.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtibqazxzy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gtrkrrhzci.html

[R07] if 判断文件
来源：http://hz.jqgufenzy.top/gtainaftvx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gteimleeic.html

[R08] 数值比较
来源：http://hz.iojbl.cn/gtdkjxfuiy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtwlzxamqf.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gtpktsxzqx.html


<!-- 参考信息 -->