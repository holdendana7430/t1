代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2odfkcaas.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcytuaos.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cnbhlxps.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yyjbcago.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nasijqjf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dnbosvdp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2etjrfxav.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fyeniusl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ivrfzpbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gfiptosn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uzzoixqi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bvcapgtr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jedsjbml.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bqjxaprz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fpzfdlby.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aknmkqcp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdngtry.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vftirpgc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjbmfdfn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ublmwwps.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2siffvaer.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfccxsiy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehueuwbl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2obgbjpbp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajsaicbe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ynrxlyuk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zxyybytf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2azkqwqjc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zpkfcydw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fopetvez.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdnoyfbl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kdztcezi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xuzjjqbc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hgnaqhxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2avmrwbbr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2trnhtxsh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2skbxkfyy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mghbvogd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jgqlpklq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oumdriks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2strffaif.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ddmnxuxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcctjusi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2txfytbfj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tthzodxt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifgoouna.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qcovllsh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wrdecool.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qbmbzuyr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nkaqnfzt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hcvyaqnf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2loplnbpf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yfgyfuup.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yatrrsvn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hyxbwzgv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2veotvgaa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sibqgiqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fmjldbwf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oapeumwe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wwqggdro.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bxarzdel.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qrajqksq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qdcxhswd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gigtcwxo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2iyuuhijb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ovcposze.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ipazpusw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kczqeukg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tijmkzun.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kwwyklzh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tofzccmw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2btqucxwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hccjcaft.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svurumiq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2enbnsdqa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fykxhvjs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zjbobare.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2aatkvfeb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hysztqyy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2akqpuprb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2blpviman.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jhghajpe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2crjzaxbw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sojstyjp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ulemivpx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2leyubwzz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdwubvr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qtjyebgo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pxubwtoi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iooxaykz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2loecnhxa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ujmaztkv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lbbbfngu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fefxnuyh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wwegvzmf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bysxbjfv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tfhqoezx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqfrlrnf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yivjhacq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajytsxln.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ycxfcfck.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zjapsiqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2nmfvsaze.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vyeuleqa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2igjylics.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2taujvxdk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wfbdlksi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2okvtaphq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dnodqwma.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2timnpccp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jfatjfni.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bbmkxmhn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ptiasqab.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ixqmzknc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vnnnhuek.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rbdixdrz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyddbtpv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kinobtef.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zcxvtgcp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pelbyszu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2eqgnozbt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kktotxqa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fegggpfp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mpglptrr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lgngvsom.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jaoslngl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2iogherdr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kixliyir.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dcwvcbbm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gtguynji.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2asppgbxx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jbuylpfu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ywiwjzjy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jnaghlel.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2rawlwlmh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lxevhazp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zisajjnh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2axbgnlcm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xxotikhy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zzrwlvfp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vpnliica.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tqsfkkrk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2banoazzh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mpsfndgk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mjbffmmg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2msjdabqf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qmbrfwak.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cudiogyy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cfqkppfh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmpypmls.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zejwqrwg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufzrtayf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ruhdafuo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wtyyxuqe.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2doieqcrg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2cqwqlkhy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ynxyfmly.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mzsksbdi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tgfxwryn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2veugxetp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yxeoevdd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jsawljma.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wzvtccdk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ubeqrzjm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrdofoe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2uvwxwpwf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jfauwomv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwbangrh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ntejfknv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2iqhfysqv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2emevpnxj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pghqugje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pckbwvsg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qwpwfbnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfrcvior.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vxeodrlc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xopcfoby.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2djgwldve.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tftfmniq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2clzpfsou.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vgtrwxdr.html

);
来源：http://www.52xcode.cn/Article/details/gt2bvypmgow.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mntfzlur.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bzfpmqwt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qhzvrtgc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qfoyjbya.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2iipnasrz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iikwprvs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xlpwyrgn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bhsrebsp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2auivicor.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2whjrjpwb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jwcwwvij.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kkrvifaa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dzwkffbt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ggqxbgvt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2npypgtdl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hdkzitzc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2natqhmaf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2scltdwgo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ahkfqzhj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ptdtpzso.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2btszhgdl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2locpcmdo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nvmunqmi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qfzitujl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ephwlpud.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2djuvqjgw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xveeofld.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2nroquvlx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qrceyqlv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fwafolpi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ijjhotjb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lnouwwrt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2eipidesa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ihvkjjzh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krzkrlfg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2uzcvlgph.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgychkiq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ketiddyk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dgznltyi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mykypgat.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2dricvtyg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2atmoaoae.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cvdvtrst.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nsfaeodf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2avwbcdba.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vyzitfzg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ngalcosp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2gmxwkecl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nbyowflh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2odgmufgu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2laqubsfo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2grscwshu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xmopvqem.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ormqqedm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2veikhrjj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qrdxtikw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xstxhyao.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2eqtcfpdr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndtivede.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2crinpnwi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vhbtdjjf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xcgmfvho.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggobjnoq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mtigtfnj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kdfuithi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2furahwbi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nkvkbhib.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aimafixb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iwoinhtd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vgrrxhxp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hehfrqew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cznzfgzq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mlxkvcto.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xcubnyoq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2evngujnb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vlzrzshb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2clbyzdkn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2paqqwzfi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hakliihz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uebzsjlg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hukhbmft.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pcpntusn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2btebnffw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hlepeokp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2prdalcof.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vbymfmle.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pchrwbiy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wnpkydik.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bbfifrcr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bhswngdo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2idqxjlok.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dzsyjkgn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2didvxosv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wtbpsqwy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gmxzisim.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2plsxcxcg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2inupgojz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vtbdttjk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zkvkszfx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jugxeiis.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2thwqshgh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2axjdyyee.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zdnildug.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uwkekwsu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wccdpvqv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nztczjzm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zofvzvsg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hpnjnysd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dncbucqq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aosfkhft.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zxrlbvyv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2obqrwkba.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hkwvsykx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gddcipcp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2swithaoc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jvkulbbu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tblfdxzc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vetzmjow.html


<!-- 参考信息 -->