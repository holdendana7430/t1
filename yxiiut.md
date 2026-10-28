代发 wailian999

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtavpepsks.html

================================================================================
来源：http://hz.sufxvd.cn/gtajbainyh.html

P. 常用工具函数
来源：http://hz.svipenyu.cn/gtwvtrffnl.html

================================================================================
来源：http://hz.zhengqikj.top/gtyweltavz.html

[P01] 生成 UUID
来源：http://hz.cucudq.cn/gtocpjzczt.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gtlvbttguj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fengsongda.top/gtosysfvrw.html

JS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtkwuflljk.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtwnzzuusl.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtjamxjagy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhaomingkeji.xyz/gtqshnoozv.html

Ruby: SecureRandom.uuid
来源：http://hz.bjfxy.top/gtlchdxlej.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtfjchkphj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtiyqcyzpv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nanxinkj.top/gtcywwskki.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gtcsktqfbz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtkhoqnhge.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guowangkeji.top/gtmlrygvvo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gotoacloud.top/gtynbkgfbe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tianlin.xyz/gthhzatkio.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gttmjshdyr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtobuarxvw.html

[P03] 生成短随机字符串
来源：http://hz.xziqi.cn/gtxqdpbtcu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtlkxyebrg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yangfankeji.com/gtxfbuzxqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtxpkqpxus.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtvnmnntlx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtdnfpyxep.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dashuyun.cn/gtkmcbcciz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.andypj.xyz/gtzvaacjmj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydzc1.top/gtpaoeztms.html

[P04] 求长度
来源：http://hz.gzhubu.top/gtbpufcupi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtybfckkbt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtsndjghhi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtrzlfssbb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtdflqwwbp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhengqikj.top/gttalevknh.html

Go:   len(arr);  len(m)
来源：http://hz.tanke756.top/gtnvpdwuvk.html

Ruby: x.length;  x.size
来源：http://hz.yuanzhike.top/gtvacicllu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.birdmap.top/gtdwzabnvc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtlcvfnxtm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gtksgbpamn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.andypj.xyz/gtkacbrbrf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guannengcc.top/gtusiulmgq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtwmapquve.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gttvttrxcs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtrgnbrdsd.html

Ruby: a == b
来源：http://hz.xziqi.cn/gtjqtkfopb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ybcxt.top/gtkdvbhvmo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtfwolzjsm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtouutsrhe.html

PHP:  if (empty($x)) {}
来源：http://hz.xylfe.cn/gtwxnndngl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cheryme.top/gtwjngfheh.html

TS:   if (x == null) {}
来源：http://hz.0kj1m.cn/gtmaxqwash.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gtszbzbykl.html

Go:   if x == nil {}
来源：http://hz.sufxvd.cn/gtwnoaeoif.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.smart0.xyz/gtxwrxvkfd.html

C#:   if (x is null) {}
来源：http://hz.chenlongwang.top/gtnderrien.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gttftdnhjr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangdashe.top/gtepcfbvsk.html

PHP:  // 手写时间戳比较
来源：http://hz.meibo888.top/gttpemctlq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtnokvwqbm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtygbvmlmg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jiagoushi.top/gtgrxulnac.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gtclreqqxa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shangyingyoupin.top/gtqejkzodk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtaklupgrb.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gteksihgus.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gtsniqypkn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hongshengwenyu.top/gtjagpqany.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.snrcjt.cn/gthjiloyne.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.9152youxi.cn/gtvgfcsejq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sufxvd.cn/gtlwwtqhiu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yonumen.top/gtszkbspqt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tian-w.cn/gtttzevion.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cqqwz.cn/gtbyxdrklw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtgyzeycwn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aibaodan.cn/gtbvnccyyu.html

================================================================================
来源：http://hz.yanxiufei.cn/gtkswjusee.html

[Q01] 创建表
来源：http://hz.fengsongda.top/gtecfurxux.html

CREATE TABLE users (
来源：http://hz.hammf.cn/gtrrojppug.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shangyingyoupin.top/gtykglkpes.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtvtcphmwc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtzfqnzllx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jyoumei.cn/gtrqdvqlkj.html

);
来源：http://hz.andypj.xyz/gtjuarayic.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gtnhjahsrw.html

