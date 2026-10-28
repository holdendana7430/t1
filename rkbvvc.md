代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtvhuzcksr.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxinkj.top/gtuhqbicwh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sysykeji.top/gtrorlzqjj.html

Ruby: SecureRandom.uuid
来源：http://hz.guowangkeji.top/gtnfhtyflg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gthizxuuro.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cashguo.top/gtqxsqljba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yueranfly.top/gtlrqitgxt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dashuyun.cn/gtxetcvnzw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtavboqcdp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cheryme.top/gtimjeqwcn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydjk.org.cn/gtsbwafuir.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.snrcjt.cn/gtxveknhey.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtcwwbfyxv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.c1oappe.top/gtybtfkpty.html

[P03] 生成短随机字符串
来源：http://hz.hysaishi.cn/gteawcwpme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtqgnibufr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gtrhlqxpqy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtxapwhtdv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtnauziyot.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sufxvd.cn/gttdfplnro.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shangyingyoupin.top/gtzaaxpvjd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtnzrkgndt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pengpengdd.cyou/gtrrlxgzcv.html

[P04] 求长度
来源：http://hz.xingfuxueyuan.xyz/gtacsrxvsk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yuanzhike.top/gtuebdmukh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.haohaochexian.top/gtivyvamuy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtozhpbcdl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gteguybmsw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtbvnvselw.html

Go:   len(arr);  len(m)
来源：http://hz.zhongyouzk.top/gtfubowpit.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtlpmkyrvi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yangfankeji.com/gtkkumgzih.html

[P05] 判断两个对象内容是否相等
来源：http://hz.mhx1999.top/gtrioskpmt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.0kj1m.cn/gtrocdcdsq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtdpusonup.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhongyouzk.top/gtusjvhunw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydjk.org.cn/gtpvrdwfiq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cdnleiting.top/gtzdqhifsa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gthkiwqxvx.html

Ruby: a == b
来源：http://hz.chenzaomai.com/gtxkzmelfb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jlsjyb.cn/gtlpxsylxc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gtmnlviqxi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtasorvnns.html

PHP:  if (empty($x)) {}
来源：http://hz.hysaishi.cn/gtinotmyms.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtjjcdjjwz.html

TS:   if (x == null) {}
来源：http://hz.9152youxi.cn/gtfumqlxth.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtxewrkbes.html

Go:   if x == nil {}
来源：http://hz.zhijiandao.cn/gtchfmmfzy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.snrcjt.cn/gtegpvvvch.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtcztkzgjv.html

[P07] 防抖与节流
来源：http://hz.chenlongwang.top/gtacptqpfd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.c1oappe.top/gtznupnykb.html

PHP:  // 手写时间戳比较
来源：http://hz.cashguo.top/gtvfccwpio.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtcrlckson.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtabnjkcoz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenzaomai.com/gtwfyocsyv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gtttlzjvrn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.9152youxi.cn/gtvzxyabxa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sufxvd.cn/gtbrvrgcqn.html

[P08] 处理浮点精度问题
来源：http://hz.ivvv.top/gtbfusoosp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgfzy.top/gtyyxpyydb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtuboclckt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.mhx1999.top/gtwwnrlptl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ybcxt.top/gthtfxsaml.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gttwivmtsh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.pycfn.com/gtyjuxngkp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.andypj.xyz/gtfhsurvge.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cheryme.top/gtjvidtmgi.html

================================================================================
来源：http://hz.jinqigfzy.top/gtptgcwolt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.redwolf501.top/gtegfyyvvg.html

================================================================================
来源：http://hz.xuanzx.com/gtyqfchqgu.html

[Q01] 创建表
来源：http://hz.jianghu66.top/gtbztlxjoz.html

CREATE TABLE users (
来源：http://hz.shuidangran.top/gtifjuewes.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtfmnoocrw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hammf.cn/gtroowdoqf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daxiang520.top/gtzbbuhvwd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtfmlkqoap.html

);
来源：http://hz.zhijiandao.cn/gtpwzqzlrj.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtweyzwkxb.html

