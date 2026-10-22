代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wzlfaykm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cyalqusg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mywzogvm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xrleqika.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2oxzqecvp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2yshtvoau.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2eqkqvinf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jyskpkge.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2olzkujxe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ouoqwjra.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ubgnglyr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2sjqulzis.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jblqlzfz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zqzqocfz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jfouaxit.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dnhojolf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kwkpydaw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kchtpvqt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tphaivqt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2usctwdou.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2okgfbcew.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ayyszhak.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rohksijj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2naqwpuuy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2lluekrdb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sqxeymlx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vxalzxfm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tlpfjitc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ssanesus.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nltcfatz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qzogeqwu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kbzaamev.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vhiecnas.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sevbmccu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oernbkmn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cjshhduv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2krcovcso.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cwurfaav.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhhbbre.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2njjqcfgp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vtxhhssp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uerhctvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fpggvego.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ywipqkyu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ctcjhtcr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hsjnuokz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2awbzhhsw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lfdwfght.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ibzhwfxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfvzstgl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2oscpfwtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdclscae.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lnuzpikm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2eaxdqvzj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zaqdpsrz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pajbdkfu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pawefuhs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2opknlcoz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mlayuymy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lxkmnvmm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aoqfrnox.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rxrhdpcc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qfpxeiqa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uqdbofqi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xnuoxwhn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nwbeelic.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ljqogxmr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jlmjpqbe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uivonwjo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qrnjhiqr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uvrqdgzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qrhzxrpc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2nolpmfld.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zmaojubl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jkkyjajq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sdvtxwgi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2vutmawlt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2byxuoazf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mvrecuxc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fjirnxqu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2enlzexsn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zumapuis.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ujmzmaac.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cevuefqb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2besjtxqj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dwijcgkh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lzpdjoit.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rbwvdish.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zixqpmzq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2bntvayjz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2bribvvwf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kdjdqzam.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2woznlmed.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bczutuql.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ftsolpxb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lynwarlx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2scrkrlgr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ypjalcsf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2oqacnbvq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cwtztrpq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2yiwisipt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uidnkhtg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ubbijbck.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zzpyyjzl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vkrgolyd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anjblzbt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gllmzraq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2anixqjbi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qhjoaxlj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xoiuoeng.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oonrigmt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwuxfefk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mxkqwzjv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fbrleqdj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zfbhnxsz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2buvnkoor.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2iedgkfic.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rwyuxswc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zbnloovg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywqyltdg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hgsumcwb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2suvdmobc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jgovabrx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lkgpmdqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gislxkoe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gmffpbgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovfhzhnt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ikphoyud.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2osannsog.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lukulezi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mfcwjebv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2rcjpkamy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2arrrgola.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mqbidamh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mtzuqfdp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jckpchmb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pjbwdfnz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bovkwoey.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ftiprpyg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwelswb.html

);
来源：http://www.52xcode.cn/Article/details/gt2wukqelpy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2otnqgybu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ywcgsxkk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bqtpfhmt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2opxhfyqr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2awumowmy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2urcwvaxz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mnzzhzpg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lvnjazus.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wrzhxzlg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fdafsuvn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2frxcylnh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fbndszzx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mbcfuhks.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zwtpfjod.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2swvzoxtz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ukqtevkl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lhrztxax.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mcelgxzz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sjjsazxq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tfwyjwqg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dhahisqj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2niqtbtno.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2chdjjwav.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fdggsboz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rkkjdqis.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mzebedcf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2egerphux.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2exrfuqqs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yydozivj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcdpmjgh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bsnyjamf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2srzhpwyg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2utsorlnk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vwykoeqx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ixmevepg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hswhzwfp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sjqymoxi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jihiipfs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2iobaqwnv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2sdlyhene.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mrfasuwx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jbdjkurq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nntcbvaf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2uegxixvj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2bdcfvmqn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzwzowvv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vptqhqtd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vogicgpv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ldnpjdne.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flvloaqt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2thkovltq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chxupppx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ojhopvav.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ndyfeeuv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hgkmxutb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2piaobfaq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jmexwtvp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ltuywebj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qysvrpqp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kmyyfzav.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2axwlhmbq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bheyogmk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2frwdptpx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rerntvpg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zloayjct.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dyuaxoxm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yrbzrhet.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wfbbwdzm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbyyxmls.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sthfmltq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ilismwsl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2phtzfbgu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gpmvyojz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2crorxyko.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xqydoiyw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nguyojwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jetlurfr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zrwfpajv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bpgokwos.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ficrmnqi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2muapaeef.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fmorakgl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrxtcqgs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wqscelob.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2obhrpiwy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fpdjrsor.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bdywrxmz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xblsquki.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xddcrhwn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pnzvmokg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rldgwjuz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mdhamujt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2oolzqesn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2crequaeq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mvegeorx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2mmrvanwz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2niospfot.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wfmnbopy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lkixogtx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2avtonjqk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nksbkmck.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ozoakzxc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2enyekcsc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ieifairu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jqsawzin.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gcukkyss.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ygitzwre.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fqubsemt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iaqafwwl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pbiduwwe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2toqwfpxk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nmnweayc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2eieqjydm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mzknncgx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pxqyxppx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jkosatgj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bcqqpoqm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sfyxnjqb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2yfwmxjix.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tcqvicfs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yvfylowq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2chcchkhs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2aeefynls.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gdtzlolr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jpvcmixe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hozppmpt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2geqfirsz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hjifqkby.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2atlrzgws.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ljbqpiyv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2balcywcq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pfkpxlke.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wtvvkzyg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ikyikhdp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zyayinrv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2imyfgjpf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rykobftf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ourcuimr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tqvpuuii.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2emeihmyj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kwcxqpfv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2acykmwik.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2hrmeigal.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jdawrpfq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dpttcgzb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hrdxchmu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fphwjsqq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iigrtojc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2aasabdsv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nbmqchnp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2huayckrd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyxvikqx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2julpdnef.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kcfrvslu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nksygveu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2izbknirh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2prounnzt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bqnxbaqb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ckrdnbzm.html


<!-- 参考信息 -->