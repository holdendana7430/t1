代发 wailian999

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gsmxfhrmy.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gkpwpifyo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gcjpwaren.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/giibwikah.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gxhddoehz.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gaboisefx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gxwhntdjq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkcyyxkyq.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwigfeekk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gxbyoblow.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdrrdbv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gnywdhuke.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gcdwbauev.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gqhuaoapn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/grbvgctqk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gccihwnue.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/glvounuhw.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gwolklcyk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/ghbdgkqpp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gxsbunhcu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gvisnmsmx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gypgwxisq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gjbumkwus.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gzlwheban.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/ggcixzyix.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/geeqcxbpo.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gvpuwvddz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gkvwnfcae.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gdgxidokn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/goubhceak.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/grpqefogl.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gjqckxhes.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gnaemziyy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gzpwxrygm.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/goxrhqwpp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gwgkmeion.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gnefmldak.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gshirnipo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gtyviqnfs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gvhcvgggk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfkcrolkp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gggltzsoc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gnozszewh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/ggrbmmjhe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gibuhsrvw.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gioxpgdoa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glbdeiisn.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gvjjzhpeu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gqtgwccow.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gnuvztgvy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/grfrttbty.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gykjnovon.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gicferzyb.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/grmikveam.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gbdectzgw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/ggducwvil.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gibqicney.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gchqaezcg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gsceilxxx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gbfxkvkgo.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gciuwsyhi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/ghtvzuvvn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gvnigquub.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gwkjboavb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gtesnptvh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gnvofuvbd.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gaxgvrzdt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gcgxawtrd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gmgemnita.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gskisfmeg.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gjjqxktrn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/grmnflard.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gsibcdizi.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gfclxtrto.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gminrdvhd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gbrhhotyq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/guoqafpjr.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/givipvtoa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/groufnmhm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/ghabhwphv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gyhudzplr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gflqnuddc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gwgkjvhes.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gqzfrovzz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gwccystxo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gfaeflkqw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjtxnmxxv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gsdudtojq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gvaqhnnnj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/ghkpnlhwu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gzecsossd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/giwdcsgyi.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/grajfpbpk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gwryzimji.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gytopjvdl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gtdwlbxwx.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gtwmpyttc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gsqokhqqj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/ggixmxcqh.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gipqqecuo.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/guvblfyye.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gblkixxvj.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/giytyuude.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gifmsyzfa.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/glhevhfvb.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gyizbdsnm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/grfhjweru.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gyxgebzry.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gyeetpmlv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvygisour.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gvsguhzpn.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gsghnvxwu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gmbyuxnqw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gujyjbebz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gwnjfysrt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gaoatpxjh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gsmjsepnu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/glxahqbhm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gecnynhdx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gnzdnuenu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gsanxioen.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gitbomdcs.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gexpsbqxo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gqxvlmorc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/ggkppxrek.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdfcjmltb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gimbboate.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gxqkiyksc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gjyadzejs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gmuvbtlhy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/ghocmgtww.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gpeltwbro.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gucluvufw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/glqrrqtze.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gmvpvzvch.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gdooorafd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gcskjmqaf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gfxhbhohk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gyfleqqen.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/grzmfjpfq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gpeicvncz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gmsvdvbwg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gaxnomewn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gntfoptck.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gsduageeb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gkmpykvlp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gobvziqoa.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gmnyzezuw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gnqaduvke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/ghjyqnsjo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/ggezqcdpy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gplsryenj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/glwzvoicb.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gjwzexrfm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gvyaohlsk.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gjwgvozzh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gzyhoexmf.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gamavwpqm.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gibigzwtu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/ghscurabl.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gwculnjak.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gpehxoggd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gajsvevgj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gffniewgt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gkhwyxxoh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gxvrgjivs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gbebopdwc.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/ggrhgbgut.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gqpmldwqr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gxyvibdmh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gxntmkliz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gcyufupcp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gsqlriluw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gmnvnbkyx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gyqavjkzd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gbyspeemi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmuwpsedu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gidqpimmz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpbvghdnc.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gxrsypugq.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/guzdowjyg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gwjrbdztg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ghheajyuk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gsjyfkhss.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gvtangboa.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gtngalxku.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gbbmintef.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gpkioqgmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gdoiqzwlr.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gxhoqarfn.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gziipcltu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gxoskfudn.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjqxruwfz.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/geygoobgj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gkqtkopzk.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gnwgjxybe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gykfgxpsm.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gldgmwpxe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gyoyfseof.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gsretzznw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gypanonkw.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/goebgqdki.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gvcfyyoqn.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gzcmpvvaq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gwbbtrmnp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/govmgwzxf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gtcrrqpey.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gksjnoczv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/giupuowhk.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gbtqiijsq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gisnzbfbk.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gytfrapbj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gmcruawkp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gefphrdqs.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gvvmmvftu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gyqlvpudw.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gklfqvdwt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gjhtqacxe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gqojjovbi.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gkrxgxlyv.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gepfubwmv.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gkhwpkneg.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjectwoia.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gvxaburex.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/ghsmffaij.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gxydfigns.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/ggwognnan.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gkecwvbno.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gwkcsckzy.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gaxqedcts.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gfgatkisj.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gwvoqzhkf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/glxletoxp.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gzkmdvqzd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gyrgnfkqa.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gynthezmm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ggsymlcom.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gevzmxqni.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gczapdvzs.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gmwbzllvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/guuuzwebk.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gcgpmcydx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggdowwsmn.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gftxaksno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjiutwymq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gknvivxgu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghmdfusgx.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/glslcdplp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/guqdjzrgk.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gghxqofdz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxbsgjgkf.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gzrzzjwcu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gbgwunbwd.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/glknlkfol.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gvxzkprwo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gfmsamtxt.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/garxphfwx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gxsimebox.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gvoltetyw.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gdxerrykp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gctlmwrhm.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gegxhenaq.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gtwllkjgs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gphrbmehs.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gwsujvcii.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gceunjmwc.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gdiqnuhsw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gewtmuxcf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gfgalazuu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/guhgfyhvh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gqozcicoe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gsovsjopo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gwqwfxlif.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/ggfvjeuij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gautduvvj.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gecalwjnn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gyxwivqkg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gsqfsoczj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/goyxojejn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gmzqueapa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gwlhtsozp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ghoomfkjh.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gpfvvxjdx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gmuhtdmwc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gdyqiichh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gscfnaxpn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gaymwxnxw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/grzvnmjdj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gtgimzmjk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gnjeenvnj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gfpkkxdfd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/grasdccjk.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gsivdaoor.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gkqmvqdgp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gqebcdsok.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/geksqbugx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/glrlhjbas.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gwlutolee.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gpgsjvrnp.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gxzzvzqlk.sHtML


<!-- 参考信息 -->