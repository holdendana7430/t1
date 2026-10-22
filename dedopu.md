代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hyhcnvbr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2upohemvi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jkiuobun.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hukyzevc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nyadmfsg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ftoktlyn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yehrluwp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yeokgtea.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnrcirab.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tsqoosbn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2awegfdkc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vdseaotu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2thcitehf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zgmrjetk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qgeiteci.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wtrbcvog.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ifwyhine.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tlmfjlag.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2esbdkdxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uohyazdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kximsrck.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lmiwgoef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usnuuibr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wspyjimj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dhbfgymm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wjdydptj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qqzgoend.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vctzbang.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nanpprhq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2idgjkvwt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vacqkqcj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mshdtimu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yvwekxpk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2twbyulvr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ycqlnbhb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vxmsgmny.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dqwpnxdo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dvnoxbay.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2caxfuixs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qzhnkyoe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rajtpzrw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lyncxuha.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lrmiqbti.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nqnegvsz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bhvzowkm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ftqmiylg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gtqfpzjg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kecpvzms.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ligmjjdj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlsxvzjq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xlqzalhc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2dwqwzvbl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2feixvlrs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wcgqekbd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hegduchz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2grofgeyx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zwuywozq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ubqstrgy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iskpakqj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2udgbbnbd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fwpnrfjr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2npbhzqgg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dphjmkrf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2viybtkia.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2bjnymqpe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2luvvasju.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bhowekcs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2aiujowgw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2icxsdzfs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jtbfcibg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ccwfejdh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vxgjbqle.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wpmzbodc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hlkihwis.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hixvkcgp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jjwyyfat.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2phadspbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihawyvea.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmiixngl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejxfelzy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ewmdggby.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2uvijlsyz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lhoqdxhw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xhpfzgqv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kwnajnts.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ebiedxku.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jhlmjypk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gpiptxrj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ptflnfju.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dtbmdmvb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2phxzwsfy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2csnsbszm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lcxgmsmz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xamhbbgl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bfhhbyrr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mgykovie.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cihbdhrm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bscfbcqs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nsavjfme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2imrtwmgt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2utkopsuv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bjfutaij.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ucyigbmm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdxgbdr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2somaxcsb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ezeqxnzj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vmoxhwni.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qpljmpge.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2umfadcof.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mwvwresl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tjyklvsj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gkxwroew.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bbsoecqc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gqsmosfj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xlccnyig.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tujzgzhy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qcsmmlaf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cqstmtqo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ygthswpr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qzcitgbs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sefgwoxj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lgefzinq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqagmfb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2curhlyhf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2auxvenww.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lyzwtcri.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bidtuneo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pxquyczx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gzjghlhk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbjxkbvq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2imyokzhm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vgdtbacl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ejhbzjci.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2xxhvzseg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hugqzcgq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tpbedpcu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2utqalrev.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gjdojdap.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2imohyhgt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2amvccjct.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lenblpsi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gxypijoh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ecormein.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zckvcadh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqriabw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ochaopiw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2abwxriwd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cakufjho.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dytthmte.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lknlupaj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cvayqtvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2uvtgqcll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spbkgwon.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vifnxyoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdljwddb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cpmrxdgy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2bysgpygj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mjsynzqq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oipcbyms.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tegzubgi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ybiznwyu.html

);
来源：http://www.52xcode.cn/Article/details/gt2wgzeznki.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ixsktxex.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2uuppghvr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kjoeaynx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aysittnp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ceixnxnp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gcexqnec.html

);
来源：http://www.52xcode.cn/Article/details/gt2umhawkkq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qxirkaky.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2udjjheaw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2etghykas.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2oiqzumya.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kogeblux.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2cimgawpy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2auvjjvpj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qslhfbjr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xfafegui.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2rctxcike.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2eixgmtmq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eiprdsaz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2nkdpuksd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2btgpntcw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2aruvnipb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rvukcdms.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vfotphuf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ovyprlna.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2foverere.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2topebmgp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xixphglc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qcljhofn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hqeftbxv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lhtxhotx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ejtqaywa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kagdscfg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rujgocxq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ijndwqtm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cnqrarnu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oddczdvq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2otkmzzrr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2armebapp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hpbrtvki.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zqgzyvaz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xquagrek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2noozciwk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uugqscby.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wrxrquag.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pporlmyi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tjojcgjh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2otkrquzk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hflfcfma.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2uktrrohv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yktrdnzi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2grlecttm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mfskaevd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kqhyyuor.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fintdlkr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xjluotfs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkyxqbhi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ybeixdku.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iwkmibxm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2alhilnap.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mplfnews.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2atgkyobs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ocdipapi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2befltixa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jjbomxus.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wnnjbwlw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jzseuovq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fiyqjjix.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oagwwbvt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mchwylfg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nxsayozs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2aoneaghc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qhofjvbp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2styavkkg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2csmfibff.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqtklzlu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nondyxlj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gykygfhv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2pvcdfblj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zzkelepc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tfuokwiw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2owzttajy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dnshzcex.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2suymmmvw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rpyupdek.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cojullzf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wstgpfzl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2djjfsonh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yrtfqrsi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vhngvrbz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2eaedkode.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lhopnwon.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wpytvemc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wetgbcjg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zmlobial.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zxnhgwny.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xsbxzpzm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gdogsjzj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ypkgyige.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cyriqphc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2llkkwplv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2myahvpbf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fkwrilmb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bmhandzc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yvgzsxtf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vzvzmdzc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ikuuymji.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nzuwgzqr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cixkqedk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ravjcewy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vgldklgq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jdvauagq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rqdgtbyx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2kwgtrdya.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2yattwxon.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2udzigzzs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xzxyqvue.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wohbblvc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bxpqbkbh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ehxcvtxh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ieeeuxbm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cuymjzzc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fcgkacyg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bmlsazwr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fuyvzkqv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gjdkqnts.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jnxuebeo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qctgexkj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ibskpnty.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pkbdkqmd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2riyydnsb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2oztmlnfh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2djxtiosd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hkcakhez.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zukwonae.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ipkxrrvb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rvxlihoq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nawzmqlk.html


<!-- 参考信息 -->