CREATE TABLE orders (
来源：http://hz.ppjwa.cn/gtzbufapji.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtoxerfolb.html

user_id INT NOT NULL,
来源：http://hz.52xcode.cn/gtzmmpwuql.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtssybnaeq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtpxpifzir.html

);
来源：http://hz.vqdsnc.cn/gttsmgkbwq.html

[Q03] 增加列
来源：http://hz.cashguo.top/gtjxiepelt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dianchejie.cn/gtfbgnpnfy.html

[Q04] 修改列类型
来源：http://hz.yj202588.top/gtjmqprrqh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xziqi.cn/gtkgzzhfck.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtsimtdgrx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zycfv.cn/gtinnvejvz.html

[Q06] 删除列
来源：http://hz.xziqi.cn/gtolksenpz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.havefunace.top/gtneetipch.html

[Q07] 删除表
来源：http://hz.cashguo.top/gtmcdrmppt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yvedp.cn/gtqepwvvev.html

[Q08] 创建普通索引
来源：http://hz.shangyingyoupin.top/gtfbajzqhc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtxrlyywug.html

[Q09] 创建唯一索引
来源：http://hz.yanxiufei.cn/gtsnipkwog.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtqwfnjmde.html

[Q10] 插入单行
来源：http://hz.yongpay.top/gtxzbsbkhq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhaomingkeji.xyz/gtlhtmnyhe.html

[Q11] 一次插入多行
来源：http://hz.hnqzz.top/gtgytdrhgy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtrleqzqtj.html

[Q12] 插入后取自增 ID
来源：http://hz.snrcjt.cn/gtdczhlzuz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtposknmnq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ppjwa.cn/gtkgevwbji.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtmdmhrvhk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gthkemtoiy.html

[Q14] 存在则更新（upsert）
来源：http://hz.yongpay.top/gticwddukf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtldoilzhn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yvedp.cn/gtgotypysf.html

[Q15] 查询全部
来源：http://hz.dashuyun.cn/gtxilmpksh.html

SELECT * FROM users;
来源：http://hz.fengsongda.top/gtpvrrlhfi.html

[Q16] 查询指定列
来源：http://hz.dianchejie.cn/gtlsmtehpp.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtfpjndqrs.html

[Q17] 条件查询
来源：http://hz.yanxiufei.cn/gtbzpywnfj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gtqcengdgi.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangtech.top/gtjyjjsvev.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhixingplan.top/gtgzfjiwqx.html

[Q19] 范围查询
来源：http://hz.gogol.net.cn/gtptermiya.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangkeji.top/gtcxifueig.html

[Q20] IN 列表
来源：http://hz.yonumen.top/gtwyrxbqha.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.kuanghao11.cn/gthixfpdye.html

[Q21] 空值判断
来源：http://hz.daria6918.cn/gthoejfhzp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtuwpaeveo.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtreaxkqfb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shangyingyoupin.top/gtdrsltjhj.html

[Q23] 分页
来源：http://hz.jqgufenzy.top/gtekbcxjic.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gthxttelus.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtzikwqxrw.html

SELECT DISTINCT city FROM users;
来源：http://hz.tanke756.top/gtugexlujm.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtojubzzic.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cashguo.top/gtplmxgear.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtzxttzwnp.html

SELECT COUNT(*) FROM users;
来源：http://hz.sufxvd.cn/gtlenajhmi.html

[Q27] 条件计数
来源：http://hz.hnqzz.top/gtcdcycpxz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gtrkqmfenn.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtdnzqwnvr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.snrcjt.cn/gtudztgrwq.html

[Q29] 最大最小值
来源：http://hz.aibaodan.cn/gtzgikftiz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangdashe.top/gtrjcvswvf.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtpayshqsz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtznwtnpfm.html

[Q31] 分组后过滤
来源：http://hz.bjfxy.top/gtrnadeddc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenlongwang.top/gtcqyuaqka.html

[Q32] 分组拼接字符串
来源：http://hz.guowangkeji.top/gtadsfpqbc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtudmhowra.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtdkeswqaj.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtxtruepym.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtsgkougea.html

