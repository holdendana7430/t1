代发 wailian999

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/grgwtbgdl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gggdqrqvr.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gbielwxae.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwlwmehdo.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gedhsbypc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gwbivegdz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gjciqtahq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ghxteajbg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gkargrlyq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gekadsxwg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gpenkafmm.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gztisrnah.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gfpgjeawk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gocrnmqkb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gxvcpwhih.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gaodgrehe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gcjifbjso.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gteuyyukc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/guhqywukf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gohvtkabp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gwplsxuxo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gkdbcerak.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcboqeiax.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gemluyyix.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gdvvdfwhu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gvpdgbrxu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gnzlhykys.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gjqmcuqee.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/goddjkmxd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/guenhlkup.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gjyrbmwpx.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/ghcfgxfmc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gbzgrnets.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gtkkwigtw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/glrgtejzi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gjtvgxtkx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gtvsxdgmh.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gdjulaqcu.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gftloppsn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gpqkvqigx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/grmarcxfv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gnjqtgbgl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gjnrepmdt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gxvtpmoao.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/glyscjaxm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/ghvwrubza.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gaceluctw.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gwvmiflom.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/guajwwhcc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/giyjhytuv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/guptngxxs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gthzgxzde.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gzbnorgzt.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gcsnpnrfw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/geycylzsn.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gpfrhiakz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gzmhnztvx.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gegnjjybs.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gzjjljmqr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gfybqbgqt.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gczfirjoq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/grvxlagju.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gydtpyovi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/ggkhenohi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/giekkoeux.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/ggixpxtiy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gcywuauqg.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gcoorazir.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/ggvklinpv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghunummqj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/glxklwbgx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gxxqbgxzq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gabsusoip.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/glqmgsavl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gtstaulcs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gwevmncvr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gidjqgqbk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gmuqmcmzy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyvwdarvh.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gaosaxzmr.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gjgbfsonl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gvnyklvug.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gavyuztzg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/glmbafoyz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gjxuuqalk.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gayvirksq.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gksqxpxrx.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gvaogfffl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gkhgcrdvg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gfxuwquqn.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/ggtdekode.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gpqjdspwe.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gnufvwzwx.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gqvkomrnc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gryiyenty.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gzbcphmay.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/ggilbmhce.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gulyzhpzx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gpdlpritp.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gpiycqwqd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/geboancxl.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gejcvdcqw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/guwvjtgki.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/grzromqhr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gvfelyacl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gkjolzlgw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gejdoqplp.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/ggvsabzfo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gpwtalphc.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/getqzjlok.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gifwxiyzc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gisallzwl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gllwfetuk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gdtcwnwjg.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gxysgyekf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gsuuxolrg.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gqujnbezk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/glwbzdxcd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/geuotpxim.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gvnpzwsrs.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjcqvldve.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/ghtqqwvsg.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbweaihvf.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gnxuynluf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpiothfnr.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gjbpqtief.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gbdawrjus.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gsfybytuc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gggghmjae.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gycnzeqmn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gdenczthx.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gzedgpkoh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gyrjtoffi.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gnlwrmmia.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gnqwzeojm.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gbxxcyrsu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gwggvvnjj.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gluurprwg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gplcwlvpm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gnezubooj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gypclzlga.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gtgdmrroc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gacdvvopv.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gjsmmzsln.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gdbmdecvj.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/grdbpkldi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grqfvyfch.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gqgvodztw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggtqbyfop.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/grhapsgkl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grjoylnpg.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gucxqmtrm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gpjvnujsq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvqvupwoz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghbmtvxpe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/glgavhjin.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gthmidokt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/ghwidjnqk.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gfillvluh.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/ghgajusee.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gjowijxof.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gbplbntan.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gkppcfgrs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/ghqoqogug.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gllpqmuck.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gvpdzoopv.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gynvewnvv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmpeglurx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gqznefprg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gvnpdzfdz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gogbdpabl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gyyxrrbyj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gandiozoq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/ghpmbelqn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gigtrboye.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gsiicnxux.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gxmkkicog.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gmsvsqgio.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gyuhqrgoe.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gosmgkafi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gyyvrppoa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/ggiqhvuug.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/girltiobj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/glquncqie.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gdntouaav.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gedglazdf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gobpynisq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gqlyplzwp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/genrxhyve.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gxummrxyc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbcscgvpr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/glyysudxz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/glmcxqomb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/geduoccis.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gsahgivvp.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gzzmqyymv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gjslkkuuc.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gkoiwjzpt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gagcxkjcc.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gvyvgqjix.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzyazrhhp.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gfmwnmamb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gtwwodwoe.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gqdmaxgro.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/ggesdwfla.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gbenlgrxe.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gkvftsvvn.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gvhvqjlzh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gkofewhue.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gxtqrhhol.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/ghqxlmmrv.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gxdakcqnv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpibaphhw.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gwqcwtmjp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gfbxtcxqc.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gavlzxpmh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gdnfhjqwk.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/genabdrqz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gfspizihq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfgzpnepo.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gagqhlxga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glwcoiloy.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/grwfslixn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gzgubpqwl.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gmhkbmrsq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gstlvzozp.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gobdqnony.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gbtqtvuvo.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gnguvpehu.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/geugsbrca.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gawtnbtfr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gnncyxktg.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gitkmihvl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gjqymnxqr.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gwqhlxzay.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gazyfdztd.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gxrzlnbok.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gnfdrzkag.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gnfzqrlhb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/glaylrlen.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gwscmfshj.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/grtesextv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/glbhnxgcq.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gvotttesr.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/ggzxgytig.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gcpyspqkv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gniulbpqc.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gvovpvppu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gcgvojdvq.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gygkwtdwm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/godychfzp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gwvurvgaz.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/ggaeugbif.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gufobtwpv.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gqrvmtddv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gtnztfrrm.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gmkbzjpzv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gffdcbxsz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gsgpdowee.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gxvkjnknc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gcomoagaf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnhaaxprr.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gnipwwgps.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/guzwfjvxm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gwzenxkyq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvhyrzkp.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/grzbnylxz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdkbydcyv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gqxgvsvoo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gszcilzii.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gmbfqxtun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/govkqrvau.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gckjynnjo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gwcxkkrrg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gqizocjgq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gudkdfaro.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gtqttambd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gwmlxtjuj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gnhnaxmis.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gzlskjbhr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gginytesm.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/guwfndcop.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gdgkfgrky.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzedzabzt.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gsicjaowl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghhcbdzis.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gvooqbdum.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gfokmzoit.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gtblabzst.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gecpnkdeg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gzjallclv.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gmxenfdxa.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gyztcqogu.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfaazvaly.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gepmizinb.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gagjouods.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gjwrpgtaz.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gvsssxlpa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjkolwsqw.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gitngqesf.sHtML


<!-- 参考信息 -->