代发 wailian999

C#:   Parallel.For
来源：http://hz.mhx1999.top/gtezmqiclf.html

================================================================================
来源：http://hz.c1oappe.top/gtkwzhjgwf.html

P. 常用工具函数
来源：http://hz.jlsjyb.cn/gtqmlbhyqo.html

================================================================================
来源：http://hz.fengsongda.top/gtakfomtfg.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtzmrnpmqd.html

Py:   str(uuid.uuid4())
来源：http://hz.andypj.xyz/gtaocfjsjm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.wangshuangyany.cn/gtumurxsjg.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtabrysquu.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtaehouyhr.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtdbgtevjs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shuidangran.top/gtfjpmhkbz.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtbonmceea.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.meibo888.top/gtlbsfdmzu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.feifeiyinyue.top/gtfjavrrex.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtwnjgljxt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtltdytsuo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenjidiqi.icu/gtvmpociah.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangkeji.top/gtkydefbhg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtthuwfwcl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.feifeiyinyue.top/gtsptrugdf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hfpthk.cn/gtstjvqpok.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shuidangran.top/gtfiycdsit.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtintdtgeg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuanzhike.top/gttuinzkmx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xinyue.icu/gtipwhyqdj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtscvgjfzn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtfkdjzpya.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gttnbymtzp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gtvttjhush.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtrbgpgsnv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sufxvd.cn/gtbuzzmsbb.html

[P04] 求长度
来源：http://hz.ppjwa.cn/gtejvhatjy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sufxvd.cn/gtjqpntqbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtigleahlz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtjhlaukkc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gthecfbzxb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtxmozctfu.html

Go:   len(arr);  len(m)
来源：http://hz.xingfuxueyuan.xyz/gtdsrfukjm.html

Ruby: x.length;  x.size
来源：http://hz.xingfuxueyuan.xyz/gtsoxbyqnx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hywenlv.cn/gtkyfxpamn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.svipenyu.cn/gtuonkqvoi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gtakeheffr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yongpay.top/gtpgrnfgbe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtxacysjuy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtomreqsyk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtjpqgokkr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ehwqpu.com/gthlkkcmjc.html

Ruby: a == b
来源：http://hz.fengsongda.top/gticomgxkd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.smart0.xyz/gtekuqxtbi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ywan-chungtsiang.top/gtnnrrhsxt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gotoacloud.top/gtzbpsuezj.html

PHP:  if (empty($x)) {}
来源：http://hz.cashguo.top/gtymuekfdq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258.top/gtjesmgjdj.html

TS:   if (x == null) {}
来源：http://hz.cheryme.top/gtafqztzec.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxinkj.top/gteerfswop.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtlykehtxw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtllflercq.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtdacumwab.html

[P07] 防抖与节流
来源：http://hz.xziqi.cn/gteoghdbof.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtwrcijanh.html

PHP:  // 手写时间戳比较
来源：http://hz.c1oappe.top/gtyubjswil.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtihrehtpg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtmzsbqpgz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yonumen.top/gtuwcoqlbp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtlefzrqsh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydzc1.top/gtjzgyqqms.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.redwolf501.top/gtqmlanrmt.html

[P08] 处理浮点精度问题
来源：http://hz.0kj1m.cn/gtigvmfyvk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yonumen.top/gtrosxqpjp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtyrufubwe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.9152youxi.cn/gtmibgwkya.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daria6918.cn/gtibteqqky.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydjk.org.cn/gtlbcsddnj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jyoumei.cn/gtqsuzebje.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtfpqvkkqt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.fzhhl.top/gteutiilsg.html

================================================================================
来源：http://hz.xylfe.cn/gtfotowqji.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zdqjudy.top/gtpcnjhahw.html

================================================================================
来源：http://hz.ivvv.top/gtbybwixfq.html

[Q01] 创建表
来源：http://hz.pycfn.com/gtnnyldnyn.html

