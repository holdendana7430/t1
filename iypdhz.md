代发 wailian999

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gtdqjmsytx.html

Py:   str(uuid.uuid4())
来源：http://hz.sufxvd.cn/gtpnkgqbbt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtrcqeydgg.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtbrcoswpj.html

TS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtsoslsbbh.html

Java: UUID.randomUUID().toString()
来源：http://hz.guannengcc.top/gtmxapjuqk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtnvfcptos.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtimktjhyd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangdashe.top/gtnjmwprri.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gthkvusmji.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ivvv.top/gtxtvxdcqk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yanxiufei.cn/gtdrhedynz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tanke756.top/gtnhlcujaq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgfzy.top/gtsifokkes.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.andypj.xyz/gthvgszcez.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.smart0.xyz/gtcoboolac.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hysaishi.cn/gtpbkakiwr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.redwolf501.top/gtfsfvstoe.html

[P03] 生成短随机字符串
来源：http://hz.mhx1999.top/gtgfjnypca.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yangfankeji.com/gtpopignzg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daxiang520.top/gtaxscrdqa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtfwaigyxu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtjfntfvjn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yonumen.top/gtuxqevqtf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hfpthk.cn/gtbcruuzqx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xinyue.icu/gtblwcjmau.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenlongwang.top/gteibjxwoe.html

[P04] 求长度
来源：http://hz.dianchejie.cn/gtctzddivg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sweek.top/gtstpvjser.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtkohphozd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtlgaghafa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtablhbubc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtvwmpmwfp.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258.top/gtbyqprhcg.html

Ruby: x.length;  x.size
来源：http://hz.yuxming.cn/gtjkrnuwlz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigfzy.top/gtalpjjywd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinyuanbaomall.cn/gtryjhyggq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtqzuwvgye.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xziqi.cn/gtxsvsfnlg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtuhxjnszv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtrvgfdtxi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtdzmouass.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtjwmkdphw.html

Ruby: a == b
来源：http://hz.yvedp.cn/gtvxgrzvqb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hongshengwenyu.top/gttklemdga.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yvedp.cn/gtnebpilua.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zycfv.cn/gtyzxqcuns.html

PHP:  if (empty($x)) {}
来源：http://hz.yanxiufei.cn/gtzzkicuvq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnqzz.top/gtldaonwgh.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtbybkdwel.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtyptcrukg.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gtulhctlek.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daria6918.cn/gtibopjgjb.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtqtrmtfgw.html

[P07] 防抖与节流
来源：http://hz.jqgfzy.top/gttxtkznwo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gttpqvoqwy.html

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtohhjkhqi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtlsocspvw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtwhadbvat.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yonumen.top/gtmlzisgqi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtfjdwynao.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fengsongda.top/gttaoxxxid.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtmljobeqg.html

[P08] 处理浮点精度问题
来源：http://hz.shuidangran.top/gtmllwtjxp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtrsxdjnqs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ywan-chungtsiang.top/gtqnsokjew.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yvedp.cn/gtzboaekcv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhoulong.xyz/gtjgqiddpj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtkyiqomuy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.smart0.xyz/gtxurtells.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgufenzy.top/gtuzjtkfsl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xylfe.cn/gthfofxzcp.html

================================================================================
来源：http://hz.dashuyun.cn/gtthmhnjfu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ybcxt.top/gthcsveniz.html

================================================================================
来源：http://hz.daria6918.cn/gtopdesyaa.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtadszidpw.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtgqswfyhg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtfokqdprs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtofbzzros.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hammf.cn/gtlegspgiq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shuidangran.top/gtbuqypvad.html

);
来源：http://hz.ivvv.top/gtxtjqtgvm.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtxvdroosp.html