CREATE TABLE orders (
来源：http://hz.sysykeji.top/gtaaykbldg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtbuiibghv.html

user_id INT NOT NULL,
来源：http://hz.jqgfzy.top/gtnboqgfrp.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258888.top/gtgivvqykw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.mhx1999.top/gtutnyqeby.html

);
来源：http://hz.nanxuanxn.top/gtyeaqbfmy.html

[Q03] 增加列
来源：http://hz.tianlin.xyz/gtbplplvyn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangdashe.top/gteslvtvcw.html

[Q04] 修改列类型
来源：http://hz.gogol.net.cn/gtmgiuzboh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guowangkeji.top/gtjlmeraup.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtqsysdiyw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dashuyun.cn/gtxaddwisj.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtamkwutlr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtshdqdfqw.html

[Q07] 删除表
来源：http://hz.shanyushiyangkeji.top/gtjukhikku.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shuidangran.top/gtyxhzfrbe.html

[Q08] 创建普通索引
来源：http://hz.ydjk.org.cn/gthxqftxpm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtuelgeoeq.html

[Q09] 创建唯一索引
来源：http://hz.wangdashe.top/gtnjlxnbfo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtujrwzipv.html

[Q10] 插入单行
来源：http://hz.aizwys.cn/gtpijitwjw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtzuzutssa.html

[Q11] 一次插入多行
来源：http://hz.chenlongwang.top/gtmlsxgzqy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cdnleiting.top/gtvlbgzneh.html

[Q12] 插入后取自增 ID
来源：http://hz.jinghuilouyu.cn/gtbzergzjb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgfzy.top/gtljzoycgc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hammf.cn/gtyyynjpao.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gtnabwobkn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fzhhl.top/gtevpckpzb.html

[Q14] 存在则更新（upsert）
来源：http://hz.cashguo.top/gtikudasqw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigufen.top/gtbulwxsza.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtnjptixyq.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gthrbopziu.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtmownprnc.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gtusjqpgsn.html

SELECT id, name FROM users;
来源：http://hz.sxryk.cn/gtupqrcbzf.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gtsvasstfl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gthectmyih.html

[Q18] 模糊匹配
来源：http://hz.guannengcc.top/gttstourox.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangshuangyany.cn/gtorcrbogq.html

[Q19] 范围查询
来源：http://hz.shanyushiyangtech.top/gtzyxbnekq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xingfuxueyuan.xyz/gtlyhzfvud.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gthtzshylz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gtvdglzknw.html

[Q21] 空值判断
来源：http://hz.jqgufenzy.top/gtgbpvlaxy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuxming.cn/gtxwxsbcra.html

[Q22] 排序
来源：http://hz.ivvv.top/gtlucntawt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtgognmxov.html

[Q23] 分页
来源：http://hz.c1oappe.top/gtuuzdfopx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xylfe.cn/gttrlbimqk.html

[Q24] 去重
来源：http://hz.cheryme.top/gthtscreie.html

SELECT DISTINCT city FROM users;
来源：http://hz.iojbl.cn/gtmyathqab.html

[Q25] 只取前 N 条
来源：http://hz.52xcode.cn/gtsunbyrpi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigfzy.top/gtbbeibviv.html

[Q26] 计数
来源：http://hz.xziqi.cn/gtjwssrkrf.html

SELECT COUNT(*) FROM users;
来源：http://hz.9152youxi.cn/gtglapukab.html

[Q27] 条件计数
来源：http://hz.cqqwz.cn/gtbadjykpe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ppjwa.cn/gtkspldylw.html

[Q28] 求和与平均
来源：http://hz.jinqigfzy.top/gtgptncwgc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtvkbpreww.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangtech.top/gtxmtzmiiw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sxryk.cn/gtqpyqtjce.html

[Q30] 分组统计
来源：http://hz.316326.xyz/gtcivkiije.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtdwllifho.html

[Q31] 分组后过滤
来源：http://hz.jinghuilouyu.cn/gtzinhwbha.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj202588.top/gtyqspxczg.html

[Q32] 分组拼接字符串
来源：http://hz.52xcode.cn/gtazzxbfdd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtvhweyuvo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuanzx.com/gtgyluzwiq.html

