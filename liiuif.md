代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtzuhgwnbl.html

Java: UUID.randomUUID().toString()
来源：http://hz.fzhhl.top/gtotswjfhv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gtwephcuaf.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtqhremkte.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtkdrqqlpo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jianghu66.top/gtgkvomtnn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ywan-chungtsiang.top/gtcmuebiqe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gtlrdisqcx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtiicmakpv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtlywjgqrg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhaomingkeji.xyz/gtqpazwjnx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtzfrbqjro.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gteclubmhi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gthrizgqfr.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtgzqjgfgj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yueranfly.top/gtzdgijvum.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gtshsjgmck.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtvksekaut.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tian-w.cn/gtdxbhjdgn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xingfuxueyuan.xyz/gtaubggvkz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xylfe.cn/gtefroehia.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtdjuhgsye.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gaohongyu789.top/gtgcmzihke.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtrvtnewvd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ppjwa.cn/gtgzqwhxam.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtokfiehnw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtjbrrbpxz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtawlplotl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fzhhl.top/gtqolvlffr.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtnjesfymu.html

Ruby: x.length;  x.size
来源：http://hz.quarkkingdee.top/gtumxvrlxw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gthgimtbwv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtyeikmmuk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gogol.net.cn/gtftrwzjwr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtjrulnezt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.andypj.xyz/gtlfkdgsdq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gticidotoz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.andypj.xyz/gtjbyogxrt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtmcxeefyi.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gtfepndmeh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.snrcjt.cn/gtlviiqqwk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtopetitgr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.haohaochexian.top/gtoeifeako.html

PHP:  if (empty($x)) {}
来源：http://hz.fengsongda.top/gtsrknjplg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gtcthurxlr.html

TS:   if (x == null) {}
来源：http://hz.cdnleiting.top/gtsfkmizie.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtnvwarfsu.html

Go:   if x == nil {}
来源：http://hz.hnqzz.top/gtewanccyn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhijiandao.cn/gtzkesknyu.html

C#:   if (x is null) {}
来源：http://hz.bjfxy.top/gtdjsmbqxr.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gtmreulyya.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtblutlnfy.html

PHP:  // 手写时间戳比较
来源：http://hz.jianghu66.top/gtpkijyesa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gthcvxuwuj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtdzngoood.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sxryk.cn/gtncdgyapi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj202588.top/gtfescsxoh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuanzx.com/gtcwtfnusg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhengqikj.top/gttoaqpesr.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtpbxbqsfl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daxiang520.top/gtchhxxakk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.dianchejie.cn/gtmvpvxxhf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtthiwfzqa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guowangkeji.top/gtjxupbgzi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtjpbeeqym.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtuhiqfqyg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cqqwz.cn/gtixmmhgre.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinyuanbaomall.cn/gtokkktcfw.html

================================================================================
来源：http://hz.guowangkeji.top/gtptmvxwgf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.redwolf501.top/gtwabemceh.html

================================================================================
来源：http://hz.guowangkeji.top/gtljrcpddl.html

[Q01] 创建表
来源：http://hz.jinyuanbaomall.cn/gtuuoaxdgt.html

CREATE TABLE users (
来源：http://hz.xylfe.cn/gtxvmdkwym.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtuxolsgdp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daria6918.cn/gtttdkxgbf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgfzy.top/gtuqnofpvr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yongpay.top/gtagnrrhno.html

);
来源：http://hz.aibaodan.cn/gtmqdxesdy.html

[Q02] 创建带外键的表
来源：http://hz.zhoulong.xyz/gtecbfgiqr.html

CREATE TABLE orders (
来源：http://hz.zhaomingkeji.xyz/gtkkodzttl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtchwyymnq.html

user_id INT NOT NULL,
来源：http://hz.gogol.net.cn/gtnkzzggbe.html

amount DECIMAL(10, 2),
来源：http://hz.gogol.net.cn/gtctbweagl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ivvv.top/gtarifhbpv.html

);
来源：http://hz.ivvv.top/gtnrbahxed.html