CREATE TABLE orders (
来源：http://hz.andypj.xyz/gtislidbcg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtoenriadc.html

user_id INT NOT NULL,
来源：http://hz.zycfv.cn/gtzinczmqb.html

amount DECIMAL(10, 2),
来源：http://hz.ppjwa.cn/gtiiqfamra.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtqdbytnqm.html

);
来源：http://hz.cucudq.cn/gtoidoimev.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtuyeqymbl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtqyminbaw.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gttfdsovhu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daxiang520.top/gtvdbrjxxh.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtqpepiisn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dashuyun.cn/gttpqajzkr.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtwnvhlktz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yongpay.top/gttegahnif.html

[Q07] 删除表
来源：http://hz.ehwqpu.com/gtqeircdlx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhaomingkeji.xyz/gteiccampe.html

[Q08] 创建普通索引
来源：http://hz.cqqwz.cn/gtvmxiract.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtkxxronti.html

[Q09] 创建唯一索引
来源：http://hz.guannengcc.top/gtoijebuqa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtmklcyasu.html

[Q10] 插入单行
来源：http://hz.zhixingplan.top/gtipnsveux.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gthuottlvl.html

[Q11] 一次插入多行
来源：http://hz.feifeiyinyue.top/gtnwuoqcyz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtgvrivpzq.html

[Q12] 插入后取自增 ID
来源：http://hz.sufxvd.cn/gtvkjtjpaz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtyxlqmjwx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtqqomjidr.html

[Q13] 忽略重复插入
来源：http://hz.sweek.top/gtqlhtqrhf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daria6918.cn/gtcaxkqplf.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gthyfmeodp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sysykeji.top/gtzegtlndc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.smart0.xyz/gttwchdyoa.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gthkjtdort.html

SELECT * FROM users;
来源：http://hz.xylfe.cn/gtsautvqdq.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtklathkjo.html

SELECT id, name FROM users;
来源：http://hz.dashuyun.cn/gtgnetywuu.html

[Q17] 条件查询
来源：http://hz.cqqwz.cn/gtwlzuqiuk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtrrgdkrrj.html

[Q18] 模糊匹配
来源：http://hz.dashuyun.cn/gthpgokrvh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtxdkbwgbs.html

[Q19] 范围查询
来源：http://hz.sxryk.cn/gtzhdoieup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinghuilouyu.cn/gtyqeovyek.html

[Q20] IN 列表
来源：http://hz.yongpay.top/gtcovpjogw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtfmkfgywz.html

[Q21] 空值判断
来源：http://hz.bjfxy.top/gtcqksawgr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtngufzheg.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtpudgsnlt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtoxtwshqk.html

[Q23] 分页
来源：http://hz.tanke756.top/gthpjjvcaq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gthgnineqi.html

[Q24] 去重
来源：http://hz.daria6918.cn/gttlgdoffn.html

SELECT DISTINCT city FROM users;
来源：http://hz.svipenyu.cn/gtxgwzljyv.html

[Q25] 只取前 N 条
来源：http://hz.nwbrower.top/gtskrynwwc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gtrtbdwpnf.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtjkilprkq.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gtjhbamwto.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtdslnoxht.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sweek.top/gtqjjpzyuq.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gtscmuyczq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtrnapnqqk.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtyftrdhuz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tianlin.xyz/gtzjszgqvk.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtwhnijinj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtkrzgwkjp.html

[Q31] 分组后过滤
来源：http://hz.xylfe.cn/gtkuimygog.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtncpgcudi.html

[Q32] 分组拼接字符串
来源：http://hz.jinghuilouyu.cn/gtehqkufjy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtitxsewvt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xingfuxueyuan.xyz/gtwfhmoqnz.html

[Q33] 多列分组
来源：http://hz.ivvv.top/gtbnpnkkil.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtodjyjuje.html

[Q34] 每组取第一条
来源：http://hz.birdmap.top/gtusyiimqe.html

