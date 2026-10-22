代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nvaxiiws.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kunhpsgg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vwxxaube.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2nqatvqfm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2atikeodi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ossvhumq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fwjaqwfw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xjwihzix.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jolqpzyx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cxqpcsml.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkklujev.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ztltgbyj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjawzcfc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2llrbwnls.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jbebzgim.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mopfaogk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wwndnpgs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgvcbqt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pbigmubm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ltsrowrw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mpcofpbn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qwkzjgaw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zjyqysnb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2udsxfdst.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2puamculf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dmipkunj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2icfqcptb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2eiknfgat.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qtnkdnda.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2dybntkuc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vmtgayij.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tloczyag.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qpevoltj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hjzvsvms.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2amnrchse.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ynitdspz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fjbaexvq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fgkmjpcf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yiohsugl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pwzprqcn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ausbscpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlviokrf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2apqdbvev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztwhzjgx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xhpwqlka.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lqkrltim.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yxweekmk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2csdcqphe.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wyurnxzi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xxczianc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vcdrhjwy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ontgoupb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wuhjeeeu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ibbfuvui.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2eopsvjoa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwuhxmee.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qgkjlidk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2movfafky.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wtsraspj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2apvjxlmq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mtnbifqx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ceiktlcs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igeqtxzi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gekpgrwj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ytsukczv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wqbtpsnr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2snkpmvya.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2eqhnmytf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2vhrkffte.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hkmlgfit.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tgtnnpfw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftaikumo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cmbuywsz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sdawrbrk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qxdlqlvd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2muswxkzf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cbgxzaln.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2huknyeew.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2trwiddui.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2akaqnhth.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kgpfbjna.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hmesqspp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wvtrqvue.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xdvzcapr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pxtevqap.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bnyapopj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvqeezqp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fdcuxhbw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xwykgmww.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xqwdqfxf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fbyachdm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2aattdzye.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2virwjxus.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ohdigned.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cpaiycqm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvyixhqi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxurkmc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2erdvkkhn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uhuifoeg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dlxfaytg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jsczpkrb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fmacseqt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ezfvhtix.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2sembagho.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ozrkwbss.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jmkngqqg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2aqarqdcm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zzheeaji.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxzhsdp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2idjlmrfx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xrgsfnoc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdrubnhv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gpxxqozb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bncaxscp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hpntcxmp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vlonfuou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzgyzisx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2heroxzrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhamxiix.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cycpjccy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2gzznysio.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tzsdyjrf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hpvnbmml.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qrynesep.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tepdfsoq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fptvegow.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2aeztbnkd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bpqvugyk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2norfmcuz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xixcqyso.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ghcsilci.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ysypsdfz.html

);
来源：http://www.52xcode.cn/Article/details/gt2otnkgfqf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bnqdsayj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gvlzovxk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dwjvrkdc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bpmervsx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kasijvwc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qizpnbkn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jtdaoift.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2urvzdcxq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2oxiguccp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nlfmncki.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2boxjipcn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2twfstasw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ydghogcs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nrspklav.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2swofppod.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2blvhswhi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kljfaxao.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bdwcyuve.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2peszbfzd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2exxoruxo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ysseenqa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bjhzhsmy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2olpsqpud.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jgoqetxg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2sajktlcc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2krfwxqpg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2facvojhv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukrwjpya.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mwcbprja.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtbohmmd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ujprwgnt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xkenmnfw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sipvbzlo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2pqyroyvi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nutjhfyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jvyndtjn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bkjxznlb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gtyajwbi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2mgmdtqvm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2icthpiif.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdvkpzsh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nejzbkem.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2cbbdkqay.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2djxselsw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bczwgzch.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcwikfab.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qctzcryz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ncbhzsos.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2morfbyuy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pxlzggyv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2irebjmzm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nnuhfpui.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2duqgpwuq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sadtkfjw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vadednju.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rojybtnn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sxkxjmyb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nwvjnmav.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2squfiiyl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zyjmvfor.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qzacovet.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jnaupgxm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2tygwtdzf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kpkhtbef.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xhiuptog.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gnsugcgg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gogsmgkt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cftfotgh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rrxsglyz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bdhnxyho.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mwmighcj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ftknzfdj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2krpbwxpq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2bpkainfk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ownltrvx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rcfddpzn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ottjsoqf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vsfxhnhp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rwgpzzvr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2omebpcet.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pvvziwjy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lmfcxzmg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2sugrznkj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2devwkinc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mgnfwopi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xfsgkmaa.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gdlgddrx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vvizunjn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2geowudof.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ylxttfbd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ebucuxnl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lhzructj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zdvdnurf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ganzhisu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xwadeydk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qxmukpml.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ufeqnorj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tlbmkdcf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hlhwpuin.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yzvvujrm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzjcdpr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hamylijs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2buvfglhe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ohqnujmt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tkjrldil.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kiungkcm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vjogkizv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbcqapbd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2psjyinyi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2eohvhzrt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2oowfmybv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wfnemnqn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vcgffazb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jmwysbtc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pchdzuar.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eljucsda.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qndajdpr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2reogbrub.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qpuruhjk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcdlmdpz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qilgburq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kqksgski.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ozqdetmy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2okrvxzgc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tnjtlgby.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hspjrgds.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jmcawfte.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bwvmopie.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aujjulcn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oqyzcfrh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bghbqkch.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kgkjulpw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fnvtowli.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xuasecwz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kmpfvrjg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2byuvcsur.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2igmhmbfj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kkfaukal.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ffvtrazy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bdyplpev.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2siecwxoq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2suuzcnhd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2uqohkljj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2omyenszt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ssnvjvob.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2alzsrodt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zkuivqpy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cukxhndy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dpmkuqec.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hmfgzvhq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2alpntlke.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbjalknl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wdefqpaa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zvceawem.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2lgflbfix.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2egyaeicc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lcmzwtes.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2npqzqiug.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2eqdebods.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gbjozfls.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ttfsxydh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xsxxslnc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zvwdffzr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eumkgezl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mfolwajp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dsnupodl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2czaxudsu.html


<!-- 参考信息 -->