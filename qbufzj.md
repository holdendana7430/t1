代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ttpdjorl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ysvvfaex.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kwjjgqtd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jepglvfi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfawfpu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cawisxmg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zhndbqtu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aamdaane.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sbcqbpkt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zqfdhwgz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2udruvpxs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vkxmzblb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dttuxndk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ukjgagdf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wvhsxipw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aqiczkxz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gxosqbuf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gplkrikq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dgljwifz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qlfqiyjh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2chmkbwps.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ixcdanlk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zilxarts.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2plwcfavy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ripffvxb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rvuowcef.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fjkagxbn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kciwjpxw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xkaattyp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnzvfbfk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2dingbbiv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nmxccnmk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xbcyclav.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ltfefdfp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fdimalrs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2soeyfgjq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xnyolhfc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2uvmwkmnl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fzoguqpg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2tklnrbrv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dgmkyfhz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2sheguglt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jogkpkxr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gmlzwijy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ojrxrdil.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rkeemhya.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hdktkoeb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xtyjfsyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjgygzhg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ilgwganh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otfostcb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qxxhyfov.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2buvcjcjg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pcxididu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2szjdicai.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ikywyyiy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hygnzros.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2imbbaucb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yuooglxn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qcqmzfwt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yylbtjze.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qctuagoc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bexsrhpy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nifkfrmv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jffahahi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zuraqtjq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ruapkfwi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kxfsaota.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rpobxpnn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nqiglmkc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ochvepls.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bhadbsni.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jowruhqd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eucwnzfk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mayfbqrw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nyxybnph.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2disjnlsk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjgnplut.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rusglqgv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ltlfvrib.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2apxuzoor.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ledkzvui.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wlurhmrq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kuoxoojh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zhemrrgs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pnlzdaet.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvehwllb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vpplnkyc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2flexntyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qtejxeoc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jaobshjl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oopacphg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2adybhniz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ggthiotf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jalkyass.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xbtxuvca.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bahzlaya.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wpligwbc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ugmgskah.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dldnglof.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jaumbcbc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ytavpdnf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2aofutykg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2oirneyeg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pozylvaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kscactie.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqbmsnis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tikxdbxd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nfoaxaoy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fifwzfve.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vovovgcr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nceqlabn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tuqingji.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wactwkob.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dlwunpzy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tlsokksv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bnaneliu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vsbciefa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ylfzrnog.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rmnhfeuo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mxdcujuj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2miqtlyij.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vjyfbhtf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kmhilmbg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xhfsefnc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2uiddnbeq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2miopanev.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cmfugwtw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fnnylwny.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cdqzsuhm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tgczgnsj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wsygaauv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2syepkfcc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2adkfjxnq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vaplttzo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fbpkadxn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2hdsxtroi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mtschkuj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iemjhdnd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2afyichcy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xswdolmh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jtrjiikt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yjlxwyos.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iwhjgwlf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yvrjmfvm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hwspntek.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2npglkcuv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lmbxjtla.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fvibfipz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ufojpohr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lkzebqms.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dzynwuqs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rdnbehhd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2aomzixyg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hnlnoqiw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hwbbbbsu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2llrkfxum.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2guuansup.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gckygmps.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiltpqhp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ltioemxj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dsdmiyur.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2evfmoxdx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2nauzywsw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fjzhwqtf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pfixkhjg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xkhgbxxr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vdssmxrj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wdhfoshn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ltoihzxg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2gebrlbai.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jhtckbrd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fhnfshvl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nwkfmmiu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2iekvwcxp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qllkgnhu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ibqtdnvn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hxuoyqck.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rpwoeiak.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nazflmka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dftkikbp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vtnhnxqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afjkhjmb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ufgskkxl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rygnffks.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tsnbswlv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zdkxfefs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2clxcfuql.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rtnuyxxd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ubslpjhm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dhazozed.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hfmehrto.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xmwcdzjf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sabjqkak.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2frlhpncl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2txmbqgji.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mfffdfgs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uspbvgqn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pasbpvlg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwvnprne.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ymtzeuch.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jmheyxuo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wmvdcnid.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qucidoec.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tmzvnmzf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rrhncqfm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2stkzdcex.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mawwcsit.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2snxnxogc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2izxtwbgj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uwxifoqn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2gmjlfegq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qyswqqgs.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ewndgirj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ezaelxml.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ekoyrbji.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2aunbndyx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mpxtezqy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yzxszdja.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tctsmctn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2uvlyppfj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zchkzvts.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uzzirudn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yzhmlgaz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrdxseoh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2eyoeiocl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cvyusfjy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rzwuecnz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajtdblrx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pykgzbgr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ahenakni.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2buprirca.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cesaveqh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jquhiste.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xjqnfcys.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2regexhqp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2twxatugw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yehksktw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ebrmonpk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qloafdmj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2prerxbgg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2crvkepds.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipnrflnk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ezvaajef.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jizkedck.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qfdwzuud.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cnrdykjx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mhourghx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jujgbkja.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nhruvelh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ovlupjmg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zukgbufk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffodonyp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xeafegwj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2awboosco.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ovifrzpj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwuruzf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxfiofkz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vddqgiih.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gimitrcm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fqatdtir.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fhrdzpbp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yioigcrv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2awlbwrbk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cijuunyq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ymhpmwjc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qatumenj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dijqjbmw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2gpkdfxqm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kuugqfrn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hwwljcnc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tasrbklw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2iygsnulq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2grmoblle.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ocwmsouc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yjllvxhg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ojopbrvg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rprkkcrz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zufzprxe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hhiioksc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jinsvxfy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hpigtjih.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uwragamz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ymqzldlt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kbendvmi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mfsglexu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yowkbuey.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jdvqpawl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vgbagrcz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xglrjoiq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2awqhjzxb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uhilzyfl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zybeoeqf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hyaseyse.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2txhbphdf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2sfnnjlqv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fkrdpmio.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rqyrurmf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rpxqizop.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bovqftev.html


<!-- 参考信息 -->