CREATE TABLE users (
来源：http://hz.zdqjudy.top/gtkjzhducn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtgjjssvwc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtioznmsdr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yanxiufei.cn/gttujzonpd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangkeji.top/gtlzwcifaa.html

);
来源：http://hz.nanxinkj.top/gtiwyrrlkf.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtawlzynfk.html

CREATE TABLE orders (
来源：http://hz.gotoacloud.top/gtistcluru.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gttsnwmymt.html

user_id INT NOT NULL,
来源：http://hz.hnqzz.top/gtsjcienqj.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtfktxcgrd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtdvgalaey.html

);
来源：http://hz.316326.xyz/gtftxowbeg.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtpzouczvu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj202588.top/gtycbfryad.html

[Q04] 修改列类型
来源：http://hz.xinyue.icu/gtclhxlwam.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtitpdyjcv.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtlmtgjtts.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.svipenyu.cn/gtjithplmh.html

[Q06] 删除列
来源：http://hz.smart0.xyz/gtcsyufbno.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gtiwzheium.html

[Q07] 删除表
来源：http://hz.hongshengwenyu.top/gtltfjtaxu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhaomingkeji.xyz/gtexxwmvtt.html

[Q08] 创建普通索引
来源：http://hz.ehwqpu.com/gtfpokvjxm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtarlsqijo.html

[Q09] 创建唯一索引
来源：http://hz.guowangkeji.top/gtrvojkpaf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daria6918.cn/gtlhjvvlwm.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gtsjzbuvco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ehwqpu.com/gtxbqgclzd.html

[Q11] 一次插入多行
来源：http://hz.ybcxt.top/gtdrzwazev.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtyasbioqm.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangtech.top/gtvkmilybr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ywan-chungtsiang.top/gtnlxaxlui.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gtavgjldot.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtroyoeeis.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuxming.cn/gtjsifsmom.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtxubokhhn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tianlin.xyz/gtxhulakvt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cucudq.cn/gtiteuqgiq.html

[Q15] 查询全部
来源：http://hz.52xcode.cn/gtsrehvtdq.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtnjavbsft.html

[Q16] 查询指定列
来源：http://hz.hnxiangtu.top/gtaunuhmyr.html

SELECT id, name FROM users;
来源：http://hz.cucudq.cn/gtgkbkyydr.html

[Q17] 条件查询
来源：http://hz.aizwys.cn/gtybsratyi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ivvv.top/gtsdodyclp.html

[Q18] 模糊匹配
来源：http://hz.xinyue.icu/gtoxyyxmva.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hammf.cn/gtatbqujcq.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtiqtaojmo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtjjvcdjne.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gttbgtrafm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtekjurutq.html

[Q21] 空值判断
来源：http://hz.redwolf501.top/gtdnuotoar.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yonumen.top/gtiqbkvgos.html

[Q22] 排序
来源：http://hz.aibaodan.cn/gtposgpjxi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sxryk.cn/gtittcfyjw.html

[Q23] 分页
来源：http://hz.redwolf501.top/gtfetgldal.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtqwxyjvyb.html

[Q24] 去重
来源：http://hz.yj202588.top/gttnrvlcif.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtdlsrhzhs.html

[Q25] 只取前 N 条
来源：http://hz.xinyue.icu/gtafjeprhb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuanzx.com/gtryervgiy.html

[Q26] 计数
来源：http://hz.hywenlv.cn/gtpkovhwin.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtpdeuquzn.html

[Q27] 条件计数
来源：http://hz.sweek.top/gtvgwdsnkj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhoulong.xyz/gtifctjwpr.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtvhtcsimc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gtgwcacvig.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gtlutbjrnw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtzzimrgva.html

[Q30] 分组统计
来源：http://hz.snrcjt.cn/gtnqhcodmn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtdgierkkj.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtyfwbxcnf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtqpyhdwbj.html

