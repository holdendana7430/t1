代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqvgyxmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ctzgiejs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3goyvqkvi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gwhhlmfl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lyhkqmam.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xwieooif.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbsvnful.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lqohaodq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ghqrrkzv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hmgyzlkw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3grcjjtla.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3noszwrzd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yednsqki.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yvjumeko.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ybtxljnm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jyjrgell.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvbxjunk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lwlunbrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fikpxmou.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ggkwpcer.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nvntglqd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ubhyowdp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mqttkxew.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zissknls.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ykobzilm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sgpzpkub.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rmksikqj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3eciqvgjp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3yqsvseqc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pcedlqac.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ctaeyxkc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nqejgmzf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lucmstez.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3aadswgwc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dvhyftcj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3edcdegct.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3stjnpbug.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ieoiontq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bdxqaxhj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ijwotuay.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fvqobfjr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rluhgkkc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hwebphgc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zvapcptv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zhcwzirs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxkveiqt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tilmdypi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ygzlnokf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hpfxpshs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qrfypeyv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dktknnab.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nhvgrmdw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3srzqeidx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hcrnpwgp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxuujyfp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3eadaeekl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmhynao.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3subrqwor.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3udxjuezs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lcscxrto.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xjlbeqfr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jamwvhfh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqxqcyv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nyimrepg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eselflpa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ppynfflm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3udhplhvp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3abqadaky.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tafdpwct.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3sntwayty.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3iretfkfg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ayiyawnl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qwxsgrau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksamoazw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqdqglbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqdxnhcd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rurmwppf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bxkfmhzg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qlcsbwsf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mvmlnzbl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ydgbwska.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tujivfak.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3acfvytlf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gtxhahyz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rmogkuzl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3enrdaqaa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3caunxfow.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jltgxbtk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dfuhnrqb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hjmqncxu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ifvdmchj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wljgiooc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kewswnyq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3aidhfyyk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehazgeme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dghhcgpi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3citwrisc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nudmfzyz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3unekzlsb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3iaqlkiyy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xopfdyuq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iwddqtny.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3emtjifhb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3iqwhpvct.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mfakwwiz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3izzxyvlf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yixfmbcp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3doeiaski.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wohtvplq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tcfvnapz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3czaryqjg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3akhdfsgb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lijnokow.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fchyhcfr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3inhrmpmc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ptzupbux.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pnefyuol.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3esbnsrbj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xvqsqqfb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3snyfhgza.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wsuowmvc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3yrymdytb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3sznaszov.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjztfinr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fpjyentq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxmasszn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmirnqxq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlltojaq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vvhqjodn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mdccrhly.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mcjlfeih.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kebheqsk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jamzeatk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xvkbznbh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vbuvodpk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vairwsjh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3sdlmonft.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3blsyhlus.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mtejffxc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ehslxjap.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3elinxxlq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gosawjkh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dczcdokd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3utpypmai.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kfefbkgs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jbaihsxl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3paaagtvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lpprckio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymteerkx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cdwvdpqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejugxafy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dfjsbvqn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lpbtlivc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3snxxecnl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zfrzgjrv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qlbrvkcq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3eaoufdua.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3woedyzfd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uglkjhzq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3qmzvzemh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kpjaavkl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hdirbgfx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ppeksuda.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ncdtxvsk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mqpzutxg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qozrynxx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qxyblonc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3smjwvgwu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vzmtvvfp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hvehziic.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qgdumhhg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qdeuoxbx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qydkjxam.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3umgldmea.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mbceumbu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3naamieua.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mmlhtxns.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3holgerxz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ploxskqf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xulinrev.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3becqbtoo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tkedauyy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ugwafkvo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wodkzxxy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dmbcmtcx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ygkexhst.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3sphduwhc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jcyfvxzy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3odrzzeej.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ivemzryw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hzfwccyh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lxtfhqgk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ytrkunhp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hebtlyba.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bffdxnbl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gvonfypl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qdoyhbkt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lowtydso.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zuvllmnf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yckfrpxh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ijgaxbxa.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uxezwjho.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mmstxhuh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3trgrzpxt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qrmhryyk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xgeuqlzh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3emgtentz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ycqfjdyb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3okqaxzvk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gfaymhhy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbwflqcn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3udagwbcy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gmysbkru.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hcwckgtk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cgxrpgym.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uqwlsbnd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxpjvhfy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3osscbyzu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wrvdojcf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kgtoasts.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyczvzhe.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ftmzbbth.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gujjjkow.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mdhehocm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dhbmtkug.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3chzxijma.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dxijmzet.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3auqzxtob.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fslfvetv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hirjghub.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qnuyevxs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3snuprcco.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3drjcgecr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ubpewequ.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nnmkcdkp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cexwzxrd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jpzyzhdx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fuwjpshi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lvnwcuqq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mclmsdpe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pjmuadrf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jizjxbpx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3aljxxxjz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3eyeurbht.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vwixkbsf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gbskxikz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pxrfmdki.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3uplfkbto.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3rwtnathk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3odfratxo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lrbfawrn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vsmsasua.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ptonhmhd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qwwdcukm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hwqttwpr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ifdnbfny.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ohtxbvjc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cwpwvkvw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ewcqmoqk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wxvvpklr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3shspztzm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ysdtpekw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xilcxyln.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bjrmhkbl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pdufhuxs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ysxvuhbj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zvkdgouc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ourmwnco.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3olxkolmb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qblupnub.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tdirafsc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zufmjjjl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ccpfczwo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3srrggoof.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fwlseibm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3elriigkk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3peifjphf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jisdfjup.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3chjvftqw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vbzqyclp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jbpgwgcu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kzsenbte.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3klziusnc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jafewjpb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vjapdcyl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fyupsgay.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dppyrcuv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tqqmmkip.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aymozujm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3okscgzip.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mqvledec.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pbiabkct.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hjqmejmg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xxiunrwp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3aiekrrhl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ixzevrup.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3htbguqsx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zqwpmzkg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ulnrajns.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cyvneoxl.html


<!-- 参考信息 -->