[Q03] 增加列
来源：http://hz.zhixingplan.top/gturmyxver.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenjidiqi.icu/gtwprcjuoo.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtqlqldity.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gturgabnyj.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtgmgavscm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yonumen.top/gtrzijikfh.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtqiyjvskj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yanxiufei.cn/gthjaiithu.html

[Q07] 删除表
来源：http://hz.shanyushiyangtech.top/gtiljncgtx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtedshashq.html

[Q08] 创建普通索引
来源：http://hz.sysykeji.top/gtkymyszfj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtzcixtlel.html

[Q09] 创建唯一索引
来源：http://hz.andypj.xyz/gtswpxbkze.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhengqikj.top/gtylubljxf.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtlwbbqigi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtehzyfpnl.html

[Q11] 一次插入多行
来源：http://hz.quarkkingdee.top/gtapjjqxnu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shzxlz.cn/gtdikjcobg.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtidzzmhpr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtpkgsndra.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yangfankeji.com/gtatsdxfiz.html

[Q13] 忽略重复插入
来源：http://hz.cqqwz.cn/gttqmjcbvc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangshuangyany.cn/gtxdkovbcw.html

[Q14] 存在则更新（upsert）
来源：http://hz.fengsongda.top/gtbnvbziwp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhongyouzk.top/gtbjtvbhfh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.kuanghao11.cn/gtabtjbfqa.html

[Q15] 查询全部
来源：http://hz.0kj1m.cn/gtclsfxcln.html

SELECT * FROM users;
来源：http://hz.0kj1m.cn/gtucvveeeq.html

[Q16] 查询指定列
来源：http://hz.gogol.net.cn/gttkhnjtwd.html

SELECT id, name FROM users;
来源：http://hz.snrcjt.cn/gttrdyofnp.html

[Q17] 条件查询
来源：http://hz.zycfv.cn/gtbzksyehs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhengqikj.top/gthlhpanpu.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtelnejlhd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gtdhspaafr.html

[Q19] 范围查询
来源：http://hz.snrcjt.cn/gtfflgudtj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtcgbukedu.html

[Q20] IN 列表
来源：http://hz.c1oappe.top/gtqjlfetfg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gotoacloud.top/gtehedakxz.html

[Q21] 空值判断
来源：http://hz.hnqzz.top/gtkriauizr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhijiandao.cn/gtquavbnta.html

[Q22] 排序
来源：http://hz.hnqzz.top/gtztfpcgsd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydjk.org.cn/gtotnzjwrr.html

[Q23] 分页
来源：http://hz.daxiang520.top/gtrybcwivo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shzxlz.cn/gtxfjyrsoo.html

[Q24] 去重
来源：http://hz.wangdashe.top/gthwifvvwb.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydjk.org.cn/gtkpfhtcmm.html

[Q25] 只取前 N 条
来源：http://hz.sweek.top/gtngdjipnn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gtedvehpvr.html

[Q26] 计数
来源：http://hz.hnqzz.top/gtxtbmypoh.html

SELECT COUNT(*) FROM users;
来源：http://hz.quarkkingdee.top/gtvwjsxyxr.html

[Q27] 条件计数
来源：http://hz.havefunace.top/gthgnpwbch.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.52xcode.cn/gtcuimexca.html

[Q28] 求和与平均
来源：http://hz.nwbrower.top/gthhqlijuw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtsxckuypx.html

[Q29] 最大最小值
来源：http://hz.cheryme.top/gtxgroawge.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yueranfly.top/gturtakcvo.html

[Q30] 分组统计
来源：http://hz.yvedp.cn/gtqfurvxjb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtvxuegnqt.html

[Q31] 分组后过滤
来源：http://hz.ppjwa.cn/gtaoshcmpx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxuanxn.top/gtgbxnoukb.html

