代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jtocrnne.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xslluuvr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oriebrce.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2axlzxrbn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bohmaaek.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qwadzsbx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mawggqdp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2locywzld.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bzjjvjfh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yavcspng.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mwdrqkib.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ecyhwabc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dxlexorl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2shswcczy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ircanhty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2athxzfir.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2chdmxoev.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yhwstmsd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2inkkdnas.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ybhsmeby.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2krddjuge.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ldgtgtwc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2koihwbtc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hcotprxj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qocxvoih.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xnfnghug.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycwyxnfd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2iacyeqrg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xdvsihjy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2snavagte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rhdiyjje.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hnmexzzw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mpxdgqwj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fwlgfwuz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lhytmqum.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2btluvmkw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ytodxbqe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pvfiioro.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2awotwmad.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xxuhvvva.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mushavcj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cygsccfh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2muybtnll.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2foigbxsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sthmykyo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2yvpkmoju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uaoreghx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jswagnmk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fgrxxtab.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifbubmgb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ezhekojg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jgcpqjak.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2awbxftth.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gggtinkg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2nktxrucz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2dusbhfsh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wrcgchjm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vomwtgmd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cfwvxtjl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jglnvnxs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2flacomsw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hnsjpdgt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2txdhhxkq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vpmmvnrq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rhgnpjgn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jjkwfidh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uahknbic.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2roeurgjc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2edbprrjz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hnucbpty.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ouxrfjhe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ctrmtdvo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zknbazhp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2shgetnne.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vkywphbr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hifovzll.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qnjfkwuz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gerhraec.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gekcralz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xyuqnxni.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lqxmiryq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2gucbyoxg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyxfxewo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bgfyuuzi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2itiiplbt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2wvfptmdm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dwdhacwq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lqerkmdo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xlusvdyo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vbjmgbov.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ycscuqul.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cnokfane.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fwhbelxe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mbkcrdog.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mojjrcrn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2omgztxvm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fnhvlpki.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lfdifgbd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cmgzxsqi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2icxlnwmy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2utsgdwxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcgthfgm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2iygqjeja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhniklhi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2astnzxpu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2oydjpgjh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gjckqiqr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gwkmxgyx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zrrsyhwt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2anggwqkm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oerxxlsh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mmelprpm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gykddcdo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hgpxqrfo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ygmspjke.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dkrqkmlv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2cxrigqsr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fjjkhexm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tfwkcenz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2syukboqi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbuwpncl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zsnuhylt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2accbqjea.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bngdczns.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2oyzkkwan.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2goxiiyqj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uswvkxgr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vhuauhrg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bqrbeomm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2unprolgc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ztsmbrmd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2asbfhitd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2eocsvffi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2auzmoarg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tzngjvvo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wtwuowqy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hkbpgvhy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2djmmypzd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ouowcubd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2slgxthqm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jhaldhmk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ixryrttf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2dmrdxvhg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xpozyter.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlgotsr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fylgwajo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2alkwxswi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yghkodpn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jpuomwiz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fsfeepuq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ldqykkpn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igfbmdjq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tqscqumz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlosazgf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2woiqskzy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2shoeykwf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uuvmnlcs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2pfykbdsy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2njluflrs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lmvfrper.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dpktmdtw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oipnwpjq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2brinikzo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfnhdwsl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2iqccvilm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lpkimbam.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iszlfnwx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pzytpnct.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fhqbfcco.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jsjvosdc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zxhwerbx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jupmmqxp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2inwyxqde.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xycxtiqx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2eojkivxy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gkhmogvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fziucgtp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2leygnbak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtyyngta.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2eojcmipo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2icuprftl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nxfhexik.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ylfhrgdf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2yvfctdfv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vwvenarz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cdeoafnu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dkianndy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2abzxboqb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nbycnybu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2prrrusfq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kvkzefof.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lqvfyqpj.html

);
来源：http://www.52xcode.cn/Article/details/gt2aiolbkzu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yqryccxk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kesjkhfl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2uadmpxyr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vxipojsd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vcwnkoss.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2towbduxh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qomrxryf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mwkemarw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2gydvzoog.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ebhzwfmh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bqpxvfqa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rrylzwho.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tmftsrnp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bdvjwjyh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uwurgdfh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dpiixqch.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2twvbjdjk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dhfqhzon.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ukurcrnf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wjovlyjo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pqmwcufi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zllvcihs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rbcwdbgc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kayjhvqw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wwwkknep.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kgaffpys.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ppnikvrt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jhddurxt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lgcuczmd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xqrhnwxk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ijqokmnb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2spumygdu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lzijycjq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2iiqmwrom.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dnbdwpfu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2phptpfze.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2eaeaylaq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2blniohhq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qfzvfevp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mfyzcsds.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kbbwjnlg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mfxpqwft.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jwbbffmn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2dygvhixo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wmelpkqk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpncdfjz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dswkutla.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lbxaqgpw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2btqwkcqj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfdypxqc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qycezufm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eoshujqd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sdfhfabf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zwkdndlw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2avcaiqlv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdeeectk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pxfioedt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aeudrjor.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2cwlvmijd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cslgnnqx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pfjvzzev.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tzqrhqiy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nflywefv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2utvrbmxn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfoupsn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xmtcvcdr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dqpfforu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2toglhitr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2macvvniv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xttwvbnh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uiabpffm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eufjjruy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gtbqaqzx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dpyfgqyx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bvtiffnu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nrynpiyz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ykzjewvq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2aboecmdk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2knteqdui.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rnjbtpjm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jafjwcbi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2shbapyja.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xzaaxgia.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2neywqcmz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2tjzchbth.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rqtwpssx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cenejxfv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gnnuiywc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jmzkybjb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2shgujomo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2umamwhpv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ndtjpwdu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yxqaymcy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2beyldzgb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vbnyatof.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cahdlycs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mkcfcyan.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ubphnslm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vnqxfjfr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ozusnlcb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2kvqzpcds.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gtwmlfdv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xyycigbz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cttedpas.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jjrxozoa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vizaadot.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2osibymhg.html


<!-- 参考信息 -->