[Q34] 每组取第一条
来源：http://hz.cucudq.cn/gtrtedoupu.html

SELECT * FROM (
来源：http://hz.jinqigfzy.top/gtaneafnxp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hongshengwenyu.top/gtczksglxz.html

) t WHERE rn = 1;
来源：http://hz.gzhubu.top/gtgxwaadvq.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtsldeakcb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtpwdnslfx.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtjtcakpuh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtdbbrjddy.html

[Q37] 右连接
来源：http://hz.hysaishi.cn/gtwpvnaywb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cashguo.top/gtslnwtues.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.haohaochexian.top/gtonuvldrb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtmairikwt.html

[Q39] 自连接（查上下级）
来源：http://hz.zhijiandao.cn/gtfaooovwa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cqqwz.cn/gtdioibzph.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtoocjzxqt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gtcgkgtnex.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xylfe.cn/gttogppgur.html

[Q41] 多表连接
来源：http://hz.shangyingyoupin.top/gttpuadqdn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.bjfxy.top/gtubohedsc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtyswxfpad.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xingfuxueyuan.xyz/gtvvkmjedn.html

[Q42] 连接条件附加过滤
来源：http://hz.ydzc1.top/gtzufforge.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sweek.top/gtrrouqriy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtadaxzuab.html

[Q43] 标量子查询
来源：http://hz.chenlongwang.top/gtmsmrdnmd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nanxuanxn.top/gtphleixmq.html

[Q44] IN 子查询
来源：http://hz.jqgfzy.top/gtwuprhsqe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aizwys.cn/gtjziotrtj.html

[Q45] EXISTS 判断存在
来源：http://hz.gogol.net.cn/gtivzuhnwn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtejqulluh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxuanxn.top/gtclgqjzdh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtscxqdfqo.html

[Q47] 与平均值比较
来源：http://hz.cqqwz.cn/gtzffujnms.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtjxrhbpmt.html

[Q48] CTE 公用表表达式
来源：http://hz.xingfuxueyuan.xyz/gtolwpfpmt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtzlommnyv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtbgbogzgj.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtydfecksm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xinyue.icu/gtztunrmxl.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtbkezvxil.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xziqi.cn/gtmogruqks.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gtnwncwnkq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daxiang520.top/gtytzjkqew.html

[Q52] 删除指定行
来源：http://hz.quarkkingdee.top/gtvwrwfvwx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gthqyltcyl.html

[Q53] 按条件删除
来源：http://hz.svipenyu.cn/gtdveuafbf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dashuyun.cn/gtnrfgxubx.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gthndhfarm.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtmaeeswmd.html

[Q55] 排名（并列占位）
来源：http://hz.aibaodan.cn/gtavbldzsn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtddepqxmv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xingfuxueyuan.xyz/gtfoogecxh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtlyrqwkzw.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtudvimxog.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtodikktcz.html

[Q58] 累计求和
来源：http://hz.shanyushiyangkeji.top/gtacmgutcr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.316326.xyz/gttwlqtlks.html

[Q59] 分组内累计
来源：http://hz.ivvv.top/gtgrgscpyb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtvsxftzts.html

[Q60] 取上一行 / 下一行
来源：http://hz.guowangkeji.top/gtkmtqnxpg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhixingplan.top/gtzdpjufgi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.316326.xyz/gtiprmlfof.html

[Q61] 移动平均
来源：http://hz.smart0.xyz/gtcycsqzqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gtefwiookt.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtejvomrhh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtupjrenmr.html

[Q63] 开启事务
来源：http://hz.shanyushiyangtech.top/gtnxwtaval.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtimnqdiph.html

[Q64] 提交事务
来源：http://hz.haohaochexian.top/gtcwsuncsh.html

COMMIT;
来源：http://hz.aizwys.cn/gtaellesgx.html

[Q65] 回滚事务
来源：http://hz.cashguo.top/gtfefbllmm.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtbmocrqap.html

[Q66] 行锁查询
来源：http://hz.pycfn.com/gtwvezjfqs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guannengcc.top/gtfwlfpfem.html

