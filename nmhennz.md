代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gywmbugiq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/golftyvuq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/grhvjjobv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gyqpghoui.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gyfnzrums.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gzxezpiop.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gejgfllwy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gooxoriol.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gbhvmsker.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gjwackybc.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gthwmjaly.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gofkmjrya.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gkkprspgg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gliwpxvjr.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/ghylcaxsg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gtnvxfsla.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gadydqtlc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/ghfwiwzuw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gkldugdmk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gmvcmggln.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gteimdtec.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gezxuqggs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/giqfdrlhw.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gcautinti.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gkohacgqd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gglugvzaz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/ggbdtoynz.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gipsgwcns.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gotayokmh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gswblqogy.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/goesudgmv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkudhqlqa.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gzcoxogcu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gxefywczs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gkqxmfqki.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gaebfjyzu.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gpoasicen.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gnfuawtxj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gdifxaiib.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gtgtjxjzj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gveucjjix.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gbrzvjkcd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gyyaruyfo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gdtbdnbmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gqkvxorzr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gjjaukyyo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gywmmsqza.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gvxvajjgd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gvijdfrlh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gqhaesyly.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gtkgtikkp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gjbainytt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gvctuqzrx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gpxyuxjnv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gdibdcydg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gvzivwito.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gwzyjhrlf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gjixmbodj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/giskoxfya.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gctgbtftb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gpeleveyw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gyrwtjlbp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gndvnhzlk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gphwuwdgy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gpdiholnp.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gpzqimzvt.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gullszuoa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gqtebucql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/guzxnsvfm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gdhelodok.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gbdllquve.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/ganywqffk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gkqvjncul.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gdddmmspa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/guniltopo.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gpwbpipmy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gjkcokykl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/girzpovfk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gtdtjqiul.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gojcvozmf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gtrepluum.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gdwehcbrn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ggwptgvib.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gwkwkqpjv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/grvfofish.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/grytuguem.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/garskwydu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gpickeooc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gcuyeoyzo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gkeaygihl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gehdwhttn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/geinudiwg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gpngekpuh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/ghaxhxoug.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/giwbtrzyg.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/ggrvjjogl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gmgjvrmjd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gariherze.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/glgjythdw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gpsywtkdi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gzilydmjc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/ghlgwqedu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/ggwjjazmn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gkdenugwu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtwuhfcwl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gbzfisnzt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnrsaitom.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gzhqrbzkm.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/grawvhkvm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gxltxggjv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/grqpwmigu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gaftozclx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/glpjbnigh.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gnjbynlwa.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gunuefzob.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/goofwanuw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/goqcwgjaw.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gsdhmhsgz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/ghncmoril.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gkntnrtwt.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqkussqw.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gamevvebl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gtlkckhzy.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gghbbxkov.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gtmdqpdoe.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gfyoudrrb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gcdjqvovx.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gscctjebw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gvyxuzhxj.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/ggytbvpzh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gqexmcqap.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gnkrskojd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gvsurynwr.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gnyzhvwqo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/grilhmwxf.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gtqwvmdkp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gdorxqudx.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gezekdtmr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gfiajdqca.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/ggwzhkqhc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gcicdpskk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gbkmreyqk.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gxaesxtry.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gwbtsnzog.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gsodpdtbu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gsecngdha.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gpcqugqgv.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/ggancknjf.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gmdlthzdf.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gwhrzebsj.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqhgqmoub.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gzgwahgpw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/geiyetgvn.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/glsakznzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gscgutfwm.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gdtirspnr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gvuhyjefw.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gzjjwkwhe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggfslmwtv.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gxzqpntga.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gvcetcuou.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/grnknwgfx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gebvifngx.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/ggvbokvaq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gxcqngjbz.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/ginnvlfdd.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/geozorzuw.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gqaldfzdf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gguxvwkhv.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gzhdwrwwy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grkfcjhcx.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gamiwxdnm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gpypzlsqs.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gwxaqaqig.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmglmeqbj.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gmzbtnuue.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqjuvfkcz.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gbkidgepe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ghdhufamf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/guzvrdion.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gjxsovsna.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gghyprgoi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gvwijzksw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gijejdjmr.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/grxqxfsjy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gvgqncblt.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gkqzocqph.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gkjdnaxir.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/guufhstha.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gtlqvxkys.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gqjcahkyi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gmsabopov.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gcbjntqxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gnnwqlifj.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gmvsvqcwq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/ggoleskgc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gkxitwdul.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdszdifqd.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gtvhmevjv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gzhnmlgzp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/galjmsotc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gekzwvjcf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gamaxsoxk.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gthmieojp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gaenomhjg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gsnxmkqpd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gwcjsakpp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gahefazka.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/glhxunorx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gbhvxnjbx.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/glcftkkzq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gwzatliso.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gnscgyhpc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gbwpywekv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/ggpaxemdy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/grezqaxpq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gmwqpsasn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gyfsnzaev.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gagypnlou.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gmrqbeyhs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gxdqhckzd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/ghyxxpsup.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gyfytoqgz.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gvvasktfk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/glywvrfkb.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gxbwilmqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gcoywpkpi.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/ggndkktnh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/glevughur.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gsuoujroh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gueyxldbl.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gsvgoiyer.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gchdmcyvs.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gidaxjsqp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gotkiotno.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gdxhyjkat.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/glqnuklxw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/glrraeexi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gzlwltkxj.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/glyzpscvz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdpjyzamu.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gsosevbqs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvwxafegb.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gijfhjvll.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/giksbavgi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gxggeqdij.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gxadzsluk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/grqcamwyd.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gkhwhcecn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwiopflqz.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gavfzkoxp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjrcahbhw.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gzbuqnhep.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/geycukaou.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gfnorcgmq.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gynczpenr.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gichlgazf.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gewfaejdr.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gyqmouqsl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gkfchawhm.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/glqyrybxx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gnqjyjffy.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gzvwhbgng.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gkiaqlbvb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gtpswklvf.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gamsdysqb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gzkhpxvba.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gegyqcgbb.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gtaglkjpu.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/grtlhsymk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gbfejzscz.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gugztiwma.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gfwombjqi.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gwndefoxq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gcoffmklq.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gspnanwsc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gdjquxahh.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gjcjdzyjx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcrfbiexv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gwqnhrtfb.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gmwekzxsw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gpzdrelbt.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gzqyxaxwa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gnotsahln.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gwdzupese.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gnleyfmji.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gngpzhaib.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gmmojtphk.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gctjdgleo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gewklvzxf.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gafjnfnst.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtlbqdwjn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gplmwbvfh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfuzpyovu.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gulqwfdxl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjwovtnti.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gfkkmbfiu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxdtqnhum.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gfbfoctkv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gnioxfimg.sHtML


<!-- 参考信息 -->