代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mkeuulip.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2sutshpnu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qfwamibm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jxfebrbc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tytcnpkd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qbmjqyvi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ovkezrhc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ngezjuhi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aixqmpjj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wcqzgxzq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zmmniars.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqtbbf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jnrsnpzy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zzxlwyza.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2avscmfbl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2phtglswn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fifatnvz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fcopincj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2edbxsfqe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fpixhhve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvuhdflp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2egrqmfhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmwjittg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2itukzmyf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ltfzbdkd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwogauzi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mhgevmlc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mncaquje.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2upyknfqd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ngpirfmm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2znlogwru.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fcdakuat.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dxmboopg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wawvxivi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fpxbzfam.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2klznvwpv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2evjtlmry.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yzltgqwc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2uimbhsew.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qdnynafp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ouxgbgsk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fpokttsi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sfsembtz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2tlwjfwxc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mhtailew.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gjpdbixv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpfnrpoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hawrnxbm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2kartaqmz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2shmimqtk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zdkdfyze.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kppceltp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2egxbeyre.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjkhicgm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jvbjpvwj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2niqadobj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ekzoyoih.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lwctkcel.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2whmlwudp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mchgdqgl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2eeqysjfj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gaqhanwu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2golmoxrv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2isfqaedm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2iwatflhc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ozdatker.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pniqtaoj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2uijhenvb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ltrdubid.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2tsixptgr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wfubjskh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cqskzgim.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wqagfudn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2askmryyd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wgbngmnc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2eilsskxk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dhxhmjhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nocytaox.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmeenhil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylqehqdy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qftxjeas.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zspelmue.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qseriykx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ppoxayqh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mlqdiodf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jqzczihd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aaqsatuq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2icrbkasy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2omlbzdzo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2lkqmhqdc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dwnldvfj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kgzbxkfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2aqjbsctn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gszzygks.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zjlhtpjv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zpxedjsa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2azoynrkk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qrptwotj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xtfzumec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pufbrgdp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2nxjpvaxh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ukpxhstm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nygrfljx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uabyjvut.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2hjzhhxef.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2eowiqxwj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fyuroftj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kcpfuudd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2kujqfcec.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kxvcmiet.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2snorjftc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pyrubqfl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gacgrekw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rdefioiw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jjrozhtz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yxkvbptl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kxghthga.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tvkxfqcf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pehovbob.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kbsbjkzt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubvwuugp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fcapyxst.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pzjzoeie.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hqtdieoj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rionljog.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dlauslzs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kgfjvisb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eajsykzo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2utdxmcjp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bzkbjtup.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wekovzaa.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fbyolyga.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwlnbxi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2airvzrvh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rzsnyqkn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2nqfuqhws.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vydeofpz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vbdsdozn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aubvfnbm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jzduowuu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tbuhvpsb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xeletxkt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2dlrzrwvf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2enxqhjix.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2umnbtsce.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zmnzzale.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cchigyys.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qbslqdbh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zpzvpkkf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pvuunzwx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2avhxzarw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2btrresme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abbgoqwi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zdsorohk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjimoroh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2egocztcl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wzvseexb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dmwkfmjj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zsiuxjdn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fwzcdwhy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2sjcnvfay.html

);
来源：http://www.52xcode.cn/Article/details/gt2jabiqqio.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2meprtmtx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dbxxoshl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cjbhubir.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yqruqqwu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fsiuommd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zufbhcyv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lghxrtrq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dhtnvbrs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zqggglre.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lwlopceh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ntjtjwml.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ddlcljey.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2looybbwr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ezkmvpxo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2aruxqzos.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2zddhpicl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2skbuofbq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bjjoylgq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2desdlffc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dxgcgrqt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cikbkvvt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ewuqvacv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ugrqmpyb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mbxyyeuu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fjfrylnd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ugevzmrs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pebnvxjr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2dedwctmy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kswjltyj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2goochkna.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hlvzpyer.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vvekwums.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2qjlbjzbe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2elcfrmum.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2krpeshsp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dvpbbors.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilrpioep.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2nsaqrzle.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eqdrnmwc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aoabjous.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rjxvodwt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vpycsxnl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nyfaelhi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cgiodhem.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rewofbnc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lqojuqox.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2afddzods.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2frkehncd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2llgqzjfq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dtaatens.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2blngjhli.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vdtranai.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sguwsyah.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hnfbjrjr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tkedzgpl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bzkxhkgl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twdtbejq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2yeipwnaa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gfoikccl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rdovqixy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fjeaxcjf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2orziajrt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fapxdifi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2cqsdemgv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2krpxwlqn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yfekjqjw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ohalxajp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kvssdzki.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2znpexikm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2smhkactp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ngdcpjjn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ovrrktbi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uopqxxzn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2okqrxrkk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nkzqawpz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2diexsjzc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yhblistz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ccmuenqq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2sapqapvw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2weabkuek.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2joueasxt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yvoqlsey.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qexxthup.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pbczhilp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2opyviyxc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dicqoane.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bnyoqclx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nbubfcvo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nsgdajct.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ljagwgrr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xvmphcnj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lfopdxem.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vtuyvvqb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mblkhrct.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rrlfyxgz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ctawfnbo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ucboouxv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tvxfzkyf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2coekapiu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cfeuwyeg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2clpjedkc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rkcvnioo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nrifocwk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2htwbknyi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ppmzeqgd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dnwdtbox.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yvqpviis.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2smolelkq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2aoiffcgx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wmqobywu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dezpkzpy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2owlmbfbi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pxxxbcyd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qjajtysn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kgxefqiw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2akhmmbzb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mcbgopgw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2enxpurhs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2edkvtejs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xjnrujxr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zllyhbka.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2perlyzgi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2honubxhk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ynedzjva.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vgsgtcaq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ezkhmgkx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xchbdkeu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jntzfrvw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iauslbwc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2aagunkgb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wwcepbmi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wosbtlgd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2eipohcdd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2adoyhpkm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vmreabit.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2taciqjoa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2mnpxxquy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lqjyxkjc.html


<!-- 参考信息 -->