[Q32] 分组拼接字符串
来源：http://hz.hfpthk.cn/gtoyyvlfgc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtainxilak.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.0kj1m.cn/gtpiwlbzle.html

[Q33] 多列分组
来源：http://hz.yueranfly.top/gttjstoqxe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hfpthk.cn/gtzpjwlqpq.html

[Q34] 每组取第一条
来源：http://hz.jlsjyb.cn/gtnrrqqylr.html

SELECT * FROM (
来源：http://hz.yueranfly.top/gtyafmulsw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtjygxhqre.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtgoixggkf.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtnpumveuh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gttxwouziu.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtlbopdhre.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtywfpjxmm.html

[Q37] 右连接
来源：http://hz.shuidangran.top/gturbrqvyn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtddntfwvv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtbgnibwjy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jlsjyb.cn/gtqdleyfao.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgfzy.top/gtbdvatmaj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.52xcode.cn/gthhwxghlc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtpeueldei.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtgsqeywzk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.bjfxy.top/gtdhjewkea.html

[Q41] 多表连接
来源：http://hz.shzxlz.cn/gtrkpyvsac.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtwsorbcuk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtpcccprmt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yangfankeji.com/gtrsdbgtpw.html

[Q42] 连接条件附加过滤
来源：http://hz.gotoacloud.top/gtraasgcra.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gtjbvzqese.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtqdcvvjqg.html

[Q43] 标量子查询
来源：http://hz.yvedp.cn/gtwwojhenh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtmrfizska.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtdpccfgzn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daxiang520.top/gtzjegmvvr.html

[Q45] EXISTS 判断存在
来源：http://hz.cheryme.top/gtvurhqxry.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtsfqerzwx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.mhx1999.top/gtsytbmxrr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yueranfly.top/gtegaxjdwm.html

[Q47] 与平均值比较
来源：http://hz.ppjwa.cn/gtleynhcfu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daxiang520.top/gttxdmmlav.html

[Q48] CTE 公用表表达式
来源：http://hz.yuanzhike.top/gtewayvdla.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtggvkteri.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sysykeji.top/gthbxtqsqd.html

[Q49] 更新单行
来源：http://hz.cheryme.top/gtanpnbnvm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ppjwa.cn/gtuepifoiz.html

[Q50] 批量更新
来源：http://hz.havefunace.top/gtskzmfdjo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtsgritkxc.html

[Q51] 用子查询更新
来源：http://hz.ppjwa.cn/gtoiwhrzcq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtbaocmysi.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gtrgkgeldb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pycfn.com/gtdqnewihs.html

[Q53] 按条件删除
来源：http://hz.ehwqpu.com/gtxyaemzrw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtksismvdv.html

[Q54] 清空表
来源：http://hz.guowangkeji.top/gtbmedsjsj.html

TRUNCATE TABLE logs;
来源：http://hz.dashuyun.cn/gtrpqcwild.html

[Q55] 排名（并列占位）
来源：http://hz.mhx1999.top/gtlupreprr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgfzy.top/gtoosileyh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.quarkkingdee.top/gthrwvcdgq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhixingplan.top/gtxgsiobrg.html

[Q57] 行号
来源：http://hz.yj202588.top/gtamqukrih.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtotqnxbol.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtesdwukvo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtzcjewrha.html

[Q59] 分组内累计
来源：http://hz.xuetiantiany.cn/gtmcbsghux.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.kuanghao11.cn/gtvdyxctju.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtmsrxuofq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtyxqogdmp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtuuzwblix.html

[Q61] 移动平均
来源：http://hz.zycfv.cn/gtctiyoelh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtdsqkouod.html

[Q62] 分组占比
来源：http://hz.zhoulong.xyz/gtvukvbxhm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtmuelfscd.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtjsadqejm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuanzx.com/gtcqeoqvsb.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gtjanuyoja.html

COMMIT;
来源：http://hz.xuanzx.com/gtynwcdqzw.html

[Q65] 回滚事务
来源：http://hz.cheryme.top/gtmpmfewjz.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtmqolnynr.html

[Q66] 行锁查询
来源：http://hz.nwbrower.top/gtwvxkhyoz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtwzpmkpcs.html

[Q67] 设置隔离级别
来源：http://hz.daxiang520.top/gtfrdgaqmo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.52xcode.cn/gtexhhmjxt.html

[Q68] 保存点
来源：http://hz.shzxlz.cn/gtdiqstlxt.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtpoxlqdfw.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtdrzjnzyz.html

[Q69] 查看执行计划
来源：http://hz.daria6918.cn/gtjgvejvlb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.guowangkeji.top/gtrwoqcctq.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gtfxsbyoax.html

ANALYZE TABLE users;
来源：http://hz.havefunace.top/gtwcwqvwqt.html

[Q71] 查看建表语句
来源：http://hz.zhengqikj.top/gtwwsgodne.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtvfqilvar.html

[Q72] 查看索引
来源：http://hz.bjfxy.top/gtyeuwlqee.html

SHOW INDEX FROM users;
来源：http://hz.ydzc1.top/gtcarlngjv.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtbfisfdwl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gttdsuxtjw.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtknmzgpgr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.316326.xyz/gtgvowihgs.html

[Q75] 日期格式化
来源：http://hz.mhx1999.top/gteoqorfiz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtytciedoi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnqzz.top/gtfwsnegfc.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gtylgfvohi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtszypmybw.html

[Q77] 时间加减
来源：http://hz.gotoacloud.top/gtdcqypaux.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pycfn.com/gtgfcgttgg.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtgitbelft.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtupvsootu.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtelyrzynv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangtech.top/gtiwnjrijd.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtebsibkiy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gogol.net.cn/gtpqxnsbpw.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtlpphfobs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tianlin.xyz/gtbujcljad.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258888.top/gtycovxstr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtqkkhxtzb.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtkxwvbgfj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgfzy.top/gtzbxbxlfr.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gtcfuyjuko.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtvagbnreo.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtxgolqckt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pycfn.com/gtywpuzppa.html

[Q86] 读取 JSON 字段
来源：http://hz.yongpay.top/gtcqfnlbqs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigfzy.top/gthvrbjsvc.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtorzrmmbk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gaohongyu789.top/gtlbjqztmp.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtuyrxjxye.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgfzy.top/gtoloocqvc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtednufnld.html

[Q89] 判断表是否存在
来源：http://hz.zhongyouzk.top/gtxzdqonbx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtyagqmqyt.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gtvatdjloc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.snrcjt.cn/gtcsqjdsxe.html

================================================================================
来源：http://hz.haohaochexian.top/gtiuhwcocj.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtkagfkusb.html

================================================================================
来源：http://hz.yj20258888.top/gtjugjwohg.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtdfvpkvce.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtbvzzlqzt.html

set -euo pipefail
来源：http://hz.jianghu66.top/gtuqgzsbah.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gtyealzmwj.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtnztjzpkq.html

[R03] 只读变量
来源：http://hz.hammf.cn/gtofhgrabe.html

readonly PI=3.14
来源：http://hz.gzhubu.top/gtspiplpdq.html

[R04] 位置参数
来源：http://hz.pycfn.com/gtmnqpjbfw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtxfhnrxcc.html

[R05] 参数默认值
来源：http://hz.shanyushiyangtech.top/gtojuxtyqa.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtyxzuhxwv.html

[R06] 判断命令是否存在
来源：http://hz.ybcxt.top/gthcqtnbee.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenlongwang.top/gtavllufvf.html

[R07] if 判断文件
来源：http://hz.feifeiyinyue.top/gtnigbfkrx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtfinovuki.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtjbhoclqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gtzsrkclgg.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtgxgzphfq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigfzy.top/gtccmlhbdo.html

[R10] 正则匹配
来源：http://hz.52xcode.cn/gtyxcbjxlu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenlongwang.top/gtzlkjqlmd.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtaycjpylq.html


<!-- 参考信息 -->