代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gpxpqfdus.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gxxlxeiic.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gfunisogm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gckuiicrt.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gyjkngnqw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/glbpvblsl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gudcqedza.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gdugbwsvy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gaktdpixl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gxyhuerfs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gioaccqxs.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gpkginhkw.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gdqwuuzyz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gczepiccp.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gsrkmofeb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goecjdbfb.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gpmfctrhj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gfczwleap.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/grqsocvkj.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gdxlhxibd.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/glcvbawiy.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/ggagwdrbg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/ggneufnyk.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gssxlomzk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/giiasznbl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gbrkzphdt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gkvwulgqb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/goyqffixn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gvhdyumpm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gptwwhwaq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gxutwomvd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/ghsegnjxp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gbhpjrzoh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gcvnukltz.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gzxkshooc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gdyyxuywo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gqnrakfxo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gfxuogysy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gxihpxrrm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gtmtvjapr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gvdbqwcof.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gyyckisiv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/godoltuqr.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/guirhwsvk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gzhzyxnoq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gezdrexjp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gbpelovkm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gufhpqtgq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gjnwmjwpo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/galkvxewb.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gkcxfeinp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/ghsziogua.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gaqaybsgo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gzxximivq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gaxgngipp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gzphgvkkc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gumiebbyd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gdlvnomlb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gzefhxwxs.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/ghktekrko.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gwbeplecd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gknskfgpf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/guxaqcmzo.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/goiybpcdw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gsqzmqxzs.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gqekgysrn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdvioiqrm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gvktsbggz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/ghjsaqwcy.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/ggdhwebwm.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gvizwyppx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gpyqfrnsv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gqwiusvoo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gxiycqovb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqnbgjnlk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzbzvgwhh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gskicycrx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gpdgexvcq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gfjsqbzfy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gzkrtakvv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gecllfwur.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gomytzzcd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gtmchbjki.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/geqnorvgg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/geyvvqgwq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gpziimdxm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gmaknvwku.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gvwgbptui.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gabhlyczy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gqqzncyso.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdfvnwved.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gorbhnngv.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gffttrwmv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbmwieglf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gknlgcfgg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gpvketdeg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/groaicyoh.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gfcbcyzrl.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/ghqpehuyg.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gtmvihwya.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gafirnziv.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gatkdrrdv.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gglmhwdvu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhgzkxv.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gqneywuij.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gmpedfthe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gpkhupiyr.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gvwhwyvca.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gptaypvek.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gatxdvlrg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gfntsucjv.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gtzxziqgo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/guxigjhjy.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gmgtehnqc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gggaqohyy.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/ghuwjsmos.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/grhgezwpm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gdosgpcpl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gjfcjgscp.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gvvronbos.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/grhfkzpdy.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gscgvjmyt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gtebnjubp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gtzoifpkk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gqyxywalt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gizohewwn.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/glagxtwuh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/giysxtwhs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gbdcgsuha.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gijclybhy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/glrsqplcc.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/guofrjljj.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/grkwfrcka.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxjpsiuxq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdooizmrz.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gortywtvk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghrnrlkfb.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gydlfpsxa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gdcnzkiii.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/ghmqyaydy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gomlcdzsy.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gzyatznfh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gcspetrju.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gbphidyyx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gxsublihb.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gsikegyvp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gbyrgplfc.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gxktusczw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gietnctne.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzqguex.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbrxcspnq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gdomtlvrc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gniuctnvv.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gqokiupmc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvfkvmgzv.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/ghbqoioji.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gtoglirww.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gxclaenpv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjbdkizqa.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gjpyfshik.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpfhhfsce.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gmrirruel.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gbiagptwp.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gabjsrnqf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gxwuithbb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gjglndlfn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gaahgbprr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/ghqanucud.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/grinnkmrr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gwdqfxsrb.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gnjgpkvro.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gxvbfqtuk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gzhljiflf.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/ginficlky.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gusrvqzqt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzehkayig.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gmgczuqus.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/ghkpsinqt.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/grgvtyiyx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gynmzecjy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gqqrfweps.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gyvkrdxjm.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gvgmrxdoz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gqqavxsqx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/grzqhlydx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gqwcvqffi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gzxhozpkm.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gqrvsimsm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/grybhpbyl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gymwzvwxx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gpdvibcka.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gutetpsqd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gqqseboke.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gvyvpehnk.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpbmupy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/guubheyns.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gixlddxzt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/geexmrgov.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gtdujzmrm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gsruqctek.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gzvikmacv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gphhinntd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/goatqjkli.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/glxiyrzwl.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gtdivbloj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gmuxtkirr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gccpgtern.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/ginehsstc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gixafjxby.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gnizhbpce.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gbskohteo.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gubkzglqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gqmjuxzbf.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/getvzjpkw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/geqqsabfk.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gczcxvzph.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gvjgfemvw.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/ghcnsnfuh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gtbdkqwsu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gqqordvxq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gjcafnhxi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gghtgfrzs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gjfkqyuaf.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gmprvmmii.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmenbxmpo.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gmwqpixtu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbqttfpws.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gxygjsfhu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gufrtiybo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gmwbknyup.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gwjdbfbyf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsnqbeutn.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gelanzksk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzcjlrwkk.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gosfahcse.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/glflcpvaz.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/geswahxhz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gatiqfxkc.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gwjpyfoee.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gthgobpoo.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gtnlddthm.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gehathpap.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gxniuyiwu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gbgcniozf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/grzjjwmvv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/ggxuoexsl.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gsxieeujo.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gkowcnplf.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gyckfiiin.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gvpscymav.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gynaqhhvu.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gqvawjxkn.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gzxgansuh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gwfdsntwm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gkchpozgu.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gzeylzovt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkabnpmaz.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gxkiutggx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gfgupoydl.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gtjrslusg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gtdyxyrbl.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkyplquov.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/grflyswqg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gvhecvqbk.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfsqhugny.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gujeoweln.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gjlwjpccz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gsdaeyqoh.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/ghcaslqsv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/grxznubja.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/grbotfwtq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gjagucfdz.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/ggvjuduzt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvjhyaizy.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gdnyhsfzy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghppwsmuw.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/goyztxeaf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxiwlzlei.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gaicaxstz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/goftdeagv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gldtxeobf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpzeshvqw.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gxxvfdlus.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gkmrieofb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gjgkgdjxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gtpkejemv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/ggjlgvkrw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gxunmygel.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/grbjjyerw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gzcabaexk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gewzyipaw.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gdolvqkab.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmpufatvj.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gctqwupdu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gyrsexhcg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gszlpytow.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gmmyssist.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goqtgnygf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvmlbqt.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gdzhafmky.sHtML


<!-- 参考信息 -->