[Q33] 多列分组
来源：http://hz.fengsongda.top/gtzvlynoxb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtupuxlvvn.html

[Q34] 每组取第一条
来源：http://hz.jinqigfzy.top/gtapajirjw.html

SELECT * FROM (
来源：http://hz.yj20258.top/gtydbbslas.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hongshengwenyu.top/gtjneeaokw.html

) t WHERE rn = 1;
来源：http://hz.jqgufenzy.top/gtlwuocfzm.html

[Q35] 内连接
来源：http://hz.daria6918.cn/gtknhzuvmy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtcszmuqvj.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtbtthcjde.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtgybhvjhe.html

[Q37] 右连接
来源：http://hz.sufxvd.cn/gtfiwfqjvu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj202588.top/gtltyeprkw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.andypj.xyz/gtaawxnogw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtidgdthtw.html

[Q39] 自连接（查上下级）
来源：http://hz.jiagoushi.top/gtrekrexmw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtwslaecpl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxinkj.top/gteddcarnx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fzhhl.top/gtaqbakqsd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtcaoawetz.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtzahxijzd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pengpengdd.cyou/gtyrpcxned.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj202588.top/gthumxqsvo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenlongwang.top/gtyqbafphh.html

[Q42] 连接条件附加过滤
来源：http://hz.pengpengdd.cyou/gtodczfoli.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinghuilouyu.cn/gtjmvhghui.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtrcdxersb.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gtzxxamaot.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtjzjvcgja.html

[Q44] IN 子查询
来源：http://hz.ydzc1.top/gtufqpfhgl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtueitrzkh.html

[Q45] EXISTS 判断存在
来源：http://hz.gzhubu.top/gtxchbevok.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtsuyliqdx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtbgryjixo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtaimqldkt.html

[Q47] 与平均值比较
来源：http://hz.cucudq.cn/gtnwuvuwal.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuanzx.com/gtxhbsobyv.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtemnipbiq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ywan-chungtsiang.top/gtnaaycejh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gtqnwcpqrn.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtfbkltaqn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtdztlxmhl.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtixmvytls.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gzhubu.top/gtrwvrffdw.html

[Q51] 用子查询更新
来源：http://hz.aizwys.cn/gtypvkqtrf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangkeji.top/gtnjfwrfla.html

[Q52] 删除指定行
来源：http://hz.wangdashe.top/gtocswjody.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtshajwgoe.html

[Q53] 按条件删除
来源：http://hz.hnxiangtu.top/gtussferdi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gaohongyu789.top/gtjjfgnbzn.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gttnxytliw.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtsrovmgxi.html

[Q55] 排名（并列占位）
来源：http://hz.ydjk.org.cn/gtsbrvjwnl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtoiwxrfwq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtbazalwtw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhengqikj.top/gtexsnpwem.html

[Q57] 行号
来源：http://hz.guannengcc.top/gtslnnpane.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.mhx1999.top/gthgsqutim.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gtgawixhrz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gtvegtsfad.html

[Q59] 分组内累计
来源：http://hz.hysaishi.cn/gtnakgpbur.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhoulong.xyz/gtcnrozbrm.html

[Q60] 取上一行 / 下一行
来源：http://hz.aibaodan.cn/gtwbzahnvn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxinkj.top/gtbccknpjq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenzaomai.com/gtdmpzlmxz.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtxedzxtac.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtjxcialuu.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtjrqiqrao.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtfgqusdct.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gtxrlnpalj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xylfe.cn/gtnsoettoz.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gtzhafvvba.html

COMMIT;
来源：http://hz.birdmap.top/gtnednjtnm.html

[Q65] 回滚事务
来源：http://hz.hammf.cn/gtknrrnuis.html

ROLLBACK;
来源：http://hz.zhaomingkeji.xyz/gtlkpagusw.html

[Q66] 行锁查询
来源：http://hz.yonumen.top/gtpjuyfnct.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtivfzrgwi.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gtjqjstcxa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gthdjvqbuz.html

[Q68] 保存点
来源：http://hz.chenzaomai.com/gteuofacql.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gtepegkekd.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtcrlhujlj.html

