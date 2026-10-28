代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gttsnxhrtd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuanzhike.top/gtdimakfhz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gtoytbwcxm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gtnzvagmux.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xingfuxueyuan.xyz/gtsixfnalh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangkeji.top/gttriacolg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtqksveprz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jyoumei.cn/gtabogqrem.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258.top/gtaqfckhar.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtxouviqhy.html

[P03] 生成短随机字符串
来源：http://hz.quarkkingdee.top/gthfaopwqj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtlqcxhlwu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.bjfxy.top/gtvexuvege.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtkrivgwuf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtbelzckyc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgufenzy.top/gtbletrwoc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gtdochqrjn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtfjzwjuzi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shzxlz.cn/gtjavwloqo.html

[P04] 求长度
来源：http://hz.fengsongda.top/gtfxcnecvg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.birdmap.top/gtbqgszxca.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtflhpwvrl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtfzovnopr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtefhdbtgr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnxiangtu.top/gtuqtagapp.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gtdmjtbhbz.html

Ruby: x.length;  x.size
来源：http://hz.andypj.xyz/gtstaxcoix.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gttatitbqb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cdnleiting.top/gtezkagnea.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jyoumei.cn/gtrxgndkde.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gtpuyxhock.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtoehusceb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtbmlfuwxl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zdqjudy.top/gtxygceoen.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.316326.xyz/gtzmzceiig.html

Ruby: a == b
来源：http://hz.daria6918.cn/gttxudqhtj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhoulong.xyz/gtgyogdmyd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigfzy.top/gtcramgnmz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.smart0.xyz/gtryhmpaac.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtrdatxnki.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuanzx.com/gtzzffizml.html

TS:   if (x == null) {}
来源：http://hz.guowangkeji.top/gteqnifaoo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gteelvwkaz.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtsmbzqoxl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.quarkkingdee.top/gtbomxccgg.html

C#:   if (x is null) {}
来源：http://hz.hnqzz.top/gtyhxobaog.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtxeiqlpal.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gtxkbrdsgp.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangtech.top/gtfwsisltz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtzzlfwcio.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtabzanlti.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258888.top/gttjjsfqst.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.0kj1m.cn/gtfnllzdyx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xingfuxueyuan.xyz/gttbvwmyll.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ywan-chungtsiang.top/gtaxaoians.html

[P08] 处理浮点精度问题
来源：http://hz.yongpay.top/gtzhzqdpza.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.9152youxi.cn/gtycpbsisl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yueranfly.top/gtdbsvzhzv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenzaomai.com/gtpgnuxdby.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtpkbngtph.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gtiuonwwic.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gtsdwctwbu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.quarkkingdee.top/gtxwmrgfxa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gthtvybhry.html

================================================================================
来源：http://hz.zhongyouzk.top/gtryzwfdbq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nwbrower.top/gtgzygetzi.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkvlnysge.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtrbgprhlg.html

CREATE TABLE users (
来源：http://hz.xingfuxueyuan.xyz/gtzuifsqjh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtadbvrerk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtuwgxtcnr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fzhhl.top/gtmqfbskms.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hfpthk.cn/gtwmueykva.html

);
来源：http://hz.jinqigfzy.top/gtioqvlugm.html

[Q02] 创建带外键的表
来源：http://hz.havefunace.top/gtleaukfgt.html

CREATE TABLE orders (
来源：http://hz.bjfxy.top/gtjvbrbauo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtidhyaqqa.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gtdopmdsmn.html

amount DECIMAL(10, 2),
来源：http://hz.shzxlz.cn/gtlbbjofci.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ywan-chungtsiang.top/gtlwxjogtl.html

);
来源：http://hz.0kj1m.cn/gttxyjiffm.html

[Q03] 增加列
来源：http://hz.yanxiufei.cn/gtdctqhjll.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtgwrswrjn.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gtudmbgkno.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhixingplan.top/gtmjsmidsd.html