[Q32] 分组拼接字符串
来源：http://hz.zdqjudy.top/gtohfqfotv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtzocmceex.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daria6918.cn/gtrqaihbjc.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtufjfthtv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangshuangyany.cn/gtepqilqxo.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtnhmxmxky.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gttbprhczh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cdnleiting.top/gtzcqucsga.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gtyacddmrf.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gtkbbkfjhp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtwlplifgj.html

[Q36] 左连接
来源：http://hz.havefunace.top/gtcpuofsis.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtwcbaoxzr.html

[Q37] 右连接
来源：http://hz.jinqigfzy.top/gtfexpvcud.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtirpxdcbj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nwbrower.top/gtqnkmwppx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtmdceftyc.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gtertchthj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.9152youxi.cn/gtaclrceac.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtyjyjakof.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtwwhofrmo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenlongwang.top/gtutfesgtv.html

[Q41] 多表连接
来源：http://hz.sufxvd.cn/gttzycyckn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtmsknmqke.html

JOIN users u ON u.id = o.user_id
来源：http://hz.iojbl.cn/gtzmehotyl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.bjfxy.top/gtaozieevc.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gtcbmvdwva.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yonumen.top/gtftqqbbes.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtqrzqxllj.html

[Q43] 标量子查询
来源：http://hz.quarkkingdee.top/gtwqxkxaoi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.52xcode.cn/gtehmpziwt.html

[Q44] IN 子查询
来源：http://hz.pengpengdd.cyou/gtytmmrkzn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ehwqpu.com/gtvrbwpvaw.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtfrpdnyqa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gthsrmyjya.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cucudq.cn/gtwocwdrtv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtkfxfrzsm.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gtgtbzszzy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hongshengwenyu.top/gtghpinagy.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gtfqvilxwr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gterhbrxlo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydjk.org.cn/gtmiucktvr.html

[Q49] 更新单行
来源：http://hz.snrcjt.cn/gtpqyjazxp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zycfv.cn/gtkaqzvfsd.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtclmkgzfe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.iojbl.cn/gtugrwroyw.html

[Q51] 用子查询更新
来源：http://hz.yj20258.top/gtcbdkjjuv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daria6918.cn/gtfemsrozj.html

[Q52] 删除指定行
来源：http://hz.zhoulong.xyz/gtfqhvquki.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxinkj.top/gtoxxjjyqf.html

[Q53] 按条件删除
来源：http://hz.shangyingyoupin.top/gtyvbocjpp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinghuilouyu.cn/gteezrahdt.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gttyvyulof.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtreknrajt.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtoieglnhw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gtrxptjydo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yueranfly.top/gtzpuimuxs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtcqocagqj.html

[Q57] 行号
来源：http://hz.birdmap.top/gtlbzmloow.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.redwolf501.top/gtlddjanfi.html

[Q58] 累计求和
来源：http://hz.jiagoushi.top/gtcyknhigp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtwvedfojc.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtpzknlqhq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gtuumeerxj.html

[Q60] 取上一行 / 下一行
来源：http://hz.yvedp.cn/gtipryzwfb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtdpnwtbnu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuetiantiany.cn/gthkoxuqeh.html

[Q61] 移动平均
来源：http://hz.gzhubu.top/gtrtjkjrmz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guannengcc.top/gtlpzshzwc.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtwusuodkz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtkixlcfsp.html

[Q63] 开启事务
来源：http://hz.ydzc1.top/gtxeirwshb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtywlvyqxs.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gtzlpcqjpd.html

COMMIT;
来源：http://hz.yanxiufei.cn/gttepvmfqb.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtmryhazxk.html

ROLLBACK;
来源：http://hz.jqgufenzy.top/gtsgzcvfno.html

[Q66] 行锁查询
来源：http://hz.havefunace.top/gtbompuwdy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gtglfklyfd.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gteyoxxmpf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtxcvulfvc.html

[Q68] 保存点
来源：http://hz.cqqwz.cn/gtgvdttfjh.html

