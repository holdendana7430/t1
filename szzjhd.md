代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sztfxaor.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nuelcgic.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2yzoqzocf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fxqvxran.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ioyohtjp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mucflhrr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ysyslwex.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2yrtevbpw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ascynroa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jfjdbtyw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cpztobyf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qdkbxubf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2omjuweau.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bcfoxzhs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sdnpimrv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gxryhqzb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sargnoul.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zlawzirt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qdoawgii.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iipmhzlj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vmhriamz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xlznsmad.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yepmyttg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wqidggdp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lzyafcyv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nosirtqg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qyacuxtv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jolvignt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pfjipiow.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uvqnkhfu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dsbrprzr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgntqwhi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kdssrptn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hybwiarh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dvivorgn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fcazjiwk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cnegawbe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibaqgzwd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pncgunaj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pxbuakrp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ihbetekq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hmqqlbut.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rryxtmem.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qlnzzfeu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tumvbtff.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vnmxdokf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xnmwtlqo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fhmypjcl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2yxblaojc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rkwoetrg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rpalkhzc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iehymoml.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bbrgljwi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2llpzygiq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vtcdsegd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yiiglvtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onxrebou.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nmmmcqvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngsskxms.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2sisrfero.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wxtgemtq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pwoercgf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aduszang.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zqkwsplz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bypieokt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bcufatbe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xgbdndus.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2llvtakor.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yalcciwk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jglllezg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2cgtigwch.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vkptixbm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gqesyavl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xorwtzfr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gmrciiaf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hzpbdvnv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nmtknpwk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xedfcgea.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2cjiqmgkg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fhdzpymu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2luutoqlz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tezdwgll.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2idngtqzk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dkzovkeh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tjnujgba.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fugdzyej.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2encxxjrj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qklyexxr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2aoivinvi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ubogrwkl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbpfhsgt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2izogxqsf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hnrcqmuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2orkuxsff.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ccgkdwda.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vwpgnwoy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xptbmrqt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kcdqgfyq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iyuxeofs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fnactzyn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2oopggidc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2edfegcpi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2helhrxhd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsuiaxbu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fohacnjk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hpezsoxi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2uzfnjcau.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2uqmpvaxx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zfhwbvua.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kaipelsv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ixddtbdg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mnaftkli.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vkvzegyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdashqsq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sngteyqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cusmzcml.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2krrvjhet.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mwwkjqew.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2czofarfn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2akljtmwk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2blwqaqub.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pdwhajid.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sfjdtdzq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2acqvjkzb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2iaxwbpir.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rxhcceig.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2barudtaf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2iuoslgny.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bosekxpr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2bgrguhjm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpcnomp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2chpwclav.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rttcouyz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2opwlugxz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vmygqaen.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bpzggwca.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ixcqyivm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qpxyzpmg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vevogqhs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aqaxmwea.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qqtypcep.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bkeqrpee.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jftmgaun.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2gyygrsrf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ivwgbdks.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hxmqdjqd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wisyhbnq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vymmeksa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aroyxpkt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uprycmhj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vyclnpvb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hvukqaqx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bpdpczxw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2livvurkb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xzkgofvg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jybankjn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rzqquqdf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2gzfdzccx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2okkznlgv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2oiotenmy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ohwakcox.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ugvsargk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dskixudn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dvyszlxo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tvajwxeo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uymkdwce.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frphtcpz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bfpfwzvb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2aoudbefo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzcybgjd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tsheqmfu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ffodwsyj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wrjlufoy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2svfkqmvy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dimcuaok.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hkgwdkxb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uakktzxj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zcmcpyxv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jylimzbl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jqyuqakc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wowkikij.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lkxrkluy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rjcsqszy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2odmibgux.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vtklthwx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pqdmtcxj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2amjtnnlh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jkyxadeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mobnzggr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bczdhvts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrlxxmsb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vukjzkkl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rbbjtgrs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zasqujtp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vvbmqaxe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zuzevsci.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nispfkbk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dsczrvyx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kbzzkwbp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ynqdpevz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2punuqadg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xneyqfoq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2tvtkzbbg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dvlyfzcq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dzrbhbzc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kmmvtkgo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ysoagotr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dfhmyway.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xbtiifcs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hxfihbpi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mgqzkmne.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2skoirffs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2joftsxdu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2glmtxjuj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmzmksbi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lihpytih.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dgcgrpmq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dojyhrsk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dzjwrpxj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uwjqiids.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2klayjcep.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nanbbblk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oqbnmrkc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tkrzhmox.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2orxtimca.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xdieipmq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zfzdhexe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qvqeycpu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2cadcrkcg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2nodhasdm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lhqyiwxv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2oplxqtxr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdklcphn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nijcgyhb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zefkfbml.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2bihgafjy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nxsncrec.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fhdskiyp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wiaupiov.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ncmoqhkk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zfqqvvff.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ubbsldec.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2sepybjls.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2unsjgnyw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ztqcvbig.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dtrjkfhh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2anpqfvit.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2erjbcmym.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cdygyguh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nwnixnnd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtqtnlht.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2bliyxzcf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fdaipvty.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2payavovh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gotymrxo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hmtadvbl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxevgbov.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qwgqvpzg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2apfxucdr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nbbjapmm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2momaboqq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zvljkcss.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2swgnakbz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dyccoeej.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zmuevofm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mkyizczr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bmubvkdo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2omluwumr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2imjubavv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tyeolsmn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2duagunwq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jrbzusre.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cthnjcjm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uorbsoum.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iyxydrrj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2scoeukao.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2muxrvjol.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fbaechlr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cygcdofi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2cbftwhym.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2knlyaslt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dmvmfahk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wezkhwqd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2csetmumk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2musfwddk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2epxfntry.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2viegnzwc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ltfxecqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zokvosbq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2khqngblp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qnlbckrs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zlabmbmj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ymfjdzip.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tydztpxh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cqosdavr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2grusnack.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ioznwidy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hmcrkrvs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qdsbksnc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yqtuoqgw.html


<!-- 参考信息 -->