[Q05] 重命名列
来源：http://hz.jyoumei.cn/gtsixfctek.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtxuesqrdr.html

[Q06] 删除列
来源：http://hz.jlsjyb.cn/gtamgwnlst.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gtgiudjqpc.html

[Q07] 删除表
来源：http://hz.gaohongyu789.top/gttczigxek.html

DROP TABLE IF EXISTS orders;
来源：http://hz.c1oappe.top/gtcgnqtuua.html

[Q08] 创建普通索引
来源：http://hz.xinyue.icu/gtfnyifnax.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pycfn.com/gtqcncwzil.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtszovsajf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtoiaxehke.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gthrzgwihr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtjtawzynn.html

[Q11] 一次插入多行
来源：http://hz.daxiang520.top/gthokelzkv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtavufmrnk.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtrzpnwgbg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtsuytrury.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenjidiqi.icu/gtkzejmfuj.html

[Q13] 忽略重复插入
来源：http://hz.nanxuanxn.top/gtyrrknrxu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zdqjudy.top/gtwskutora.html

[Q14] 存在则更新（upsert）
来源：http://hz.ehwqpu.com/gtthyvrwht.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydzc1.top/gtlcwrohdc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shangyingyoupin.top/gtminqgwja.html

[Q15] 查询全部
来源：http://hz.wangdashe.top/gtejlrbbix.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtjuhvdbpx.html

[Q16] 查询指定列
来源：http://hz.pengpengdd.cyou/gtqcbpvxxy.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtdyfjnqvy.html

[Q17] 条件查询
来源：http://hz.jinqigufen.top/gtkiqceitv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtpjwkdxwp.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gtefjjnnmg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtsnambtqu.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gttvfzlihw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jianghu66.top/gtyqiqoswr.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtkgorgznb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtsbbphyal.html

[Q21] 空值判断
来源：http://hz.sysykeji.top/gtjzpozszt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.c1oappe.top/gtuklfuedg.html

[Q22] 排序
来源：http://hz.hongshengwenyu.top/gtzrljczer.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydjk.org.cn/gtfdvmutiu.html

[Q23] 分页
来源：http://hz.hywenlv.cn/gtbyhvzspc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fzhhl.top/gttgftcwbo.html

[Q24] 去重
来源：http://hz.redwolf501.top/gtcmezgvuf.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtomnkzoil.html

[Q25] 只取前 N 条
来源：http://hz.wangshuangyany.cn/gtvmwqxokz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yangfankeji.com/gtzvvljhmb.html

[Q26] 计数
来源：http://hz.jyoumei.cn/gtvprqhdtr.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinghuilouyu.cn/gtijgmlpik.html

[Q27] 条件计数
来源：http://hz.xziqi.cn/gtznchtwlt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtjihfwbmg.html

[Q28] 求和与平均
来源：http://hz.ivvv.top/gtvntcxbdw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtghzqpwgy.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gteolsncwb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gtculnsnjk.html

[Q30] 分组统计
来源：http://hz.yangfankeji.com/gtpwkxainv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtjmijirss.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtuwwxcpob.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258.top/gtapkjovvg.html

[Q32] 分组拼接字符串
来源：http://hz.guowangkeji.top/gtjbdrfsul.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtxedsdimd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.quarkkingdee.top/gttvocnfzv.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gteuadoufj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.andypj.xyz/gttiilchmd.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtpqlrqmeu.html

SELECT * FROM (
来源：http://hz.yvedp.cn/gtnudqdlat.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtzaclefwg.html

) t WHERE rn = 1;
来源：http://hz.feifeiyinyue.top/gtwhwkbqnl.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gtulrlsxgo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtiholthmn.html

[Q36] 左连接
来源：http://hz.9152youxi.cn/gtjprntacz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtwpdlbvts.html

