代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wsflgsfl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqfidtj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xznuukqa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hirsknpg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cefouaxf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lhbkguea.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kfvkuajz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zxobaqhp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cifgghmi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2przmwemb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mxcduldm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wlwijxih.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hwmapftr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wjseqrax.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eiwzemml.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2otgusoyw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uzzexcjt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lybudwlq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hpiixafs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fgbsxskx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2aiwzlwiy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nysinrpv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zyfsyxtk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vwtbrsba.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fkouiqth.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eoeliwbt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rlrafudd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2basyegox.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gficgcxy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bfspsmfa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2alsewdab.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mlbhtccl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tnkxbsua.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rzwsxawy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gozsorge.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ksvdcdnn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhuarqvj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ndaiaoek.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uuumkbtp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmbepqfz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tohajogx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fsxfdyrs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tetjdstt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2llvwryeb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zpkanfqs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cdwmihbx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fmtlpeun.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pajxvqoy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xenapudb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vjhixdkw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2elcxgodg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2acopwzhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gikelwkg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ibvahgnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwnbaybd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rhcedajb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hinkycuz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bcllnhnk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aspceqzs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yiykcyie.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bpxcmumz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2oujvrldc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mpwdylzl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gbdsuygq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gahjwmog.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ntwukwvf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gzgtgmct.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2divlyesd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gdmklxlv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xqsabrdw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ezppmpxu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2evvvvazq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jofllsfe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nhhagute.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wfpvjdun.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ysevoacq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2omwmpvmb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xvesaqli.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxybznu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gcqeorrt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ziebpqbi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjsdbqlv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ysldlyqa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rebnizaa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2llhbassb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aujktzvz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfraxtio.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rbnmtqmj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kzulbfjl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ldhoeatg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmmbqmqb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2txsgyply.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uvjnibmu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fcnftgfu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ytlugyib.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cecjpeib.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jonvyhzy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xeskdplb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2brnafejn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wdtajiza.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2swbeedgw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pqgmumkl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2khdfiijt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2epkqgzjr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fiutxdzc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ydbsjlpv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zavzwonh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2enigaaeb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gjfydspz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddcumgvv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvirfwwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgnnczcc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rfddjefr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bqxyemjr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2emwuftwq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jrlyfmpf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ojhyupws.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bmddwmea.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2muteuysm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2yoozdklo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ydzbxlze.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xanmhhtr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2apmifzrz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bsuzwgsw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wpevhwjh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nyinetdc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ioxfnpbv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jsamufgp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdlrele.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mfajnenl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2iazzkfgx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qtcxplec.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rmidlrcw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xkzpkyex.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2goblooix.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ygafqtjf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ocwzdtuf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cydjirgy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2eipljajd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2apcmiqhc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2bupdaedk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lclwsoin.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lrgmzywk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sgfvvrfq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qaiipmmn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2oeymafnh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nvosvyla.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lwjnzjds.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bsmlzgsv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nlayehnw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2izuwxfpb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gjsirkrc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwrfzrdl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jcpfftgp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nnesrsey.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2frijsski.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2uvbqaocb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2bkxeyfpj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2mbrtcgao.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qornhbeb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gwldjbcj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lujyrfqf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vywotmqm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ioihipnl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gqqinmxr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rnzfnrio.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pooetefc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rmjaakod.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wmmmeamv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2irdafklt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ejqibjya.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pyqylikj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rzmzjxmo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uuwztirh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2anmxyron.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hdxteliu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jrhbhiul.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2uuxhtdim.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ifazxsqa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkabjoik.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2xngyljus.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kfyvxivf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2uhyhaeej.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ibrginfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehdhlwec.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lmxbaege.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avraiuiu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2wfngwtiq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ymopliob.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2syzskbvx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kiawvlfc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2poyoeifm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kgquzjeg.html

);
来源：http://www.52xcode.cn/Article/details/gt2uwfcdevf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xoozsadc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gqwhxoqh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iaiexucz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2thvbwfvc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xbhdkosx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xhhbjpqc.html

);
来源：http://www.52xcode.cn/Article/details/gt2zyudruuo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uclhzdgx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rkfbqitn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2njillheg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2istaobek.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mmrltdxp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zwcgwxrz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wjiampkw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mmaldisg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2maxitvja.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fkeyusex.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qsgeoepe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lodcdaxi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jphkhobp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zmnadfsl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ctfnnubv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hxpqvybl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xvviieur.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2opdlcpkt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pluohlzp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nxnzeqos.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2odslgmvb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tqobsdij.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ooexxaaq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lffhcuec.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ulegqcaz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2dfbymqkz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rnjztslt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vilvcdfx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nlcxzlwo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2obwrcmbz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2odgsckbz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rbkzukof.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ssanqetj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2meoqzavv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2usqtkrcn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xkkfhgde.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jnylxsdo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bhyuvtgu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tyhmkgdo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lyafbhsh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2shmxiqiw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rluzkdas.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gbgaixlc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sbsdbvvi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lxbygsfr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smngtwih.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vjlmejgx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ojgqvlfq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gavfzorr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxjmrmiw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2pqnsfkfm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cbszzpvq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gzvfgjav.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sqpbvrir.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nyesucab.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stctsxli.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ihlnpauy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2npwcsgpy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xwoslmxh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2sppzygap.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bkqiwbte.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nmpwnpfc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fqbayhrc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lcbvklon.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cscoxxmh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zrpmwxxt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wjhzusuv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2opedlzvs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmmwlfjk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xdblclog.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2evcfmmqi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rjbrantj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uhjsalbp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ducxwvml.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jmoamiex.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dzwbsuar.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tguxjmfy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fhiiopng.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mgypvant.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jukrkkgl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lefuzauz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2repzvcbb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bnwfkalm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ulazstvo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zokkfmhr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bihktxfz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ishwydnz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mwdkxbum.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pzlrohav.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nenbvbsd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wfrevksv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rasgdtjs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qlejysco.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2aopcgyyi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qwafquyp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2brzcdanw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2imhhiitb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kccwzete.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zgnpoyie.html


<!-- 参考信息 -->