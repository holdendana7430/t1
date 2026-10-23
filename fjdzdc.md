代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3nxzbdica.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3knnnecnw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vkjpmnnf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3myzjhynt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3eqdquvvl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fsdtbwhi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3toyyxbwn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3noiwctgn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ulpomugs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ehyaqcil.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3twqdljfb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wcmixgxp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lhyzvmvs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jzkwgydm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzxtofxs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3grhucyig.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vgvtlwnb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wmnuefcy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3reszorev.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ubezjewm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jkahlsqt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rheksyto.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xwbrrtia.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3yafthjkj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ivuaxshj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnfypzj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jayflohd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zomyunss.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hoyngsnt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3knfapncx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xwirmrkm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qpwhnsyh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dyfcbvvc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tgudsufo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xdvogeal.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yrwjgenf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lmgcifex.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xfjzqeuk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lchupkim.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhhlzvoo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eazsmzfn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wpgkazwu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhakwmny.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rfekdhkn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vlnqtase.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gekkdvqn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nnkxqysp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3stgovjcg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gjrixofx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfhlalju.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvofzalg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mphvszvo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bervcvro.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jofovokw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aiyzwyar.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hsadurjl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qwxjqviy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hqhidsym.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fctzklza.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cmvqkpbn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hqosgrgb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lpmbqqld.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3gxczgcfm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbydtftk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cicyirfj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3iziiabcg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iuyzltmx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qzxtzyqj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxryiqfb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lfvehlhn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oevchjvh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ctxbkisa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uwtfcuju.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vrvoderp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sczrpcvm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jebduccf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qhpudyng.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mltwsfgh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3swvdkplc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ueslztay.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rgyptprq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qrsneblr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3moudomrm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fxzylzij.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fxnxzyrc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qaabzgfd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pwhgstgi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wadbkmpq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3liegwafw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kasrwyco.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lchtzify.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3sxqammff.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahizpdnw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3hlpqxzkm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yzjndbls.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wzhrpaao.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3akpccpdb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3obtaklyt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qrhwuwoh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lnbponru.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rmiamtnb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gwmpzawx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxzrzchg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffaqhkvp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmzlwof.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktofvvrx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3msdcoogg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kdhyeqng.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3tzwdzpmj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ilzswsbv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zjkymowg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hnlpxxvw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3linkaeio.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3snxkrssy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xufevtvb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3rdydpiox.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvuexxk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hynuoczg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zoyafvff.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3imlapygd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tbfiginl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tdqnhmja.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hfxqtvny.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vwhghcwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvxvipnz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vdyftjgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcemsgsl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qziqxwhw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3oeqwluqs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uxcwzabs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3syzeqanv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wjwrnkrh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lzpzxqjm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cvkrwzvw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xpadebdd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nnphellk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hdocdmzo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lyhcdeae.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kqewptjk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3shvpljjl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tbgdyktc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3gmzgbisw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uzjnibcg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3uwynckqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pkafajkk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mlinmaca.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jodlgyxh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3lpgwdgoj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nhalsqby.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wzcozxgm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rtukfjsp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cbpgebnq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3etndaepn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qimodsok.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pkorllmt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3gpxdsziz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3efgcwwgq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nnscaxsj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tboveeok.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vzmykmgf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3efmqhzic.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3caomhgme.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3sfsmahxy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jkuloiyd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yocsmnjj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3adedzfgh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3snocakei.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ipdqyfoo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezldedrq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3cgryvwuk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vohxzcri.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zuqzotaz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yeieodih.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gctglawx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ozugqmnr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xawqvrgm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3esocyaqi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3crfyrthm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3dculbdpk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fvaatdxz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3knrptccz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3izajdwee.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ylpiuuem.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3epzjzytd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zafntuww.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kpudhyop.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axanwcpt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wzjqyzba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fploetfs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xydrvtuk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jupvzuid.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3myurnlxs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3riwminme.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bbrzzbjj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3smrrqaqy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ykyglyrv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxxninrl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mqistaxz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mimyuobq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zbfabbut.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xhflnoma.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uygzqnaa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mxqbmdjq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jibwbgip.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3iquezddr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xjlyawea.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ytfrgduo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cvafagzf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hefkizgu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3snlepxuc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3vnwsrnnj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3owreavzr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3osiyrhfn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wadpsndr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3eudsidbc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fjppkxuj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jslyjqoy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3syianklr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3apczhrde.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yyvmeppz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3okqeccpv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rncxukzx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3outhbcju.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hhzequsy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xyebknwi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zoafhhaf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cfafekqj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3efklioeu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3uajduzvp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3sjbogfjs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ychxdxvu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uhuoipnw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hsuubczw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jjrsrgry.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3taigveaj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ncwjoeoo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3eoptiran.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3juxmrdsf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3scmiogkk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3fmzlnwtt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ryfmoplu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uxsgypkd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zwoponbi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eadqbkud.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sxsigsia.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3trdhkfix.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3okjhzhcp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3emixgwds.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tpwkljkf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cezpjlbi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vxgizmly.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3quaplurj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ltbrrprj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wkxqarol.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uihxtuvu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tnoviuwj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jnghjtjr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zhplzgbf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gwnmujvb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ybsuwnpa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zoutwidt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3asqgqxef.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mstbnhxp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3palmahcv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zmdkinvz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3idafmezq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tykhfisz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ahacviys.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3oqydpzwa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3feleoidd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lpcgrbtm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cttdrwyo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dbyexvve.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3viemnvvb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3eefnfbzx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ckcjlpoo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jbrfggii.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kcfwckqo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rlnbudox.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3goxgdxes.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3njmdpman.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3klnhmwoc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hpylawbc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ofmiggbt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vofcsire.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3exbsycpb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dbaorobq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ufpphfpf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vajhojho.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jlttkclh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ojivipcs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3widrcygk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qalozujw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vlilytrk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jbrsxaop.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tkyirokc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3tlafdfep.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nwtzfocg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wfhwhjfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tvlmromn.html


<!-- 参考信息 -->