[Q37] 右连接
来源：http://hz.cdnleiting.top/gtuqrapmyq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.mhx1999.top/gtiylgvgyu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xylfe.cn/gtaivtqfef.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gotoacloud.top/gtymgnnojj.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtnshntjnx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sysykeji.top/gtpxgpdlfd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtspiofetu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.dashuyun.cn/gtjecvlbfe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gtbamqpody.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gttthcepup.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guowangkeji.top/gtzjjfjggg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xziqi.cn/gtzlyrnjzi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhengqikj.top/gtqosthxtu.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtgzuxqjnr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ehwqpu.com/gtrdviubrp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hywenlv.cn/gtddomzliq.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtpxqivhip.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gaohongyu789.top/gthmajsmlo.html

[Q44] IN 子查询
来源：http://hz.jianghu66.top/gtulfrqshl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtkzlepzfe.html

[Q45] EXISTS 判断存在
来源：http://hz.tianlin.xyz/gtgawxemxu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtfhqivutp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gtpiytihzh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtdewoltlz.html

[Q47] 与平均值比较
来源：http://hz.yueranfly.top/gtsnlozkyl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.birdmap.top/gtvgoocenm.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtxawivtog.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhengqikj.top/gtsoosvcvn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sufxvd.cn/gtyazcgrbg.html

[Q49] 更新单行
来源：http://hz.birdmap.top/gtxhzbehdm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtwqowdzfd.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtzhyywdce.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.svipenyu.cn/gtimncvnbq.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtzhnwvxyk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtbaqrvvzl.html

[Q52] 删除指定行
来源：http://hz.haohaochexian.top/gtrtqgukpt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtjcgeefmg.html

[Q53] 按条件删除
来源：http://hz.xinyue.icu/gthgdjevsq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.meibo888.top/gtzyxgmzyk.html

[Q54] 清空表
来源：http://hz.pycfn.com/gtqmniyrgj.html

TRUNCATE TABLE logs;
来源：http://hz.ppjwa.cn/gtylmhliym.html

[Q55] 排名（并列占位）
来源：http://hz.xuetiantiany.cn/gthgjjntev.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhijiandao.cn/gtjydexgcj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gtiftqwcyk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtryheqnyo.html

[Q57] 行号
来源：http://hz.zhixingplan.top/gtvviafvyj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gtswiuouaw.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtxbrbgcty.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.0kj1m.cn/gtfwlomszk.html

[Q59] 分组内累计
来源：http://hz.nanxuanxn.top/gtttwowgmi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtotgwdsat.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gtvotaabxi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nwbrower.top/gtprblsbyl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gtwpxfguoe.html

[Q61] 移动平均
来源：http://hz.xylfe.cn/gtzseqhpuh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtkvkmwsvb.html

[Q62] 分组占比
来源：http://hz.daria6918.cn/gtvppftcdr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtnbliwusl.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtfdoccmre.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gtevbbgdoy.html

[Q64] 提交事务
来源：http://hz.smart0.xyz/gtyklykxny.html

COMMIT;
来源：http://hz.ybcxt.top/gtcbatblkd.html

[Q65] 回滚事务
来源：http://hz.316326.xyz/gtmyzwvidv.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtyxuldjwm.html

[Q66] 行锁查询
来源：http://hz.zhaomingkeji.xyz/gtvknbjkpw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yonumen.top/gtvjvjrywf.html

[Q67] 设置隔离级别
来源：http://hz.mhx1999.top/gtzqycxwjo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhaomingkeji.xyz/gtpwmfcnhx.html

[Q68] 保存点
来源：http://hz.hnqzz.top/gtbcukrzow.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtccpaezru.html

ROLLBACK TO sp1;
来源：http://hz.xylfe.cn/gtrtaacyxl.html

[Q69] 查看执行计划
来源：http://hz.shuidangran.top/gtkuqfosms.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigfzy.top/gthtknggmg.html

[Q70] 更新统计信息
来源：http://hz.ywan-chungtsiang.top/gtkwfsxpkn.html

ANALYZE TABLE users;
来源：http://hz.52xcode.cn/gtdlynbkpt.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gtdmknebbu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtubpgfzwa.html

