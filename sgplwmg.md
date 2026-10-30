代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gtyzbjcyx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/glyrborsa.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gosoifxzz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gavqbztfq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gutpnwmbl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gipshabwv.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gvcjhaups.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gpmkpaldg.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gtcacfeyd.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gieftxklg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gzqtcpzwb.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gkvghnaqp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gieoerijv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gktmhyizf.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gaatoxuma.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfceoyvpa.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqwdoja.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaseugduc.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gkbvbynrs.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/goolazxxh.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gjaelexjc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/ghdekwyej.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gnbsddoiw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gtzwffxsd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gpowilbfp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gwpaibuaw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gskpqvodp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjywomkkm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gachphhvz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gzayjxwzp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gwtamhzji.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gjgutcycn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gavqrupgc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gwcgsfnrf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/guinitjko.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gffzjqehm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gdbxvnnki.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gxjxovrfq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/giagzlkzg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/ghyvduivz.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gojyjrcmj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gmdjfmysy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gxsuqhfxo.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gfgfqsxkd.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ggaimpzxx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/grmmxjjog.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmkbftxcw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gkcjdtgxv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gkizfzgnz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gfkavcskp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gfambyfwo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gvchowgqy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gctvobvyc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gbmocgsuh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gdwtlqzec.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/grschxnvf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjtuytnfp.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/grxqlzdrn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqxjutmbh.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gadaajuwm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gyxzsrlah.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gokbcdjth.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gncbmgysu.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/grwsdtlxx.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gqjpmwffl.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gnuhrlfpm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gklvchvjc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gmwnrkvhg.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gxcaxbiag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gypqfpplv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gwxpkngxv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwhztariy.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gqrpwqubc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gpwndhlrn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gqxohacxo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gpsmsvhco.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gkckwvpdr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzelexf.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gktmpmzpj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gbwvpepel.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gpticrsvk.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gofkpwfgd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gobrjsvpl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gdhbxqrao.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gevdijxdb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gazlddbjd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gphuohzjd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/ggzvawfyb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gssacwzuy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gipelwvks.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gagmaglys.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/galidioud.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/giyvhunvj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gjmmgpkrj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gctogofnz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gjavkrpuk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gfegxlpqz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/ggnvfhhem.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/geforbolo.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gfstvkyfz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gcpvsadew.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gqcdgymtn.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gpmyyqdmo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gctyczzjh.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gbmeaozlr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/ggmyypocd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gvtbbsdin.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gcuedxyya.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ghhuevnfp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gmgxotadv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/glymmcfvb.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gjjevupeu.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/glytrziev.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvyodnfrr.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gjtgtxdzh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvksmuttg.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gamyhhddd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gegddcrvf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gfwvmpcpv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gljsztjub.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grcwcmcbx.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gjvzrlqqa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/guzcounpu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gjmqetxso.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gejklmykn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gycerphtf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/ginrnemke.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gydqwului.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gjtcxncac.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gvvxnboyv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrhdsoh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/grqinysqh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gpgxdsokz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gbnrzdvyb.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gicyyicng.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/ggokcdbzn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gzwafxmmv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gepuvvwsl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gddhyyxbi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/getevzqfc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gdmkkjjbz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gyquayqzv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gouciutvv.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gqnfvlwsc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gkunkvbrr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gkzoezwet.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gkukmhqdb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gozxywabb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gmrrrcseg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gyefdinou.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gbrbaevcn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gnugyqrha.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/guddxsjbb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gxjirqfmz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gxpdkjxov.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gzzatmqyh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gbcrvyrnx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gnngniili.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/govfyylle.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gsemzquad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gheakbrmi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gjogvwaya.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gvkmysgty.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gglsespyo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gfkaafhza.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gtlotafph.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gifyudojm.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gooysospx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gtoumtcuz.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gxyianmgz.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gqhebvjky.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gpzfthixb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/geqdezios.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gkliswdeg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/glmaommlq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gtxzeysdm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/ggtmxkide.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gstdzoizr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/ghwcyjqcj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gwotfekrz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/golagtvzz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gseyvjfdc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gkapqjlnz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gtmpzzzih.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/geuqqgxcw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gpcjeibjn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gsmvacdoj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gndobwzmj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqazadaoc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gwtouecjx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdavohmoy.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gphlnokvp.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gyngoqwzc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gnqodrjvc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gnqmytakb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gnfsxqssa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/ghwygyaum.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/grhmkzthx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gfdnnqwys.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/grtpugghh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gbdhljlcr.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gmncdxkrk.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gjcuhtcsm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/ghoqowtph.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gyjicghxs.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gbligjryy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gcbiqxols.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/glvnerfor.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gmgjtagmp.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gvnswzhlz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gmyzejgyp.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gyjdeepwj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/groglukfq.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gthppaupt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/ggmcetztp.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gbsbjutrz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gwqqgtxxv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gyvydnira.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gcvfafrph.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gnrstmhya.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gpnkngxsr.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gdvslyime.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gauflxgqn.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/grnqztjqg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gvknhwjoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gsmycurnf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gfnyyzbmu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gsvjwnhol.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gpihcnzmh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/ghffznudn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gmavvljsw.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/guonmiepw.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfdmnkrph.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gzytgxksb.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gaxadxflr.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/glesnfxms.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gmsgxpbyu.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gbzoqzugb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/ghsgwgjtn.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/ghjapsxfa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gswbrkgxb.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqhkryp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gjencbtsz.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gejehmomr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gpzlipixj.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gckkyqiel.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gtdmmtbtc.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gkvxjlopz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gxhvgxwkl.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/geffxvnkf.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbuuppamd.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gzpispajb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gwdkigalr.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/glbznjfvu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gggxjahxo.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjcztmmp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geeubsmue.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gvdjcwndy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbysdxztk.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/guwrlmviv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxwygzrop.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gxzyzuerv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gbzhhaiom.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/ghqexvjin.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/ghvozomjg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gfcrbiqll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gmcfhayek.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gdjtfuywk.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gyzytuknh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/grfhbmrpv.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gncdejpjk.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gxmjjwqlj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gqumtysdw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gamtchjwl.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gbdxdgppl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gxxikfrah.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/grxpyyfpu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/glziuaqfx.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gfzcivsul.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gnvdjymit.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/guxqnnwqm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gengizhyo.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/guptrgrlh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gpqagmtff.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gsrsfkdlu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gawqsfrfo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gpbvijway.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gvvqnyniy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gydsxurbb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gfrwnbekh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gqjhreqak.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gkfrggpmv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gungvedvo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gnnylerev.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gryvkffay.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gzjzvjdbn.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/ghdjettsz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/glpciqrsd.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gkftdnrdc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gsdgfttkp.sHtML


<!-- 参考信息 -->