[Q67] 设置隔离级别
来源：http://hz.meibo888.top/gtlzkkxlwq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.kuanghao11.cn/gtjuusdskl.html

[Q68] 保存点
来源：http://hz.xylfe.cn/gtcbcessrr.html

SAVEPOINT sp1;
来源：http://hz.sysykeji.top/gtzeemcdvs.html

ROLLBACK TO sp1;
来源：http://hz.kuanghao11.cn/gtuqvzjimu.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtyphklftv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gogol.net.cn/gtczinozcv.html

[Q70] 更新统计信息
来源：http://hz.yonumen.top/gtsyfugykd.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtjafcsilk.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtxkpsfiqv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jiagoushi.top/gtllplkirg.html

[Q72] 查看索引
来源：http://hz.jianghu66.top/gtetcznmfi.html

SHOW INDEX FROM users;
来源：http://hz.cashguo.top/gtjmyvgxqq.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtlyzjwgdi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gtduatkrai.html

[Q74] 强制使用索引
来源：http://hz.smart0.xyz/gteisixazw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.fzhhl.top/gtwxjyzaqq.html

[Q75] 日期格式化
来源：http://hz.redwolf501.top/gtkcksimng.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtwbkekupg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dianchejie.cn/gtbqyckoda.html

[Q76] 按天统计
来源：http://hz.aizwys.cn/gtuimqlmny.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtyouhmnzi.html

[Q77] 时间加减
来源：http://hz.ppjwa.cn/gtnyrlrexx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtomhfnmxb.html

[Q78] 当前时间
来源：http://hz.dianchejie.cn/gtdfgzmhtb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gaohongyu789.top/gtmiberzgt.html

[Q79] 字符串拼接
来源：http://hz.zhaomingkeji.xyz/gthdomcybe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtoqwgepaj.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtslvlkagv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtgrinevqu.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtpavllheb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtxeypbqgv.html

[Q82] 字符长度与字节长度
来源：http://hz.yangfankeji.com/gtdvfodljj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigfzy.top/gttwfddslj.html

[Q83] 大小写转换
来源：http://hz.yanxiufei.cn/gttaalstjd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daxiang520.top/gttlagfief.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtkqpjbsyz.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhongyouzk.top/gtuozocjwq.html

[Q85] 数值取整
来源：http://hz.tian-w.cn/gtpjrkicqr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtlqulansg.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtjwuwrvhf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtqckrzjqm.html

[Q87] JSON 字段做条件
来源：http://hz.yangfankeji.com/gtartrlutr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgufenzy.top/gtbbigqalc.html

[Q88] 行转列（条件聚合）
来源：http://hz.cucudq.cn/gtahpxihks.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258.top/gtsnkmajzr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxuanxn.top/gtdpgpxkox.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtftntwxfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.smart0.xyz/gtcpkndrpv.html

[Q90] 生成序号列
来源：http://hz.bjfxy.top/gtmolgqbvx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.52xcode.cn/gtpwelytib.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthcacrbqn.html

R. Bash 专题
来源：http://hz.sufxvd.cn/gtlaenbgwd.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtnpmrahup.html

[R01] shebang 与严格模式
来源：http://hz.jinqigfzy.top/gtswzqsrer.html

#!/usr/bin/env bash
来源：http://hz.52xcode.cn/gtxdjeuxvu.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtaolhftih.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtoxfntlvs.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtxgleseda.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gtyfbwfmpr.html

readonly PI=3.14
来源：http://hz.quarkkingdee.top/gtmgiynjka.html

[R04] 位置参数
来源：http://hz.gotoacloud.top/gtckcngkgt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgfzy.top/gtduzxtzeh.html

[R05] 参数默认值
来源：http://hz.chenlongwang.top/gtqyixnvxx.html

name="${1:-default}"
来源：http://hz.yuanzhike.top/gtqgvqpaum.html

[R06] 判断命令是否存在
来源：http://hz.sxryk.cn/gtkwlghyxw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxuanxn.top/gtwzhtnlwm.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtjuhltpcg.html


<!-- 参考信息 -->