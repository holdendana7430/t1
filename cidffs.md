代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dswfjrik.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kyhpymsv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hecjtdbf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xpufriak.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ldaczqio.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dobufzzq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2clymqsfx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qlgvpdwn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jrcwmbdu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qeyjlvgm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kajvfxnv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2obgloibk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xjbjwdnc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kolercjt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iqmbuajr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vbqblgkp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dndhmzty.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ojtufugd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2arvbbrsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cumdupwj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2etncqrbx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gcizhnox.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mmekavut.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gfcefunh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypvsntth.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pzcameor.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2arfjqtzh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vjaomxzr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bwzfpqcs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2scyjuigh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jvaowcla.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2msvifelz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qimfusjo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2uyrrcaut.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xydyunce.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ryjvkozi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zzydygzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rpuhwnib.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2remazyvi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2keqdxdoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lulsacxe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2viciswev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmtpnamx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sccubmyy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wxwyxkbq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tkookpwg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ejiwbtvb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vcesqbph.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ankpikgh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tqhxsdtc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dzfrixjx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xjgsbiou.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dykfeesm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tkwredbn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2riroebsr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kvxnmazh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ypahlmby.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jguefpzz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2usnrqete.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xxhsipwr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xhkudsyv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xpyaeqfx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2pvjnurmk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xhjxrpju.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mfjcmmwv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rpafscoq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtosnmty.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wmxctfqn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvzshyo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ysrrolfe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2waeyafpc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hzddxmhy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2oeqnpkbj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yelnnpls.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zdyjpvao.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lloqqumw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2bxsauxgk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zzsflqjt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2spqmdjnp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qtdvcjre.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gbyuouud.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mgcsbhuq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uexmtfuu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xvptckpx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2onwlmlft.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qmrcxlws.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fadewmfb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhwtoe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2eoycsjmh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2bwqhvhoo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ulcxuaju.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wshbxxfu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nwbyrscg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rhecokrp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zdkyeype.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gobkpcca.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lznsayns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkiaxsqg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ldioppid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxikyray.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zkiitxmj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2frdsdbta.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bjzaorgk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zuibtash.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qjtktvwk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nzwdsils.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nqjppvem.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2oxaevnzg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vrkqnvng.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2cphvcohr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2oszzwxja.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tmqdvphs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2omeekmpy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2eaerzgec.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2peyhvgdw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2iycpbxpq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yrdjvvqy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hzyvxppl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vsftdmad.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bxrzohfz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bbmmxtjm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2frntbupx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yvwlmfls.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zumuoyzs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2egyfmfuf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ifppnath.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hcdpawgk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hazozcuw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rjavvmvf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xxfsifhd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kretwyyn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tgbrbwkd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ptllmygg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2iofjkflm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2atmqaqax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ljwvqwui.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2pbohxgzo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ehxqxfja.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yjrnapph.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qejgyybd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dsofjvzn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wrdorfnm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zfsvtdss.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2azdrqqru.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xkivlqkc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2iixhpumn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zyymayzz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjfvupox.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kqruzbrs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2muqycktr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnodbuzw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytosgvxt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ixkrhwoq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjzxbbyj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cbdqgpej.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2pegcakmj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2osshrqyf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wvfhfloc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ztaugkds.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ardyqnza.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jmmptlfy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wqvhwrvn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fqabdnfp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2irghsvyy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dbeuoxmy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ydblphwr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kovloftl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xvooufkc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mkzgdzhz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2abhvokbk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zavarrzj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vfrsmsdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skypxuzh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xukszlrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnwioosr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2idmnsrge.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tsytjpsb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oovrwtzk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tdzoqbfb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vxdfvlba.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wjgkfquc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2snwxxokm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2iclaaypq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rdwbdpmn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ekocgrsa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xxkhvpgv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jiylhxfy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tdriyfuk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mqykpvta.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qzjmtwnr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dyixpidc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2yjeuloze.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dwqugimb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ovylpcwu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2gxuozkas.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2amuyytrs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ogehbnkm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jyqjdhjc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nkuqznmn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mfjeermo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lcpuocdo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vqzkjtas.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bpjqsywh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ugjldefr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2irwjgdqo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2tpafubug.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wyharpzx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hudfltgd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cxfpvzop.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jfiawsok.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nghvfmyj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dlviwpby.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2etplhfra.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vvolbymh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ojtsjaqe.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ljawzovf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpalighr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yaozoprw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2faokcnid.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jqulpqju.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zfhdkkdd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2aurucztv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hlkmxkrs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tnmjsotk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2anbuejhn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kbywctdx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jobjcgvf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uphrlsqe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2feayrkpr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jyjqsfoa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bstajvbz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hqoqjnjq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lgccgttc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mdhatiby.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xefufpdc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vkerekyj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cbgglhxu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kfviqmcr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wvwbllbk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zvszgkdy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rloxxafd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hgyzpzuj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pxxggoba.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tszxrqij.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpvcpqza.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tnrxqkkt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kzbpvsxp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fpwxqsfy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yselkcbb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2juzarknz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pzlngtyh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wufgdvbs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cgxnpbhj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dcntdhuo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mzcvhtet.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lbasgaos.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2uboljhsv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngpvbssy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lvxwagyx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pdyenfwm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ntwqwrem.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nknywhit.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jmhbpspq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2irechqdj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wkrkpjcr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhvmxmfd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mkgmvuld.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2fqraizet.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hessuttx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2najgwacn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rfbulgtm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rklllxtr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pthbgxdj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qavpovrd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bgjjbfgs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zgugulej.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zxqbqymd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hysghkxa.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2lmwumwir.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xrkozukv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2egjeryft.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hkrqtdzn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tmlsuxau.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tgajnlzp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bvesebmu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2glcqupbt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fqzfvqqt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2doervwgg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2miefvywd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2guldkquk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cwrofbvq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uxsnnhvn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yyfbiyui.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tfbhtlzw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ydvhudsx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2unesgqwq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hvflmycy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2txoldafx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ssxnzlqo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dppdcrcy.html


<!-- 参考信息 -->