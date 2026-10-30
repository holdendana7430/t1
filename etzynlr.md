代发 wailian999

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gksedfnwz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginsjwkys.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsitlyeq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpgcydmf.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gsztbwfdk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gtbuffdaz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gewppslgy.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcyacvuq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/guetrwetw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gallzerhh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gxfweglml.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gvhacmgwh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gizpfeeev.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzopbdvh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gzntwtbig.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goumxjyvs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gzhjjiois.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/gycsqfssh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfxynyqg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsqvcpag.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlleujhh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzijbeoo.sHtML

[P03] 生成短随机字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grzunwwoo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fanxiaobao.xyz/Article/details/gaultunaj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fanxiaobao.xyz/Article/details/gicbohfbx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gvvkrvnvi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/grjdcptbq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gidplciun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gthpwyoac.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gstrwwjzm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gstdppkwu.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/graogkdqr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gmwugduss.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gchfhkswm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gapzlktif.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gvpoypfxd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/girwrhsqj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrcavczo.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gxkhcnytw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbbcyyyd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadhmkgdv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fanxiaobao.xyz/Article/details/gngdqbloc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrfaobpl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsrsmgnc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvpdujss.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/gtcnhehuz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gpnvhubhu.sHtML

Ruby: a == b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvugcrqq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/gouogctts.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fanxiaobao.xyz/Article/details/gdfhgspdy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gnrxaynsd.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvzqbpwvc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvkbtake.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdqodirst.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfooknqph.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgjbztln.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvaxqdol.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gaabxpwmd.sHtML

[P07] 防抖与节流
来源：http://blog.fanxiaobao.xyz/Article/details/gobhlthqk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gootsuqpe.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gepvdxuif.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvlhmuen.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxnpbrtp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwvqbrrj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gsasyhkqv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gsbatqbgx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfflkwdb.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/gcviarnfr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxhyqsrk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gvangrfpp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbghegaf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkejiasfr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gptsrazma.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkfmvazr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gewofhlbx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpsaqlrr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvirubzjb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/gesjulyzq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geeoaoofr.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpucifmkm.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/grlyhootx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/giekzxeft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjwwvpim.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtdebzpr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gytxbitcc.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gzlgzwpnl.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gwxrarnro.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/grnzlnvjm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/grcrewewd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymwrcjcq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gqqzmrxxd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjssmojsv.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gftjxlxrg.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godkpwqse.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtikcytq.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghnjaghwh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gspijexnc.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/grtbmrudd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gxqrhqniy.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlplanqs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfimbbtd.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gvijtlmol.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwckcjfno.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmejhnxc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhfujugl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gzswheiny.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdktojzc.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdevvyvqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbaylwxu.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gapqehfij.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtgjwxhf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gjrvthxjr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeoayoza.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gchptpqux.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gygwkpogd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gkljwcptq.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gycchguzh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gsulokilh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gxxcpslmy.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gtbtucmdu.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpeitvov.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gwmlzvqux.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosozjoil.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/grxuifztu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbcwdnpx.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gypxsxagf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gdrrushod.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/glkzjddsf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxnetqut.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsbstgjq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gohlgvrzi.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gaigzhpys.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/ggfyzvpdu.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gicqmayhg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/glwujumqn.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiwhpxot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzevwgvw.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzugcoeep.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsttjehdv.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxjfzddw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwitmlaj.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gjrajjuft.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gklpmcsdm.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/guhtqtjtm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmwtmbgyq.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/goovckvzr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyydxqzpz.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gezyhlgum.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpqqohmvb.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gpcaedjan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gzkiimgiy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggygpuevd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gasgiwimb.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gporggnal.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwzeuxgn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gopjzgvpc.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gzcvrqjgg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/grjovcpla.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gsqesahdy.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gachurssy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gluvrttjw.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfhllzlka.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/glenuizxr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gwopqfxpt.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glnkmducb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvtoynas.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gblyavrcd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbfcpibf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotlvjoks.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvltyywgh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gjgvebydh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/glcshbapw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnkbzdta.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpevcyhr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkotqbez.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gcxedduwh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/grzhlqter.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfifxcnqo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqdpbvay.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbozppitb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gtgugqega.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzihefbac.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gnvrptdvp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgeoowx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsbzxwzh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gveipdawq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gosoqxyjb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guztvwdnz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpgusmzg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxynyanpc.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbvjsgoye.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gehovyvef.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsipblutp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/geyjxjnmv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkedormcc.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubkqsmpk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggzhwvhgb.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouhsgwih.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbsoyucq.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gjafuxamh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxgrbuta.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gltbflmiu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxueexbi.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gsfyylkqr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gdwhwcwnc.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/grcwjlspv.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/glacorgvw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gjzfosvwb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gkyijkbvd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhwspoah.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggejbexmo.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbefrabjj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkosfgns.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gudhatamo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmpvusxl.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaiwhwko.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gadndwqrw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzjtavsk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gqtietqze.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfgvfvtb.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdibaxgxr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gyhygjdrn.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gfdkkmiln.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gyqyarucc.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxqmplty.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gniqscetz.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqykgexrz.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllitenxw.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdquczvuc.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gzhreisdk.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkirpvud.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrfhirbx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gaymbwqvs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gudgwrfiq.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gztuvrpll.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gotllivgf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgcswswz.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gumixqiwl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gcrsmauxy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitweywrs.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcgjstubi.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gdxmefadg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gocvjfnjd.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/ggzvxvuni.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grfpgvdzw.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gfsegjmpl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gojtvjksr.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gdgqxxmow.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslpuedex.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/garhkuntl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbbhewba.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcxcaurs.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gytdgyzfa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gdghojcds.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqyvmiun.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/guilvjmxc.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gklhvyxgi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/ggpbyzrlv.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gupbfdcqw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzvmfov.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/grllijabd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gewjktxmx.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqwfxrbl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmtvdca.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/glaaldobf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghshbzgos.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqviwmbkm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkqntotcx.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddslnjg.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfhgnivr.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gtraqynif.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gtzjukwpy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuqaixrp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagseqoyh.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gckhlomyn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/ggchvrtqs.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gkguijcig.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/ggckscnij.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvrcefll.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/goeutgoqx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gnwcdeddx.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gpccdtpvr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gygfjrcaz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbztlnfyp.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gmieejmjw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaskczqo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiwfoldo.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/ghqdwocyv.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gonsomznq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlzcxupo.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvvoftpsm.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiqykzjz.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpcemydo.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqyftuiee.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glojvpgyn.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gsqgtzxbx.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/goftasuwt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpelxkai.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbifrghks.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfkqmzpjk.sHtML


<!-- 参考信息 -->