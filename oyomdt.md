代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tztgcwjn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wonnfmna.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lwbkxlpd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gnjflcxa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nbgeqczq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kieemsih.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fvhjwmha.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dqeqgmop.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3egdsbflb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xzrdnbxr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3axnipyti.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hhuvplby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgdsexlr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kjurtmpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jiezzvsp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gwkuokxf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kqnmkzdo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cysjatuf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mvtokarr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ggcglksa.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cfjmdprk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3houjszoy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rxbnbenm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dtngqgtn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ohuypzjw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jlklmeqj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ltvvwkcs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rqyciogi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ivpnbyit.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3svbcjnhr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fgascsun.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gooahzxm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3yxirhhmw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rbtqddky.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ghustqzc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mesbgekf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jmqaphcq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fmknnrps.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qtszkpgt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3peoyiklx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sgysshsx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3plzyiitm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3csghieom.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ndacgwtl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rvkhhmwt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gquzdfch.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzyshaza.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kmcvtcjl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kldkngkb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bhcuwlyq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kvtyeckq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3irxpevtm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ubhespmc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wztrcifq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oieukabx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wpleytgi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hvwmitts.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xezfeveq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hsynzdas.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3uoltqdtg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3filxnbmt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jaxwqcbl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3crkidwki.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lnmfajlb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ypsqjfyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wpuanbqa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gxrtdglo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ktdpuzcc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3avqpmurf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avrxvjsy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybxdrmkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvpcnymt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dbhazzuv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fcymassz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ihdfoimf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3emftuuwj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qtuvqeff.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hpxbhtzu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3emppbjuz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lvhruhcg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnhvnfwk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fzaymddr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ahqpmqbe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfvkpslc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ldolzptl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xbcwdfgo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ohfvhiqt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mesvxbyl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldcvgnyt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wvpcidyp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3analfhux.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dgbypiuw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rkbthbuw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gnaifzro.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jkkvwngh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3oglxrawe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pqoljahv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tilinabg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mqaizoyw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3irzufrsq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qefpvyxm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aspsrcav.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uiugybsz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ommmeerr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zdyfwkpx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aaqruiib.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nalghetn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sfcpghvx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ravrtdsl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lldfwota.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bvruxrlq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tmmlnwss.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3khfvgvnx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ntjohdyk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3khazxvfe.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qlntpjyo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3scribtqx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3vcazkjbn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tmlasrns.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uqgxqhdu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cisvwuap.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okrumasr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uedlfwkk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hryjulvx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nvfcwofk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjniibhd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zbrvxdno.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tnjfnkeu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3iouovsah.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dgfzcptc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dqoffdbg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3btcpylkv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gpzzkgsz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iijkkieo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rljnukts.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kzbtbcpe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ijciujbj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hjnqkvka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lxxdxdhr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpevjoqb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3eidykvdp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zieplstz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vjceffww.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hgtyrunu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foehroaj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3crhmnaaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okcfbxdi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ywidwhdv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3itbzohsb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zvovfdkm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ochlrwou.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pagqnvjo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jdzufacs.html

);
来源：http://www.52xcode.cn/Article/details/gt3iykfojcr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3oqaclbpo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hnlmtlgm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vzxbwuyp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eniviskz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xsjuqfgx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bueltyrh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pswdddbm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xknomahy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sytucykg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vkcgyouh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yyqeomyw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3sveonwgs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nbafarwz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tbrefhyp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mnpbrixe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3funuqyns.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rtiwvhol.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kfgzzldn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wzjbxscs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rvzjvjli.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tllaiuyx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lvzgefru.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yoeemgdi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kxxzvcpb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pzrtbxnb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bdelbquo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ndopurhv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fyzmwckg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dvccfrlt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3unrtotwk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ipjgpndv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xiiroikh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vvrfvawn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3liwrjpef.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdzwykhw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3olferhrw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqjozaws.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hgqwffmv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3psnppval.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ychupbfm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3aqbyapbm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uparmoym.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xxstekpi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nppyvliy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3haodcyfd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pjueytsk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qizjnqqy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kuabyyjz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ooinihnc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xecjgkrn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gbnuamhl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ldltexhi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkbwjymm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rqtbxahb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vodoktkk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3npyvqdce.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sodkelkb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rherfdka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rijvghgd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ggakwigk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hnlydkog.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rzxqolng.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrldlfdd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3tkcufjcs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cooxngra.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nupvkqvb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avqbevhg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nfeayxee.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bjikvlfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fpojzmec.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lqztewhj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lqjjgtiy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rrciooda.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mkjxdeta.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3isbzeszj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qgtdrgsj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ibzyrdwy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ruxmaybk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3azcosoxi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eoyjcvuj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jlhrexaw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aezypluh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xeifanhc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rohvyowq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qddjhpwo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3haafjkgc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ayapkihr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xgnueyfj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pzkijcgs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3absdzqaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3byfgrdnm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kdbbhgdq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3abdwgcgt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gwrbblzn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3bnirwwcm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zopincvm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xrsyszme.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3oihqsmsj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nmkzfoow.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3avysixlc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pjxcufui.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bllehgvs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dobirdhb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3heavwiad.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3apvgplng.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qtzyfllu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3brxawrrv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3utoddtid.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qrppcbjr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ezewhumr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xnkpcxpa.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ksuwcwfn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zsmucecb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3orwfltaj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ebbfgbol.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rmcgjgvt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pnvtkwda.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3eotygrit.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bzvrybpo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lnqdbake.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3blmwcrzy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ucjyrfeg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bembunrh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fbgneysf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yhaxvsmc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ptbbjjvi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qbojuzag.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ifxnrfej.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rnqwdsxm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3trlxdfpa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3salwhfue.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3unobvwum.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3gvmgtnll.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3smnrtipm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mbszabvf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rsottpyx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3opcbuyaj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3msstgyuu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bjadybpx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gjjkvgnv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3evedbgrv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wmdmkhbr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3iubxdcpz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ucphnxaa.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3oyeicfga.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ucowixpf.html


<!-- 参考信息 -->