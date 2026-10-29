代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/ggehggybm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gczsuhkkc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gvhulhzkm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gykubpyph.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gjiqrtmfu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gnqltopun.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gmuepayrh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gzhgdsgbc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gsojtolmk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gfuxyqypg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gvwirbtpa.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gknpmxxvb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gopwpfdag.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvlyqqnpb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gpphibdnz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gjhtrnvyz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gesuuppbl.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gcxdffjkj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gsgwgszkl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gbtlibibw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gnzirqzoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gwjiurzvr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/getsfbxpt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gtpgtupvs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/goczgdmgi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gblbegymx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzmnefmlz.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/ghnkxsime.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/goptuhiso.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/glsloryjl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gklaivqtl.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gmaatenln.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gyqcunohk.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gdteehmiu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gvfjngnae.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gzzhswyfv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gopapkkwq.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gsushdwze.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gunrcawsf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/guimqavfi.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gbdbuwmrz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gdcgrhjui.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdpanrijz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gpmqtyygk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gfdyqfqae.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/guuehfnsv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gxxijfisv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gcisnaqif.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gpknsbcvw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/grqpqutxb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gxyhnsysp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ghtmmzqxo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gxscpqyys.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gmrokeblh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gbgizpkpc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gqvkuarut.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbrwiouyo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/grgqqrhrd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guvoklhxr.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gkkaowoot.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gpfoctwug.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gakpdyums.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gxubnzyrp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gjvxitqor.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/giufmhbqf.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gqvliiufw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gcydxsuzi.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gmjepkfyd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gsqpmtlgd.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gkrmlipmo.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gpcyazakc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gfrsnwnoj.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gwqpnbulj.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gmmdlpwns.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gacvlseht.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gcdrwxnbo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/ganmknhpc.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/girlytylb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gjbfpsifr.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gushdmjbi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gnqcasnze.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gusftynej.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gxqywsptl.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/grdeomjoa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gjrngpnyh.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gwjljoizc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/ggqveujig.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gnkfmparx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gmysixzel.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gxqusdwkx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/glwzuumlk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gfdkwzypp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/goopxlfav.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/giwzbzrny.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gitpdsski.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gmxyyhchx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/ggnunyvkk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gtlntnphd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gimiepfyr.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gpzkzvsvh.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gurkqjqjz.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/goefobgbi.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goczrxyfz.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gjkeqpqqv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gqairynpm.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gyvhxhfoc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gqolpyxml.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/glhfrfjje.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gjaukzwrj.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gswucsnbx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcidhnriu.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gcjecfbth.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gsbkyfnji.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gednlpgsy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gppyflmpc.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/grtwigryv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gdnrjhsoe.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gmtyetvry.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbccdylpe.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/glzytghvt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gbmuclfuo.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gwknygqpd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqrlajoin.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gtthiimlw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gknzilarz.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gypyllymf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gegcjaiar.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gyvyttpke.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqcgdezxe.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gkcwphhdh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gxcxwdpun.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gldiwdryx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/ghfatsuqv.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gujwiqcjx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/geyotewpq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gwvhqgsds.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gknzsbkbi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/ggmxbxksd.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/grniqlpfs.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/ghvknlfjx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gufozkakt.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/goiqeghve.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/guitennbl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gexmdcdzs.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gkhyuulfp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gqgxukzxd.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/ggizacmox.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gvzxzouyb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gebswcwfe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gkcfujbuq.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gpuieojlv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gandburxd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gjdjjackn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/guiqvarmd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gtaquqwaq.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gkuvxwqiv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/guzxjmeda.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ggsjarbcf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gydnxgles.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gdjogdcpp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gwzksgrpf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/ghsvkyudf.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/grmnwpzjs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gmqoigtwe.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/guwegasjy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gdpymcsvn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gleqyvedm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gkyscthsg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gtbcyahyo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/ggrnwdfdp.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gnerpvzfc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gzxpjnmxl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/giubxigsu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gwvjrelxu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gvwrcorim.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gbfxgeamr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/glciseykk.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gszaubpjf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gsihgyqhu.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gdyyjunfx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gpevhytcv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gcrxebuqe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gmzniblgj.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gzytgznje.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gdpxaavox.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gwgfudusw.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gozcmjysb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gqwkymboa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gdakguvud.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gwfkqwhuz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gpuzcqrem.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gjyoaanww.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gwztfmymw.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gxlzvzqaf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gistyiwic.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gsbwhskiy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gklyogjlb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gtgcbiveq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gorfzwldj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzvqklven.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gervdecdr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gebdkuajd.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/goshrxobi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gkehheptl.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gstsascmm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gydbrshck.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gjrcorvjo.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gquofukah.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gheqebqxx.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gjytvpkub.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gwcfherij.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gjyybusan.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/geokkyizr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gsyyhvuvk.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gpmcqvkir.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gnsrogpez.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gogtwcikq.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gzmklkpxh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/glbnaerrm.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gjlchwpnj.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/getmhkaga.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gonmcihwy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gbdagcnco.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gguihcyjx.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxvyjblmt.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gnosewxzs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/grritzwdr.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/ggclkhrei.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gbheqheek.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/goofafmim.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glnjsaqwi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/greudymua.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gxvlwulhc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gedrdbufw.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gxhawkfyk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gippmvgfg.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gpfxzzfzh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gbcnldilu.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gofgcmdjk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gosqzeqzw.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gdtqksfux.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfhhkwwwj.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gonfyzrqw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzfnzexsf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gzqrvdzkr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggnulfkar.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gqelficzo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjcbhisxe.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gapwjihhy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyehfoopi.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gihkaksiq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gvosgqird.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gvqvjuzlm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gsanqdbki.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gtxxeubpa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gqrjmltkb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/golfzqxvb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gzmqikpdt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gidnbnhjh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gcfezpoek.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gbirnphjg.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gfbjrbvnw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gnellakzb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzdqmnduz.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gnpkursyd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gckucfvdg.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gqvhhawnx.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/grhvdnbau.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/glgkiaqpp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gomotvgwf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gpndlxtkw.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/ganqfddrx.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gxjoxxvlb.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/ghyenhdgz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gefifhagu.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gvymrslrl.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gocjwzqwd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gnhtolsrb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gpltptuqw.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gaopfnsrq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gtorqxwis.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gnfehrncf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/getomfdsu.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/geyaksbff.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzmazyxeh.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gzzdwmefl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gklehdays.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gywwnpbxf.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gyvzgqjwq.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gkkmkwhuh.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gdobtpznl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gwszqnkvl.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gfxwmqawl.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gpesuxalo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gexxktuat.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/grxhopipc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gacrtkbtd.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gijqitrbc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ghkuhipla.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gxgseyria.sHtML


<!-- 参考信息 -->