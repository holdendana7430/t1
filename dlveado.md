代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gjbyhgvqp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gonbvctfs.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gwayvueay.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/ggsokmeum.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gbwrlresj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/geaqqgdro.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gztfxwmke.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gtjkvkgkx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gjsexlvot.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gizfhyqwz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gusvnwbho.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gtamnuscb.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/garlqxnig.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gfweybslm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gqjplqttx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gtfsxqlsv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/ggzqgmiwm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gltoslkpq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gbkjfnhnl.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gsnzoaqhx.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/goojaanim.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghhcxeyxp.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gvxcjjgbz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggqutdytr.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gdduzmjgp.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gddvrcfpe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gqyneqebm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gjxpscddf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gwrkvczhz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/glicpaoxh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gjtbwxajt.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/glhmobycn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gcnbuyezb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gcmqrscwf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/goctlijrz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gsiledddm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gdtgrqkfo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gdkoolxeb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gyyygnfkq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gifbxwyww.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gycjqbiul.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/grujpynku.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzhwmjk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gshsivqli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gmjlpctru.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gtoiekmht.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gibacypwp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gvmnogrot.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gjhsmehyf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gfnridqcg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gibipurof.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gnzeahtuf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/glymxefgs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjmstprhs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gktynjvmo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/grgpzwrtp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gczlyrnsv.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/glzuqjohn.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/glrmwmqvh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gqaigztsj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/guuknnllc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gpwlqsqym.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gnihoakui.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gwcrpogcu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gjrggacpr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gzboiyurs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gnqsijtuk.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/glretifsf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gnfkalvji.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gxmupexjc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gkzkuuadz.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/grgcvranr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gaqdkhytf.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/glxeteeho.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/glhffqnsz.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gvnnqcjqo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/glhsobjkr.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gzbipoqvy.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gymzbqboq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gajgwxpfn.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/guvwicpgz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gihnbeure.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gvrffkvxv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gtxlxrtlo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gdzudakgk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/grpggcsuy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gjyaatuyz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gjulxihna.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gaudbklyh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gwemryikk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/grzpgjphd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/ghyypcshk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gxmbxlimj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gtbvalopa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gqqnxhfxh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gmkpeuovs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gugrygyjj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gtlyqcoyz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdhdasdnh.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gcevheccy.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gwcscoqis.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gxnpysipf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gjzolugoe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gzqfyqxab.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gvqtlgoru.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gfobhmtgm.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gxmonvpeb.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gumfiigkh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gqkxpihlo.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gdrjqksud.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/ggidownva.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gpaassbth.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gzjddijpf.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gesmcydin.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/ggohftlev.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/ghpkmvrwg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwuebopz.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/guqgufamt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gwrojqrzn.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gxnmjdnxl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/ggvmoyjjv.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gxrjbdjkg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gdpmrcenq.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gaklsrrvz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gjojshzjb.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gearirpwu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gohuatklk.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gtgitsdqm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gzfftsoab.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gofthvysk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmlyywtyp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/ghysvxjlc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/galwqlgbu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gninwnzlf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gwnbfhxgl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gdqjsujcd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gveesxssa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gjxtldqpw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gfzulhirn.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gnouevyqj.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghavgmjbk.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gkroxdyge.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/glcmyzrql.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gdvdycoyy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gjjouwdjj.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gbpqnjbxu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcgnxbj.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gojckjqwr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gykcwhvla.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gwnuwngbp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gvdjulfhm.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gvegfbzou.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gjhpylxkf.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gsfylymkj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gwhhpcfgz.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/ggtmsbbsi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/ghvnuwgrz.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gqyjzpzxk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpdvaevzs.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gtookyqru.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gmlsutemz.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/glaqgbowl.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqfsukhfn.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/ghnbkyonb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gazxdtrww.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gddrxypev.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gsanvvmzf.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gghrsispm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjbcgfvfy.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gfuaaasdv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gxmmlbzsy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gksichnxe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gugqxvjzr.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gdfxijrzf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gunspqmon.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/ggtmrxdrs.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/ghufoxajk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gmiggijjj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gkovgpacx.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/giquxpgsx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gmsprzdmm.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gbgbqvvan.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gxwlotlro.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gwzkxtqzb.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gytljeflm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gamjiryhy.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/glqxhvjcq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gqgiuixuo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gwodxgqlp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/glxqoqdjc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gmwgtkyok.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gqlyslxvu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gtjfdbykw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gkdzmohxw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/giuznrged.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/guwhkapgm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/goqucszou.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gjlarhath.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gbaoiobta.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gaoszzdcd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gdiqznnqz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gcsokemjx.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gsqekqevd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gnyubvvdj.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gipecnvbg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gxksufwwz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/goeysidkg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gccustwda.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gylatucic.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ghzxtogpz.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/geldaidji.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gyxjepwnh.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/grbcjdvnu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gtffzxgwu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gxqromfci.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gfgzgddgd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gsogbrimm.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gplbhwcbq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gzpsdykrz.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gtigdvtuq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxhrkibxt.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gwtrmozno.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gdsagmfrr.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gtlredsft.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gwzjqffxc.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gymmgqnzs.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gwfsnvpcw.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gyzcdvnbh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfasfaypg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gsfmzajay.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/guaahqamu.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gkiumevlt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwkfdpsed.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/ggtbncmjx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gulilyehj.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/ggtqrloiw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsjdzaydw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gkoqnpimn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gamxcfskz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbzjmhdqq.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gzcfjnsfg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwxcekhsm.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gsfyafpgh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gjyvukxcn.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gfihecjve.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gyjviduqt.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gyfftatni.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gurtzguxi.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gwdumqmni.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gemlxwvin.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gkldifzsv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gdtjfgxub.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gwlwwoemo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/glbotlegy.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gkhunesiz.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gfumpupzr.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gbakzdoiv.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/galupmbdw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gmzzfbxdm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gizevgypn.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gbwxupiyt.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/ghfynwbdp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gssluqbzy.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/ghcachwbp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsrlhlhwt.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gjnbejpnz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gghbhmxth.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gyumozwsj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gejiotbmi.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gbgvhrgvm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdmpbjrba.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gcdxiniik.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gyckoimgr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gbteitawj.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gskzwkwqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gkjnqetxa.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gcdbzxqfv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gwvwfpptj.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gbtrtmxmo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gqjudljoj.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/getlijckj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaxtaqhvu.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gzzlachvp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/glwbmkqzz.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gfhszwrpe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbhbxescj.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ghsmdvgyi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gniviegfz.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gqzcsutfo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpyhujeqn.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gjhtbchac.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gzzrtagtb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/ggjgmvnqo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gzednodzb.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/grffgvqqf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gbzcdfmvg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/ghenkwmvt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/ggxgmqnih.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gzrclbeuz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gytjoqxfp.sHtML


<!-- 参考信息 -->