代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kwhwjnur.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dsdrmnvk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pdhlxwky.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xiuzqume.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zfymnarc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2raufjkvj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xcongtbi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zxcdxxia.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fyyxxpuq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2svpdthsv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vdnyjnck.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ymuawzlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2acsljclv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeazbfwu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lxvtqsle.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bpemrnen.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2aoozobit.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kpbrswyt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rkkachgs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2efcvpzsp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mbodroul.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bpcvimcx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tawsxcir.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xsfiiayd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2umduboig.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fqfwlvtm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fttnqokc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2znahwrjw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dvzcyzbv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tglybafo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sfbxufhj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sjkagerf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofrmbjjj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2apbcoqfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtezjqkg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ozptdetm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yewrwhrj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2uiehhrnw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vnclacdm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zxkojewp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2efhtuufv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xuhyczwl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ivcsmgov.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xkgtzeta.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rtacoxgy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xyboshty.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ddyqrrjx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vjzpvqdf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yhodwmcl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mcnvymwd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2khuotpbe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jnaqztyt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rdwxqssq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xxvrzkvr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtsplney.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cclxbjph.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ztuhhgqq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uyaoyvbg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2suzrceps.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ciijlxud.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cqympghp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vapltshk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2yuvfohnm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xxbifquv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tsbwtqkg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cplvhvfs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouzvlbkq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2eqhesxum.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qgddkerx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2apempcqm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jpynqzqc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ubuxnyhb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbmshtx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pldwnygg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vsqbxgwe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2svezqlzy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ihqzuefy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lnxueijs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2synponpb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ikslbelv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mfhiwxrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bjayeakc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mswapvll.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2modruiyi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rvyvwhdw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2pjpkbeof.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2uckahbko.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2echnhmtt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wmzagmsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaqbwmyr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jdvgeeob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smnlsszj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ftnucnmc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gwoolpcf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2scyqmuai.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fsiptfaw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hcedjhao.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fleaupjw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ixrccazc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sitlehxm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qiketkyc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hczofwkn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kkbnkbqm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxcawpzm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xnxvypxd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2llghyimd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sanrkyen.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uaqvdams.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hsdvbekb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2egmefmbr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hrngafzv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cxmyxiru.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qmaioueq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nbbbcpah.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ulbucipc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kyayierd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xsleyukz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wfzzugla.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vlyzlsfo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cbmbixac.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2sdkdikxb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dyhvppij.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lxyjwhhd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qklvjixn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2csaqmvae.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ctruwllp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2nwccqwij.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2szyfdbdb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mflbyqih.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2netrueuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fxiydwdz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2javubohc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hqaekzxn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qxwfptpv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2siuggcfj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xlhowrbt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pfwptkmm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ngxyogvs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hqjncooh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dfyyicqh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2oybonyhk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ouaplnhp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vrrslpyk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yrhaxncz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2coquiyjk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qqrhwxzf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2txhjqbcr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2sorfmgny.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ixlnhigs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xorosptv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ouqlhukx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2nlkbbusn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2baxgsqnw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kqvcxczv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zcgxdfga.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vhbhkigs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2cvhneaul.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pqnnuigl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2shtgnxct.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jkaxzzcl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fkfvjamq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jnmhcvct.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zyaaqpnp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ayntdhpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zobnmbwq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wlznldig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oygegtdr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ldunkowg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vfylodzs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mhjdboji.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uknzonmf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yhfxlqjn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2oxramcrl.html

);
来源：http://www.52xcode.cn/Article/details/gt2ickstnlk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2pzqlfguc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2fwksnllm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2aqkyidiz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vxoblhla.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wvtczedz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2clcqsizd.html

);
来源：http://www.52xcode.cn/Article/details/gt2zyakerqd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qtjlqiwo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ltgruspy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qliawidi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mqnygcnh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ohgarmko.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lbslcbae.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vgibczwe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kfxekdgg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lkyyobhu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2kzqdshny.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rrbascis.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2byrhiacm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gyessaji.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fwlypjhw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tpbisqen.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2otvcuwyy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2oxilphyv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yjdlkhsp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jyeztojv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mxqpyyig.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rmkotywy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xdiofvlo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2peztkfdd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vqgqffcg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ftiswvgk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uvuakaku.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zcpcrxrz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhzghnrm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nqlcqpga.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qhbpkfyr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2edejaaim.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ragmykhr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tyxacnto.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ysigncvp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zuzanloh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jqmaochw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2sykbbfep.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eyqesbca.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2eehejtnq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cakibznk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hiymlyna.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ibichgrn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2llzkuwwt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zzkqszfj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mjohfepr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tornqftq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qzzkyoha.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gcvfsbmr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ewrmmauu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iivdajmr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ayejhzvt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rcqvdbll.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uyvbmysy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njvbiiyw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jharubod.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plpgifej.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qqvydtcn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nmihpuqr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2uatjvqja.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2phftxyey.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgaulqdk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2spigzyfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vgfujryg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wlvpqjib.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bnvyskkw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jpavzvkm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hlrscxnl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dpyhediw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2blbzbdnq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hxaaosak.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2igquiyag.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vgmdzuet.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jajfnfjz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2osgatpuq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vsvaudvm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wyiobvhc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uqojxjhf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2rjvclnbq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2obkvlxdn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qtegtlvg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nlcztxzz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zltzqqtu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2pbzkckmn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mmycpsgi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xacynzmm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xawtxago.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jqqaleup.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fcjjfucl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yennoinq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lvxcxnvx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2khhioizy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jlaggohs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cmwtroks.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xqslzsax.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qzrnnkak.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jomfefah.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2txafveoh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2crexafto.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rgxuchvn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nqppyzkw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nwzasqgz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2huisjsdl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2zvqyizjr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uycgzmov.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gqelxifo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sfvamvsg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ybtqwcys.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tvsefxim.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pytfmofv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zvoploef.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fyepacsl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2btasiiym.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jvlevopu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mrcsfapa.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bdddnykq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ekslqjso.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgkhrw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uofrgjxm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2umkzrxit.html


<!-- 参考信息 -->