[Q69] 查看执行计划
来源：http://hz.redwolf501.top/gtvoxcqitx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtzmwgiizf.html

[Q70] 更新统计信息
来源：http://hz.9152youxi.cn/gtuqhbpsie.html

ANALYZE TABLE users;
来源：http://hz.gogol.net.cn/gtgfbjamrb.html

[Q71] 查看建表语句
来源：http://hz.sufxvd.cn/gtzdhafjjz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aibaodan.cn/gtfcxjpvro.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtvvehamyp.html

SHOW INDEX FROM users;
来源：http://hz.hongshengwenyu.top/gtzmshnccm.html

[Q73] 查看表状态
来源：http://hz.hfpthk.cn/gtmvbwjihm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtnybcyxrg.html

[Q74] 强制使用索引
来源：http://hz.haohaochexian.top/gtjqzdlpcw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtxpqomxfw.html

[Q75] 日期格式化
来源：http://hz.ydjk.org.cn/gtuwzgfzvw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gthnrdsvpx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gthnedosxp.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gtqhvbucrg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtwbytzmzc.html

[Q77] 时间加减
来源：http://hz.yanxiufei.cn/gtvntmncjs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jianghu66.top/gtkdmddgcf.html

[Q78] 当前时间
来源：http://hz.tianlin.xyz/gtobexmgkz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aibaodan.cn/gtrjpqkxzw.html

[Q79] 字符串拼接
来源：http://hz.sufxvd.cn/gtuulgwjsr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.meibo888.top/gtthwklmys.html

[Q80] 字符串截取
来源：http://hz.aizwys.cn/gtpnitecuz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtdcpshxhp.html

[Q81] 字符串替换
来源：http://hz.guannengcc.top/gtecgejwwo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hysaishi.cn/gtkyflvlkv.html

[Q82] 字符长度与字节长度
来源：http://hz.cucudq.cn/gthpbpeinp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydjk.org.cn/gtedaqkdif.html

[Q83] 大小写转换
来源：http://hz.chenlongwang.top/gtroazfixz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtaznoqgpd.html

[Q84] 去除首尾空格
来源：http://hz.jyoumei.cn/gtgwalclln.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnqzz.top/gtudmcklsv.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtxqxavdeg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gtclmfhgsr.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtsjckizyj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gaohongyu789.top/gtqcxcznxk.html

[Q87] JSON 字段做条件
来源：http://hz.meibo888.top/gtkwpqnrii.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yueranfly.top/gthwqmfjfs.html

[Q88] 行转列（条件聚合）
来源：http://hz.cdnleiting.top/gtkdervcff.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtmuthmrjf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydzc1.top/gtesamjjex.html

[Q89] 判断表是否存在
来源：http://hz.yj20258888.top/gthpsfkxyk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtftilnsed.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gtuqbsoppg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxinkj.top/gtxsdhzfdt.html

================================================================================
来源：http://hz.zhongyouzk.top/gtpccfwwgf.html

R. Bash 专题
来源：http://hz.shanyushiyangtech.top/gtspqfexao.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkyhgdhrt.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gthvbfzcdz.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtvgtjllrf.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gttoatmjpn.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gtlnngdijm.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gtxrykixbo.html

[R03] 只读变量
来源：http://hz.zhiwuduotai.top/gthmplqovi.html

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gtxhndpjqt.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtqdfspgph.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtspteivok.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtgnleyxyq.html

name="${1:-default}"
来源：http://hz.0kj1m.cn/gtqvznazzs.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtsjugfcqa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtpyoakzvt.html

[R07] if 判断文件
来源：http://hz.ywan-chungtsiang.top/gtgicpnbjc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtzexeehki.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gtofbjrrpb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yvedp.cn/gtunwoncbd.html

[R09] 字符串比较
来源：http://hz.snrcjt.cn/gtdkhrroka.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtuakeacjy.html

[R10] 正则匹配
来源：http://hz.aibaodan.cn/gtbriycrrp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinyuanbaomall.cn/gtixqerqdr.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtikvpkgdd.html


<!-- 参考信息 -->