代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gtvkcflsq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gcilcmmck.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/glykngghm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gubiybvqx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gsybssbfr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gewmqccym.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gwjzumcyp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gojupniux.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gflywjiqn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gpbveqtlw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gdazcchdd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ghdfmwsfb.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/grvravyst.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/ghdzbwnbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/guxafgnss.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/ggkkpmfrq.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gcfgpsrkn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gacogezie.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/ghkofmecy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvwwpjwsy.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gkiziqpxt.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/ggoviicri.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gxkblrdrb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gohdmlplp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/geygummiq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/ggmazuszs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gajfogseg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gduthgiaf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/grurwbotu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gjpybowul.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gdphgyqnf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gnaqfigrh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/glygkjgbw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/giesywhhm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gvylcvfle.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/glezntqjm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gajczomnp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gspfznpzn.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gdcjcixtt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gelvfypco.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/giitfouwy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkhoxshpz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gdpkpydhx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gucwckqmm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gvhhfatpq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gegjcclut.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/grufimnhj.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gvgkgjpjq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/glvzcpzji.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gdoaecdyg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gkwzfcyyt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gqhwftozp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gqdwolopw.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gfvmsuyqx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/ghlkmlizl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gedgnodrt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gxposyzbg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gwrcusdye.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gbnsnmmin.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gmzxxqbvx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gnwtyedii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gawttuult.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqkzcedmv.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gltgpcqqz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/grwuvtyja.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/glepeimyu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/geqrhbpvv.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gglftpdge.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gswlenaym.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/guzwiczch.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gilmhgvrq.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gioylpifj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/guqeneclm.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/goiidmlep.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/grfmjfjlp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gwhmgvnyb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gtvstwtyn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gebtutlfp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gixxkninn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gigvljvka.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gvpjyewjg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/glnwlenpc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gwxoiwnzy.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gdltzmrgj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gqaaaqahs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gtchalgaz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/ggztyzmzm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gpjzzdihf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gfzshfwdx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gqpounoee.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/ggsxxizcp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gjnanfook.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmstkhkmg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gueizoazi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gstypmigj.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gfxlhdjrj.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gnfdjpmgq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gvdloyqof.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/ghwpoigoj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gpywuqrju.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gjgvfkmkn.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gvlgigrfw.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gqksziibi.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gemizywtg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gvpyxrzyp.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/grqiygexb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gjlgfndui.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gsuysispz.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/giuzqwvql.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gjgppgsij.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gpsbovjxk.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ghnnphxiy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gnhxhbwsi.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/glqhwjhyw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gzxsxfgox.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gctzghajv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/grrutxcie.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gshwehazw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/guxgvzcsk.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gaavypecl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gblbzrcma.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/glkqtvoku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gkzhmtxyf.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gtvhanuaz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/guvqtfscm.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gjdbqkvqr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gvdaunrit.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gspkfynfx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gfsjatenb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gfciupwzd.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gfedznhyv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gucvtfsmc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gpgvmyrwj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/glzrmjrqr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/giesinpyn.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gbfxgvhhh.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtclfdvut.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gnitwzovn.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcvdrernr.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gphygndcp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyiqdorfd.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gmcuqsyrs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gciilqctg.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gzgunaaii.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gvifulerl.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ghjhitpmb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gigytkvwx.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gjsmdaitk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gmgutohbd.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/ghghakpvf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gtfhqxkln.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gdnnbuwug.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gnjsqugvd.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gpgevluvl.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfolzzsnh.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gtlwqbijb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gnhiuqtlw.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gpoykkmfg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gryxkhzuf.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gvyfhutvp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcphpiied.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gadbmgwvk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzitpbcol.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ggsisgxov.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gddbunxnc.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gqxgbnrgj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/grnymfhmn.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gfgokgxrh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gcosrxnyd.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gmloxburl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gjgouvnip.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gzgsnqeji.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gcoursthb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gotfbjuay.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/greeuwcpe.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gcouwvsev.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gqmsgyfvz.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gviszlnhj.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/geacfqxmq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gukavlrcx.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gujkbnryi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/ghjutbghn.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gvzrdjkkb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gjbpolbif.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gqhmfgrdu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gzefjuand.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gpejsmsqy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/giyoaikmh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gykmtqisd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gzvwsazvi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gaadjimxs.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gmrmmvtpx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gnezazouy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gyiuowmeq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gjxuvdreo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/ghfwtsrsw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/giexhdwpr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gshtxicbq.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gekjfxhbi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/guebkdlnp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gfapokroy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gxcmerxec.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gshqjhzeg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gahteilum.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gmrngcjea.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gjetkhvta.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gzkaochfa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/geyvjukax.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/grtmzdxhz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gzpkmvtys.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gmsfdacho.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gmpqaoeod.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/glefqqjie.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gonawxguu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gzczfqvmv.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gxzkvppbm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gnltnrazm.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gcdjaahmx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gabiougzi.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gbooipweu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gyzmivval.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gsnmkhmzi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gtdrtegxj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/ghaoikxzb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gfamfvhim.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gpcaybdwf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gflrrdzdc.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gojslpkij.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/ggxmbpndw.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gmmodoosx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbotdqvdt.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gortpwsid.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gokukynkc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbqbmmi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gehgzoplj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjbjqvllk.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/geaupwllh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghcmfovgj.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gtmiloxrx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gdsrhfwai.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gsudbwbjn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gmlbkpkxh.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gbzpqgygr.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gzevopyvp.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/glnofmchr.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/geeinutvp.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gxawrerel.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gzoswbrkl.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gyiighepo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gqzgalcmu.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gfwkxrqfn.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwyzwgphn.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gzwyrbrxt.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/grbpchzfe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gfjhylgls.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gnohnlgaz.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gqxinlwvx.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gtgkvryhh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gxkxmhywb.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gpaksleem.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjslykibl.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gfxwhkngw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gyavskjpn.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/giyrifwvb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/grypmwtsc.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gqwfhzhng.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gizdglqeg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gczitrvpy.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gjxmjzmjk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/glbxjhysw.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gonwafasy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/goklqldrr.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gndosbwcl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gkinpesmt.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gkitqascf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gfhqpdnrn.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gilkkhqgt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfovyglfu.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/ghodhdyrb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyrnyzjza.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gvyxqmzxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwmmzuvry.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzsihuccq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gepvtrmym.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gqyijyboo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/geqrqfxpc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/ghywaicpk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gdtysiqbq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gykzhapkx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gssbfizya.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gwomzhqgs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gwyrzkfhr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/geknmkkcu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gwvlwjhdd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grqguavbw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/geiwkneah.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwfaydu.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/golgxqdef.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gjfbrbsdr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gajlgxusv.sHtML


<!-- 参考信息 -->