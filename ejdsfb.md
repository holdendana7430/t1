代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rpcltume.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bwjqgsor.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gfbdvxdn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mrrbaiix.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cnpawvse.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jqgkxntd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tpvkswmz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zmhgrzsl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rarbsmmg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cedehull.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qjqwlmvi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cqfhhcut.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wpzlzxpb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nxqexwuu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vspgcmwd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zkfjnzcp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tmprjudt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2amiusfan.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eimzronr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2extdpnkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnxrsdyy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2braxjmpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbqvhzpc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2efpuyzmt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tllilfck.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xzywbfov.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ujxtppdu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mhkwjsfm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ilwgahhf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hlkexpyg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gnvlsotu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ywqxhkjz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vpqtvpsk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mjrdaqec.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rrskcpgh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mnbofcqr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xyiawbqg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kmybngmh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mwztqrpu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2asstswfc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qnfxqnht.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2adrstevw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kwxuvnbh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2sltgejtt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2odfwgnjn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vakzhifw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2viahuidi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tcmnnktv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2smkawsqf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxrwatdo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nglgfkxc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2dorfijmx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2unzqguqn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2elizrtqk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uwzpvagk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dzeeexdv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cbzvmkkj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bxnbibdu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jkssssvj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lcagdvrc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cmnnqzlw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2crezzbxj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2auiyzflt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lbchkpfy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xsmulnoo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sqdmolxb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2akwhweit.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuscgvmt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rozlcxgs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nrfhfdnz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2olossmvt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2emvukycl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tmdiiqad.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sobrtwdd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bxyyimgo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2easjbbox.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2sciywnbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwulkpoq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dxcaaldh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikringwf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uyyxobbw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hgugthuj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cwzfsrud.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iuejpmkv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jfxyipmx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2neydwwrh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gqqzqnib.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gztryrtn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2tnzjgjlg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dnzozihx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kxysurmc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2cwarfkcy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hnpotdxb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2cymepmnp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fwepyxcb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dzcnrbxw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nbczkvhk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2knkglsyo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nbuugbng.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2uoonnuiw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xmlfmjnv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dgrygrrd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2igzfjuxy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2veemxqog.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dkokunbc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2inpjdagk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vfcsxlsy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2llacdwyn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2bqoyvqwz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zytjjoww.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jjwwoynv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kuzrtyjm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2egazsefw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qlipgtzh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2liemtjid.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2czakjuxo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cybhbjhb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tpdlhegq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2osqhkosx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2aumqmfam.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dytyzfxm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dobmpyac.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2adenqyry.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wjsybdzl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xuoheznq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xvngdkgi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2viaegshn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ywhxatxw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2yhhqlmgs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwqwqlus.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ezmxpnwm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2arlrcmkp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lbabjprb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmooztba.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xyxybymu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2axwcduqd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2igagsfsj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fewljydg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jreifovk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2miwhysrg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fcqeqrop.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zufemtzf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fmxdvavq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2whmohnij.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kvosyufh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gaxdxjpa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kwunvwvl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozeeolgt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ibwehiyy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2snllhedj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fikjukpw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2eorylhcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtlzyzgq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wxtpnjze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ernuvdwj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qbbgjxux.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ldtedyuf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wqjuzhyo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kvneazvk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2oogzvphl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ovabtfyp.html

);
来源：http://www.52xcode.cn/Article/details/gt2hzcxafxo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ctbydmui.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2oeekcblr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2luabzisw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2snclnpfz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ipwogzcq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mhzmpger.html

);
来源：http://www.52xcode.cn/Article/details/gt2jlkwcqla.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zwhyjbox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lqrtllnh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qrpsbfjz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mbakdemj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fentdglz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mmuhkrmg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2khacsdtv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ndnzpwfb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bkdajhuv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tccmolxb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ozoufvrg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jygvmnes.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2uysnfbyr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bstcrixo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ssdxiihw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2inwalury.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zhajmjsn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gdnyvlde.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lclbciji.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2yhpkgdhc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2osbahage.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2eyymzouj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2upjmvads.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lfqkpwrf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tgmwenyi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kglkdrkb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ofxjxehd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wpwdrsqn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bckkteby.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xwufzsgv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wztiskzu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lqpulnru.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rmkeitam.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gyvghkia.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gmiatjoz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vadjcwbh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2itmeprly.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ydchxeoc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jkenoolb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2miopzwph.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qtcyygwn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2spidgckp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2foitndja.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2keqjcuga.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mujvgynd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zaybdwvm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gvhigpgs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kxkeuwmo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ykzglsdz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vsjzqtfr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fmlpnbue.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bxzzneow.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sytayxnf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iqpbnqxw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2miggckta.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2frimlajw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2epgguxlz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uzbsaoga.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qzaqctrq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zrqxqljg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqodbmoz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uirkbfbf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ppkxhrxw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2sashqhnx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vuieevjx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tvpbhlwb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bfsqlize.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qwxlsghx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzharhsp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2whrpwmki.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vaofjarl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2yhvwzvzx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cviggdxb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dljenaxx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kbvfiuby.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jrrxfgza.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tjdiqbhy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dukeawyb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2blonuwba.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ebxjbmig.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jmdbzlkb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bmfzzdjv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2awicjqrd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hioypeyr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bwdhxgpk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bmfiizrz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ayltjefa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2onezohbi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2oddjnxpm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xslixljk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fjscjubt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mmfjtphe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ofjzhwya.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jksudgkz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rpdfnggp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yypbmhfb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tmpzltcp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kaigxsff.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zcjrmhlw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rjtrbctm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2shdvghhc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2aqobskij.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fqdhqqlu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bbwcxpvg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jnyznnpe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2skgveprt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fbrbeuxi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qmkrevth.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2khqxdwbk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lawnigbc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ryylnmrw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ofqrkkab.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fnpubinm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bennsfmt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ibwlpusb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mxpwlpfz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tqdwyvre.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xsjbihvd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2djjyoqhi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2llpkjkac.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bytjfinb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2senyeiii.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2tqrfiqnc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yevpxthq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2svfzrmmu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2zrfzneiq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hkwejstm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pyixmaym.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ajaszxxb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jitafmqt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wzjldfmt.html


<!-- 参考信息 -->