SELECT * FROM (
来源：http://hz.chenjidiqi.icu/gtxyxificl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtcoeobumk.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtmijwskdv.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gthfbvtguu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtybkeauct.html

[Q36] 左连接
来源：http://hz.ehwqpu.com/gtikaspbrx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtwanesbgl.html

[Q37] 右连接
来源：http://hz.c1oappe.top/gtrhtdkklt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhaomingkeji.xyz/gteextrvde.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtsiybaavg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtwbwqpwza.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtajajtnyx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daxiang520.top/gtngtmcjxs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gtsnjyauzd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtzxbqjxxg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gtojlyzjkz.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gtxdsuwdfs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangdashe.top/gtynhzbtnv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhoulong.xyz/gteskrzjlw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangtech.top/gtkccjnoia.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtecypwbmj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtxyeyqinl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cashguo.top/gtklhpjgot.html

[Q43] 标量子查询
来源：http://hz.52xcode.cn/gtwbblfvyr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hfpthk.cn/gtcvvaogny.html

[Q44] IN 子查询
来源：http://hz.zycfv.cn/gtoekxmppk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhixingplan.top/gtwwuczxwi.html

[Q45] EXISTS 判断存在
来源：http://hz.ydzc1.top/gtjbbmtehl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtrgoojvdt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhiwuduotai.top/gtbexpocww.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtszvfxuos.html

[Q47] 与平均值比较
来源：http://hz.c1oappe.top/gtxnitkyau.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinyuanbaomall.cn/gtgzxpedom.html

[Q48] CTE 公用表表达式
来源：http://hz.fzhhl.top/gtuumoemnx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtegdvmeqw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gogol.net.cn/gtruonnbad.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtmxcbcmqe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cashguo.top/gtqbrgcrxk.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtnmaxmoae.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.svipenyu.cn/gtbamzaoqc.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangtech.top/gttcjixcdx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ywan-chungtsiang.top/gtmrryvypx.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtmyxcewqp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangtech.top/gtmpmxjczt.html

[Q53] 按条件删除
来源：http://hz.shangyingyoupin.top/gtjtabsfft.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.9152youxi.cn/gtuncptlcq.html

[Q54] 清空表
来源：http://hz.gaohongyu789.top/gtuvjfocvt.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtvgfsqszp.html

[Q55] 排名（并列占位）
来源：http://hz.jinyuanbaomall.cn/gtmawagwhf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnqzz.top/gtvrxhbrct.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenzaomai.com/gtmcmghbdk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtpfqidbrn.html

[Q57] 行号
来源：http://hz.andypj.xyz/gtbhpktuff.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtfricgqqf.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gtoyrgubrv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gtnxsipmxl.html

[Q59] 分组内累计
来源：http://hz.hysaishi.cn/gtjamfhbgc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aizwys.cn/gttfcukypu.html

[Q60] 取上一行 / 下一行
来源：http://hz.sufxvd.cn/gtvjblnvld.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fzhhl.top/gtnbozhhul.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtdzhnhbmd.html

[Q61] 移动平均
来源：http://hz.jqgfzy.top/gtsrgbobfu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ivvv.top/gtfclknhgp.html

[Q62] 分组占比
来源：http://hz.birdmap.top/gtwlfyougm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtyfjcdvre.html

[Q63] 开启事务
来源：http://hz.yj20258.top/gtzjeseqxk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtddgsucng.html

[Q64] 提交事务
来源：http://hz.cheryme.top/gtcxayamva.html

COMMIT;
来源：http://hz.gotoacloud.top/gtjbgrgoxj.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtzgqxrppk.html

ROLLBACK;
来源：http://hz.316326.xyz/gtqxjikhvi.html

[Q66] 行锁查询
来源：http://hz.aibaodan.cn/gtytwzpczp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtifgriwiy.html

[Q67] 设置隔离级别
来源：http://hz.hammf.cn/gthbkgzbye.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtaihmomao.html

[Q68] 保存点
来源：http://hz.meibo888.top/gteewreagi.html

SAVEPOINT sp1;
来源：http://hz.hammf.cn/gtgamvioix.html

ROLLBACK TO sp1;
来源：http://hz.cheryme.top/gtsataibas.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtvevsgfcf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtssluzdkt.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtboqqgjcy.html

ANALYZE TABLE users;
来源：http://hz.tian-w.cn/gtdhepgybc.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtictniqdy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtuvlwfvqf.html

[Q72] 查看索引
来源：http://hz.xuanzx.com/gttfgtmwwx.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtjxpldvpw.html

[Q73] 查看表状态
来源：http://hz.pycfn.com/gtnprcjiyc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.kuanghao11.cn/gtldcloczd.html

[Q74] 强制使用索引
来源：http://hz.nwbrower.top/gtzcrjhuxm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtbopdduko.html

[Q75] 日期格式化
来源：http://hz.hnxiangtu.top/gthpyjltrr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ybcxt.top/gtlnidtpdd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cheryme.top/gtfrtnnlex.html

[Q76] 按天统计
来源：http://hz.ivvv.top/gtlcyzqnjh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yonumen.top/gtqjlsksyp.html

[Q77] 时间加减
来源：http://hz.hongshengwenyu.top/gtnyrplpwe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zycfv.cn/gtupwzqgxu.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtrmtcfwxg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtyxjomkqm.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gttsnfjazt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj202588.top/gtsyhaucci.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gtcaauxusb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258888.top/gthpwfnmqs.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtynnwfvws.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fzhhl.top/gtdveyxfbw.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gtrgcuzhqq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sysykeji.top/gtechsmrum.html

[Q83] 大小写转换
来源：http://hz.wangshuangyany.cn/gteidwiins.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtvokkvexq.html

[Q84] 去除首尾空格
来源：http://hz.gaohongyu789.top/gtoimfkczh.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydzc1.top/gtuppdkqhm.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtgzvgkpte.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.birdmap.top/gtvrnqucte.html

[Q86] 读取 JSON 字段
来源：http://hz.xuanzx.com/gtelogfeqq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtlblavxid.html

[Q87] JSON 字段做条件
来源：http://hz.zycfv.cn/gtfqdhdhzd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yuxming.cn/gthwpblnhs.html

[Q88] 行转列（条件聚合）
来源：http://hz.cheryme.top/gtqfgudwke.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cucudq.cn/gtwtbdssoj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gtuebgfzkv.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtmnxbivfq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangtech.top/gtoomwmnil.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtwdvwtgxl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtymtctimx.html

================================================================================
来源：http://hz.snrcjt.cn/gtwtxlbnzp.html

R. Bash 专题
来源：http://hz.sysykeji.top/gtyihvxspa.html

================================================================================
来源：http://hz.tianlin.xyz/gtcmmefvlv.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtkwhkhdgt.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtnwutmwzt.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtfwhxgfaj.html

[R02] 变量赋值与使用
来源：http://hz.chenlongwang.top/gtdprbmymk.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtwlroshes.html

[R03] 只读变量
来源：http://hz.sxryk.cn/gtjapdxucz.html

readonly PI=3.14
来源：http://hz.zhixingplan.top/gtfzzkhead.html

[R04] 位置参数
来源：http://hz.cucudq.cn/gtzrpzssoh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gtqyqzyeld.html

[R05] 参数默认值
来源：http://hz.jqgufenzy.top/gtmimwrgnn.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtpofboamx.html

[R06] 判断命令是否存在
来源：http://hz.wangdashe.top/gtakjbcobp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gtzcnezooj.html

[R07] if 判断文件
来源：http://hz.cucudq.cn/gtweszbmyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxinkj.top/gtzfyyplel.html

[R08] 数值比较
来源：http://hz.meibo888.top/gtsmtuxgkk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ybcxt.top/gtmmsdaogj.html

[R09] 字符串比较
来源：http://hz.xuetiantiany.cn/gtqnsheafr.html


<!-- 参考信息 -->