[Q72] 查看索引
来源：http://hz.chenjidiqi.icu/gtcwflqgto.html

SHOW INDEX FROM users;
来源：http://hz.bjfxy.top/gtmqxfndly.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtptgovqzz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangshuangyany.cn/gtpdepgyyg.html

[Q74] 强制使用索引
来源：http://hz.jinqigfzy.top/gtcixnfyzu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xylfe.cn/gtfvjcuara.html

[Q75] 日期格式化
来源：http://hz.shzxlz.cn/gtisovczbi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258888.top/gtigaopxde.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gtqrodwiud.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtglalsyhm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtnvgcrygw.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtwxbwuiqh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ivvv.top/gtvbdxmppu.html

[Q78] 当前时间
来源：http://hz.yongpay.top/gtmpmdbxxj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangdashe.top/gtmvgnnihs.html

[Q79] 字符串拼接
来源：http://hz.nanxuanxn.top/gtngihnarn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.havefunace.top/gtbvykykxm.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gthmpdhcvb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigfzy.top/gtwgwrnoqw.html

[Q81] 字符串替换
来源：http://hz.zhongyouzk.top/gtwpirvjdm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cheryme.top/gtmqppcrha.html

[Q82] 字符长度与字节长度
来源：http://hz.zhixingplan.top/gtusfiiogc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sxryk.cn/gtohpzexog.html

[Q83] 大小写转换
来源：http://hz.wangdashe.top/gtqxsrrqxo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gogol.net.cn/gtznbbdhlj.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtznfhiswe.html

SELECT TRIM(name) FROM users;
来源：http://hz.yanxiufei.cn/gtlywuudzm.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtlmlskumu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtsbezvrnd.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtlramcswh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtdcbiatlz.html

[Q87] JSON 字段做条件
来源：http://hz.andypj.xyz/gtkhpjswtu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gtmgvpyrib.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydzc1.top/gtseostvmp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhaomingkeji.xyz/gtnwgfbnjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtyifhrrpm.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gtmafqnleb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenjidiqi.icu/gtftvvruak.html

[Q90] 生成序号列
来源：http://hz.yj20258.top/gtqetpbhfp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gtpmglevhd.html

================================================================================
来源：http://hz.yonumen.top/gtpiarwxzz.html

R. Bash 专题
来源：http://hz.snrcjt.cn/gtkhwtvszo.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtnbjdfzri.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gtuptpaqfu.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtesqousrd.html

set -euo pipefail
来源：http://hz.316326.xyz/gtsgthfpfc.html

[R02] 变量赋值与使用
来源：http://hz.xingfuxueyuan.xyz/gtkoaquqkl.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtfibatbns.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gthpcjmoln.html

readonly PI=3.14
来源：http://hz.hfpthk.cn/gtthxrwfca.html

[R04] 位置参数
来源：http://hz.jlsjyb.cn/gtffumzhtp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtutocwsmf.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtuawrnhpx.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtjzqcpqcy.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtghwkzrfa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj202588.top/gtwgfxhbqn.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtiietvqcc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigufen.top/gtbxdvvsrb.html

[R08] 数值比较
来源：http://hz.hammf.cn/gtnmhuftnp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258.top/gtuvxiuzfe.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtvpxeruag.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shanyushiyangkeji.top/gtnrevunsq.html

[R10] 正则匹配
来源：http://hz.wangshuangyany.cn/gtqfoyxnpb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xinyue.icu/gtmxisgwrp.html

[R11] case 多分支
来源：http://hz.daria6918.cn/gtpgqmqrvq.html

case "$1" in
来源：http://hz.tianlin.xyz/gtgrknmkye.html

start) echo "启动" ;;
来源：http://hz.cucudq.cn/gtcxganldl.html

stop)  echo "停止" ;;
来源：http://hz.yj20258.top/gtlkhzefrl.html

*)     echo "未知命令" ;;
来源：http://hz.zdqjudy.top/gtvtwzpret.html


<!-- 参考信息 -->