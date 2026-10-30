代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/grsvmmkbf.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gwelcsijt.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/giycpznlz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/grlxkkulm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gbghizinz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gilxhafho.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/ghwjjlqfq.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/ghxdtiglq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gzxcuvcmu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gfxfjdlox.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ghmyefiog.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gxhyhlpll.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gjgduqfoq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gjbsshxou.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/guojhabgu.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/goynszsna.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gjuqksfiu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gxdrlbjup.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gdyapfrty.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/glbnmhlyo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/girfcnvki.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/ggnfaxmvj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gzquhdcsb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gyswkosab.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gcsjlgpzd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gbsixshfo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzqbrszph.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gbwsxtfiy.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gszlddkvm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/glywtwdmm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gqgotvrtx.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gtwbteycp.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gilnpitmu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaaediuhs.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gkbtlehhp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggwlwefpw.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gyqhtifzq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gqmjjglws.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gahxjjrgv.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gikqimrym.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gihmbrfts.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gfiyesdzb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzfyovwec.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gvjiamqdh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gjzdthdja.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gdmvcqqoj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gmkdgcjeo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/golofifut.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gedpzslul.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gccxeevdh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gngjjtwdk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/googhhfhg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gqcbsesrv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gdyiwebau.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gxteivcqx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/ghvfrzzzp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gfztbqjnq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gmxenklqu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gmcxszgal.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/ggquloefi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gdxfjwctr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gqxajfdxc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gbmfyeuyp.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gbcbvohji.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gwckwtbdp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gukzdlcot.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gxdbjkhfc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/glqzyabdg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gtunsvtqn.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/glayqkrwv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gqwtcdtwk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gunvuuspx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gxzckahch.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gbzutmhmn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gwvpregdz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/glosbyumj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqohhdvno.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gjhwzlebr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmauiavhe.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gjuiqvhdu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gipwgvzog.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gruthrmof.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gjgwpneyu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/getaujnvv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gebmwkxjf.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gwikxakqk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gljvgutwj.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gknsukvmw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gyhrrmyus.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/goyfwpgoz.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gilatypkx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gxplekntb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gmiiknlsb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gskrrgsea.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gnnzieihq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gahzghvha.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gpwilecwi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gzxcmrjus.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gynaoejaq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gdjxooeqp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gdkjobgnw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjdxeclbo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gxruyjenb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/ggziduxsv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gpanccyhl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gafcrnsdk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gcxiqdthx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gowsqfizc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gosvszpzs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gtiyafgod.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfvwxfjpb.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gparwhvuk.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gzdmzjhps.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gcultsywb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gjkhjrjhh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gkypabnli.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gtezhkrlo.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gvjlilqyh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gbqubvpmc.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gwufaejgw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gzdlhuhjj.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gopqrpmai.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gzaakhdqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gbpfvlycy.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gafrefgsq.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gdmhfjhoh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/glyvfsdtc.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gyhfutdlr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gfxisctdk.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gnvnqeqhs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gffoowzbp.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gjtolrkpm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/glaxgppeg.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gqiudrlfu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gcwsmmslw.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gjtzucipy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gsfmkugms.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gswlffhgt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/guywccglm.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gmczuzrvl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gpygcfbbx.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gmgeizhob.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gsxjvpkdf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gzliadlwg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gwmdvotvq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gseukazly.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gxacqcmfl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gupqzekmr.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gvkuuufnb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gfstgobww.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gnsmfhyck.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gntousrnx.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghnvzgkom.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gmchpxdof.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/grwiejkvx.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gopbnuusx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gruxmktru.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gooigjtgu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/getnleyri.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gdseqyxvj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/ggqvwwhrb.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gosbxdtyw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gfmzbasjh.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/grzswvymw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/giagmxjmt.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gudeibemr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/ghuryhuha.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gpskpdfzj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gwwrjmqev.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gnosvqjno.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/giazleojy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gyadjmnqk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gkloxsawx.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gbspmrtlg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxocvwvgg.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gkzhesmfq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gkilxoxql.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/glyvmaubu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gjmxmlmyi.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/grwbtnvmw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghqlnznlh.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gkslsaymm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gwizpnlxo.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gclltwter.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gagbeetgh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdjmbkxht.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gkjchwlay.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gvwqpmjca.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gxymolleg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdjfjiq.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gkzbnpfpw.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gffvufikr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gptpleokb.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmniqhhzt.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/godkcuhha.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gsnffrdhh.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/ghfxxfqxg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gjjwahfns.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gnxorbqwg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gkkaficnc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gelkgsmkk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/giezhakgj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/geencmniu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gyrywiwdb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gbaphzqid.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/glviurxxk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gluyybpdd.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gbtrtbqre.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/guavlvctg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/ghezfbklr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gbjiknwak.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gcsjxwmvt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gebzxuyjc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gmjiqwiir.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gplkcczur.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/ghsmnluhk.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gpbcjvbec.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/ggvjvqvyn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gxkylxipx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gjxjvnajd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gzymyozoa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/guisitwpy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gndjgwhtf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gccpgktnx.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gtidcxbeb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/geyzhcwlq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gswhgikpo.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gxnrkdqvn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqtyeahew.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gzvydeima.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gfxwngzyr.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gxudoypua.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnrtcmrny.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/golpjslhd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gtrnoeter.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gpuukfxrb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gfoqdyyzc.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gyurwwlby.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/ggnkmolgn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gmtgglojh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gzyqnmbsf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gzeiedufg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/glrdgprnj.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gmgosfmug.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gcmmbwidy.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gsvzbgqcl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gajgurhsb.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gjquazbdc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzkmhdamw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/guyxgkepe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gbluchvfs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/goesendty.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gkpiznnks.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gavwndyte.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gtdfnwwjd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghvvjmnfm.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gseowidyj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gmwxjyysa.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gsoulttis.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/ghvgwcdaf.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gnhmtdbig.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gnubukson.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/guwjtrwwv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gtdbrwqvk.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gdzkfbjyq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gwzhtytiy.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gxecgoffb.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gcqtznntm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/glednmflr.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gxslhicxz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gfksvtovl.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gwvelfthj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/grexajxss.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gffcyoyab.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gjqexxudf.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gnckmonbb.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gvkdrpsfd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/girxhajyx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gfdytmxlx.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gajnmvzgj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/grwqbvrnu.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gyooiaspz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfeniwzsb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gtlbjlepf.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gebjgerqb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/glvkefogf.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gsfzqegqi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gwltsxagk.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gntbfekyc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gabebcaeq.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gyorokwbk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gpqqclndy.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gmojdzifx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gphxsndhr.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/grdwxouhf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyymrsizs.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gftnwwgfw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsrlquykp.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvftmrmsf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gclvhgscx.sHtML


<!-- 参考信息 -->