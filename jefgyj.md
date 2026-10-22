代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvmwjhnh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tpruuhvk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rlolawnt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jrruklqe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dlqskggv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iouhdzif.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pxwrcdfm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pasqvhwg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yqwuhlfa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uvjzbahy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hhypmfwd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dvujmequ.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cgpacvhq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2archchwf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ssgpyezo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vdoigqav.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2bwczdsgz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yuaviyom.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rhjcvcjr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pyyjpasf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtqeptjb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ozuyrwll.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2daogyqlp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uufhppuh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qsnkyidf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqpxxctw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2phglhyqy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gofsqvld.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qphwryae.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lozhjeyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cukbwpvb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2prbbqeey.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wjvjqczs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dlbtdkaf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wnkafjez.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sfewtblk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2wgnacyva.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wsfjyqdz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wwwqafvs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cboqwljp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bbwviemi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2uojgcimw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zmhvqwnx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wmolavey.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mmbuhcjn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ajetgzvs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nokootke.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2enpngbuh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2quxrleyr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tkuptcvh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xmmmbvpl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lajhpcfh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2spruvlxm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2uibavbgw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jotduiys.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dtdfhejz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cioxlybg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2sadshsdk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2onejrkbf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2niphbyqk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zpehdgfy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gbzakhkf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sfjjouvk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rtlpwkzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwnuzxvf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xqwemxcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yptuzlgj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wmkziubm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nthpsyut.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bnbmyvye.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2udoltjwh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rmnrdxnb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vepgxupj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lafekhov.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ibocwoho.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qehlsemg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pjjaatww.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jljkqoxu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xhscyaza.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wdxjoiqi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2btquxilt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2stthetkg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ztbrpgje.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uerhlhrg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fadadioy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tylrzxsy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2bcigleol.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lomtlugr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ounbuhvu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2knmonkdd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctnecoxs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ctmihwml.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2aauloieq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdcmufqh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rsupagqg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pbyykxho.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yjoglsmf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qselgvre.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrosyodm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yqmkxmof.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jfosibce.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hfmwlflb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2drfmbyrl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2yhtqatxr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2jdhwzesf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cdxdhttn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2opiufvth.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zpheumpn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cxzpmlkn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fxlndaag.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uqtffwhv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2augaczfg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jpwvckba.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2johflzon.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2amtkvruo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2eulcwrjs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2elciorlf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cdqhkufo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ihrwvsvi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2thdinwpb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zwjtrlzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqmdtkoz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uxaxkdgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgdvmche.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kychpuuu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2opgycdpi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hyxewjcm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cqjaxgkz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2diimiitx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kmjnipor.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wpkavklk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jdrovunb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ujpbicer.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tihgagsn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2urirvmwl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2cblotsaw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zvwbwutq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ynuznxjv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qsejznkz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gskqgdoq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drlyhuup.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jlehezpu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uiycowcu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2shzeulkc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2znohhumr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2izhwtsuq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wmjgbffj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kcicaoog.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ydzxjckv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vjxiodxo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2xjpvpmyz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2brxfvvyj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wetmilet.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wgmkvawr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qsizvbpl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tbjvxdqy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zyxczmve.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hhopswgv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2irqidpxk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2svaamrqx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cfmiepfc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2edhmgvqy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hswfhbkf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ljpietzt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rrjpwlwv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zuyzmsih.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbfkvdir.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xejxlrbf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nejulnsr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2uigdowkl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mavxisrm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nouaxlxy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tacjwnkr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2oyxxzsdc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqronzpy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbhjxqwy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2umhrxxye.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wshpzgcl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2aayrahzt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2pbxdyqrw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2twjuhhmn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jrsweivh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2csfnzvff.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jaefrnji.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zpgdahkm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vdwxgdbf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jnillprf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ckpadknb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gfzuzoul.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kfdopgzj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2spzariuw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpsuscas.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2euybkejz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fbavhzjh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jdgbngdp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hjjurmcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbcdauep.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dogonpmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbaaeujz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rzqcwzfl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xqfaixjo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nggsyvji.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zqrfkvyj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ucgnevzg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2abpopimr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2olfnptut.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hujjgqzm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2tsdahqoo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2clbdlsfx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bjjvdxpt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hrokadnz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wnemccdm.html

);
来源：http://www.52xcode.cn/Article/details/gt2abgvducq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hfginegk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nbsqxqrw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xphwulfu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jrmihqqn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tbcvayev.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xkkotkon.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ysfmouaf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2iehjuptw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lyswdrjw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2crvhsxuq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cxwzaumq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qmqomync.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mnkavsuc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sublkfmh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pjyygjkg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zzzldfbc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2smrkiakd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gshuaivf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jghaninr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2nenwgcup.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xorczmfw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zajiktdm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gtvidklo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ziisiseh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ddqrmbbe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2xovlhjpl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2spwlwoxo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eekgjvzx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2apbghklp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lgpzqplb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2utoopefl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jlfbabav.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qqquejaj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nchioitb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rktiumnn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hlfswleu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nfjolqfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fqsovumo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2iwhklxku.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pemphawu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fbbpzbfz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lasndaai.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bwtzbgdw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ocokvere.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jyepnbax.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lowcsccw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hrecegnn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2idufewhb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2frykhffz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eagwfgme.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2poflrbrh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kersoymi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xejbnimo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2agiopzno.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tjikioto.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2potshrcw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zjfcpjhf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dpcnqhvv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wlsphiln.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tupxiqgq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igkqrthz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hwyhtwdm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bnpemlie.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fzsttcgz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dbkofagf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ofidygym.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lnnvrjjv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zqsuekkp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2uyyhrlag.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ieknfggd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xiviiqfn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2thepjnha.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zwxfzyzh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qergxxrt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2heuhmvfv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zqtgdzvf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pywgyqqs.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ynviekvn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2njzmrdtl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cgrkszkz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bcvmmuml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2oyezpqkk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zvzodaup.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qewbnqxn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2avjgrpfu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fztovbtk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wcoltebc.html


<!-- 参考信息 -->