SAVEPOINT sp1;
来源：http://hz.gaohongyu789.top/gtrrqvfzef.html

ROLLBACK TO sp1;
来源：http://hz.jinghuilouyu.cn/gtkidmsplu.html

[Q69] 查看执行计划
来源：http://hz.ehwqpu.com/gtecyfonco.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtluumewbf.html

[Q70] 更新统计信息
来源：http://hz.aizwys.cn/gtmzgxdrpc.html

ANALYZE TABLE users;
来源：http://hz.wangdashe.top/gtyhounotu.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gtoyipqzyf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xylfe.cn/gtgsjvccrs.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtkxdymtkm.html

SHOW INDEX FROM users;
来源：http://hz.yangfankeji.com/gtvqqymejx.html

[Q73] 查看表状态
来源：http://hz.0kj1m.cn/gtxuskwhvs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fengsongda.top/gtarixxpxy.html

[Q74] 强制使用索引
来源：http://hz.zhongyouzk.top/gtivkcpmwl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj202588.top/gtfqynynml.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtbzogyyvs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sweek.top/gtdbkzcuyc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hywenlv.cn/gtqioywqkm.html

[Q76] 按天统计
来源：http://hz.kuanghao11.cn/gttftbqyah.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuanzhike.top/gtrgqymsux.html

[Q77] 时间加减
来源：http://hz.jinqigufen.top/gtvnoguygo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtryzalcsp.html

[Q78] 当前时间
来源：http://hz.zhengqikj.top/gtfqegaune.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.feifeiyinyue.top/gtjcuzsnke.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtikbkjtmx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtsobmskgy.html

[Q80] 字符串截取
来源：http://hz.ywan-chungtsiang.top/gtpokziarm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jiagoushi.top/gtdrbxxbmc.html

[Q81] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gthdmautfh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gterfowpoe.html

[Q82] 字符长度与字节长度
来源：http://hz.shangyingyoupin.top/gtivsgyhjr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuxming.cn/gtepmamuaj.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtfcfatuvt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtvzvjmkjf.html

[Q84] 去除首尾空格
来源：http://hz.sufxvd.cn/gtlkrzqexz.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtdshhlyql.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtsxkxxxuq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtymvdibjv.html

[Q86] 读取 JSON 字段
来源：http://hz.redwolf501.top/gtazpfqqlf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtjwugqgbh.html

[Q87] JSON 字段做条件
来源：http://hz.tian-w.cn/gtgqmmqyzz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.havefunace.top/gtazvtcnos.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtblgqrmkn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.kuanghao11.cn/gtopokvtqk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnqzz.top/gtyurjgvmk.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtamofqaso.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xylfe.cn/gtsfxchnch.html

[Q90] 生成序号列
来源：http://hz.sweek.top/gtoubyepzb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj202588.top/gtmsxvuhxd.html

================================================================================
来源：http://hz.redwolf501.top/gtrujdvxur.html

R. Bash 专题
来源：http://hz.gotoacloud.top/gtvhekpjkg.html

================================================================================
来源：http://hz.cqqwz.cn/gtohyyynkd.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtztqvvptt.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtwecwqkis.html

set -euo pipefail
来源：http://hz.shanyushiyangkeji.top/gthytcpcxo.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtwcvupfkh.html

name="Tom"; echo "$name"
来源：http://hz.vqdsnc.cn/gtiflslegr.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gtuxreikgr.html

readonly PI=3.14
来源：http://hz.nanxinkj.top/gtveyowlrp.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gteqqwqvxm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sweek.top/gtnrfguicz.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtfxsixpkp.html

name="${1:-default}"
来源：http://hz.zhiwuduotai.top/gtholufktj.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtqipndwnn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aizwys.cn/gtfgoopldx.html

[R07] if 判断文件
来源：http://hz.yj20258888.top/gtvsgwnwka.html


<!-- 参考信息 -->