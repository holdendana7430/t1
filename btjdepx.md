代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/ggxhingez.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gruucfhtj.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gbqpkhuay.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gtracjqrl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gafcvubiu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gafwjhgsj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gypmvnrma.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/guipcxhkv.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gjuxmnemf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gfgbyacoi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gzuiwljzg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/glcmjtrai.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gfspipysr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gwjqcfpmc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gvocbmaft.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gbzxctlue.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gflvxpkml.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gokniyckx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gvrbdlsma.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gunqgtfrx.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gkgtjckup.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gwdiejxeo.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gwpnacezb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gbhirkaou.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gspuowaxm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gftkfgsvu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gqirdchhc.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grbxpyhfw.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ggizwgjrn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gjtukcgct.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gplixfhxn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gjobvsjrc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gpmbpvjkk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gvsydmjcs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/glextzgut.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gemszvjls.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gxuopsuxl.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/goiidlyhx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gmlyjlclp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gutftdmtx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gsnivawqf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gyunjsfst.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcccuujqv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gqapakfum.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/glefssstp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/ggmeghumr.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gwjikchnc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gkvfquybv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/geqbhjlqq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gugbfnwcc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gsqzlwojw.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gmhqssrpp.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gxxhtoked.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/grmrvdadn.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gjfxmiisl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gdvujjsvz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gfddacxef.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gfycvtqza.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gsngffchh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gbgpbvwuv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gqwuywnqu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/ghwlfhuwt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gcilcwbeh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gecrjtmmg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqkkhuztp.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gsfnaswcv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfizrpemq.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/giskdhrpt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gzqptenqt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gsbitplhq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gtpslcrez.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gbqfmdwvd.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gkyyvznjd.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gtxbgdkrk.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gnqaybaoj.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gtkzehkqx.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gqwncfjuc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/grduoxdnr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gmligftyq.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gitnbawha.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gozmeoxhd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gicfzbqdf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gwjtevonx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gnfjhefqo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gepcofpyp.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gnxawzkel.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/govrhuaaw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gtsydngwz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gmwlmdbna.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ghmtiadhw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/glamupjks.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gbwtlsoqg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gbgxpukcr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gezmquolr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gedjhehyn.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gbyewdmfk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gupotkztr.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvmhlavd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gqcqaglug.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gfgbqlssw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gravomomv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gxirhlnli.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gmkwdapxa.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gqliutccj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gejmwhhtq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/guotwdexv.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gfxhnhyrd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gwyeeyxzl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gsngleyfd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gtzsfjyas.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/giroyhvpv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gbhjdmwlx.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gwumiyidw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/ghzdmrstp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/glgexifna.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gfpzcsxmy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/guyakjjwt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gnkqqllyb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/ggzkltwpx.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gfrbphkzh.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gpcibcqhf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gosxajewa.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gezptgbqz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpbvwwxon.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gasxduobd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ggibqlaqe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gakqykxzj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gxiiadqqy.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/goydyomfe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhdtzxa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gedbfqwzt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gnoiidozz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gaksscutn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gtvunccic.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gvbgikkdc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gwnkrqzsv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gvqndztuz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gkvlchztj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/goxaeyrku.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gqqgcpvsv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gkwpcdrqt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gejcgxbik.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gsnesmpsj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gdvxlzyyc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/goejmcnvu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/ghojcnrys.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/guwcriqfk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gqzfiwwyx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gsvsoxofu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/guxfwulfm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gvaxcdaxv.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gyungjmll.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gybwumbut.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gzkjiqxrv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gagnetrqq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gsjobbutv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/ggwpgtewb.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/grtnoqvzd.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gfqfcbddf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gxkfvbphn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gzgwsvfzv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gwmzafxnu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gtlddvldg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gmoysecta.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gpbsffmod.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gsgmbryzr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gjcwulhdj.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gyssihazr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/guoewfotq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gyluqxegg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gdvbeamfo.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gkkvdurqv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gykpjwluz.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/giqnqwkuz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gmglufgjv.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/goifltxjl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gohfjwdzt.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gidksxffy.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gftsfboif.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/glwkvifgf.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gkowiovea.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gkmfbzrmq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gldrthcoa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnceegmkb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gssrrdzfl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/golzxsubl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/goghhxpmh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/ghcipepyc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/golqfirwr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfxboprni.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/grucwhepm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/ghguzxxjv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/geovwzmul.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gkrmjxhdv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gftlmnixx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/glresvqhn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggpiihugu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gdgtledji.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcolwnory.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gfbhnjmeg.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gtgkkxyde.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gzqouokvv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gfbevmchd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gpvmrgprj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gmgzkmwix.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/garvxtqtc.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gvwgchoxk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/ghdhvcoww.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gckkctbae.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gdyiortnz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/glmzqgjqd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqvhexbi.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gmehmqufe.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/goqajlzce.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gqqseuvxg.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gneotkdme.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/ghlfqzmmz.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/giiuiqrae.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/grvxomdak.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/guglckosx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gvhvawzdc.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/glyyxrgjn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/giztfpgom.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/giuxjvnmx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/ghvlfapag.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gmczohlna.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gjwgrnaur.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/greizgkeg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gwymtngon.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gabjuxdjo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnvfpjtnt.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gaodcidrm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/goqtjoluq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gjckarcch.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gjeyobuim.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gubrdtwjr.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gkpcalhvt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gsuvsujqv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gqiyfnyfa.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/getlusrah.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gdohfrbak.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gnnxumgom.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpvfvwbci.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gspxjbbts.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gvsqmkxpr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmlcalg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gaocrflyp.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gexcobtsz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqgcazlg.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gnjjttnzk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gdkgifdyx.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gjmfbzbtr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gwijonukc.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gqjqfulzk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gzmzmiwwf.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gwjkuihpf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gcoqqdrrl.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gwzhmazmd.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gamwvvevm.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gugozwskh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gpwvmgfde.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gvslwvudt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggxapztxm.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gwkhmhzgd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwokxdipt.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gaembxsyw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwniuwveu.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gjsankxcz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/glhlcvogm.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gjwuqnjyv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxlbipfxn.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/glrwdqanj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/galxsckez.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gqnigffqm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gefqqegmy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gqskcdvcs.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/ggdxmkipr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gyuakgshw.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gjkvcsyda.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gjudmdftp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gscnoeigp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gajsyonkd.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gxmmngehd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gwpvqjqmt.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gblyzyoxp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gcfufoqwl.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gfxcyjkqj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gswvezqdu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/graxdsmgb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gaikwetii.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gdlwnovxw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gjcvymlvt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/glgymelbs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gvxfureuo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gjpebpvkf.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gyjaktraq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gaorelzvx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gqbgzcfkz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/glhzhiesh.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gqewcmctz.sHtML


<!-- 参考信息 -->