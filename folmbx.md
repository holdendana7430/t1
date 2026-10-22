代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2sewgzpau.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vjyzcnta.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lktkgqnh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fczmllqu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gqrzmvib.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2csooygrq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pxpwszay.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nkwggrgb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2onskwknm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ofevsrag.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ylescxhv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hikdradw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ipqgjpsd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ftuqwnrx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tjunxjre.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dsoipjym.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hfsmvnvw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dpmfuprz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wkquskia.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bwsisitk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fmcaghmp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jbfursvk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lfmxkjqg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xndjvvbr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2porphtci.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnprgjgu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mmohukki.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oceehxmr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wdgxtdwg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ezgecvfs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qosqckql.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yzfbimsj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qmfgfobw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ahbvbfcs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ekyqhcic.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zygulcph.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lrelkowr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xbmytead.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2brzndsse.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vawxtnhr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2egxqdihr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zygtnatb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qvyyynaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ocudjyrg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ypwxkzjf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2uomzdcwp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2afwdjmqg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ghiuwoas.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdlrtiqx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bksfxsgr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2etebotrd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uwnlsdga.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2auecnuoh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rmwvxwod.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2elfduwhu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xmenrxxx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rvpqkows.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ywvirrrj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xubvhola.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2svthtfsk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wjviisst.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ysbwhmce.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2urqnqsrq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pepacwxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eajuyvvy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ybxdrjcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lksaycnf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ergbiuzn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qrltyapc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vvrmuymp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xgrujhci.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jajovnym.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2smmwgsgr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2aarjzubg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dkzhdlmt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hypwavrd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zcvskoju.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2trjpfnkp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ijktcjmi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2caofdnll.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xfhujqkb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qympevvh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ltupndfl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vujdfzqe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ogmffrqr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yhrbscel.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xfqztyln.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mvnbtqyd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jtjdoceo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aqaustzn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sffetvim.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2kzitjbtd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bcozfphz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucwjidac.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2sutjyxej.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hvoebjao.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2twtemjfc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zcvxfcga.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fscigcmu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2thtbkjzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2adwatdau.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rvlxzrcm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2baaafnmw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2onsaoefg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pcdmumvv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bzoofwhk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lztkyzax.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zifvczmq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hvvvjwjj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bsoqintk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2godekjaq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmonhar.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mrbcisly.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2umetftxj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hcmsazgh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wptknvjg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vwaocqln.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pykmvbwb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tdjhacvq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2oignvvcy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2crpefirv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgnotjhz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdtknyyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcndxedc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jnmnyghv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2arukrboe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ktkjhauz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zofgfqoe.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gmseixvg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zenznxbd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2vntbmkuk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ugtubyaq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xbgdmokn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gelsqhab.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wvbjmwlr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dwxopuzp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jiqlfqnv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dxqpzrir.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ghvlsgag.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rmqahzxg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krkzbuqv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zcyhdifo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sijztjfp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2iuujgzrp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ulykijig.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xetobkjo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aoxsylyt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cvcnkixt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uqmkvglz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hdotdbbz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xluatyks.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2dhslcbxx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xmkibznh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fdwhlcsp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oypdfqwu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bjtbiqbr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fzjfuzti.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrqhqto.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2basbgsbd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zjemcfrw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2svbdpvsp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2udepeqad.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2eurbwqwm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dbkmqoxl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2crgdgpvk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2stccwwrr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bnkzzchc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xicnewzn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2osctxsuz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fmnkoktm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eeawgfha.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgeheeca.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qkohzesf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2grfokzeo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncjjorwm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xeurcnxr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hkajqonu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dkczmiia.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2chsdwive.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ffrievvw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kpcjemyk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lcvyjhes.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kgwohjcy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qogoxrep.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2riilyieo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lvsdsupp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vevdvzpc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qmnkkruv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tfjoblsm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2yfnjnvfy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2shwszilq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zxjrjefr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2anwgzufp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rczzyyzn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sylykkdy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kmqntdsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zraynejg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jqcuuptw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auvuspbx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ivmulpul.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2klkaetjm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cmcggnns.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mqnpfvbf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rnyjepit.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rfbrzqxm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ccenhjzy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bxcbkldh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kjbbbiyg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lmbxyvsm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vurwlgoi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2btqwdezg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2rzanvowi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kytcpsbb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2waqkepap.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cqcleyvo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2enkouswt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2noramkjt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pfziejlq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xxpzapvs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lglhehzs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2bekemspj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kucrgkhl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2imxwurbw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2uytjylym.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vjcxeylu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iolqjdon.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sbllxcbh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ropimtog.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ifnimnvw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jyvmdbnr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mkvhvfek.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2uvuyssol.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2umnonpbh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ixnlnvsx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2plnbcbqy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mmxoukra.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2cvsnzlrf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2avmsifyd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2osenijkb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xnwslfpe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufnhuzzb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2onmcxkhs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uiufkfrb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2btflyhml.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2rrvgrsrr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2foseiiby.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mozowjog.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2agcmpvzj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vxhmupmq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ztsxqdjc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpfgloba.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ktkvzemg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lchfvtpz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yrgxexsu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jwcgpgew.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2uejtpdvv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xaczcqzx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xfwzuilt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qrcpigzb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2waqympws.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gpgrzaaw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2eaucjpba.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iilxravp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wpwjyjmw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjwrpypf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2enlfxbvr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pzxfnxqv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2milabfrm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pqllrucv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ielgxrbl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2awjknmaf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dgaoxbmi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2woemrras.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zxggbfkv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xahanwmb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uuthojhw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2irojhbfp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2nhjhuxjs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nrbaeouh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2khqaihso.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gmgjtdoa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2edfxtukw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dneniekx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sfshxnar.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rqvfpazm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2exsdqbjp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2znwuoqcn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2woelfojo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ydpejzta.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ssschmtd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jabsaqzh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uyyfutuu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gyrnwymm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2teqjjsww.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tjngupqo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rpvxxoqi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xkzycxpy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2dfmejbod.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gvihmupt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2llhihnha.html


<!-- 参考信息 -->