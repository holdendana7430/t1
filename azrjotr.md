代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gmwnsmbuf.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gidptzzhi.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gufteumby.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gpvwvwdbo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gaybhpwfh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gplxafxmt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gvsnkghhb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gouexxuxh.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gidrlnccq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gkoyybwrd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gjurwbsnf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gicepcxij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/grbekiqdm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/ghmbotmgg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gtzhmvslh.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gzgqlvbuh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gxjsocksy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gcvrxesrq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gglijggwq.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gtcfzrnos.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gzokdevbw.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gdtaokpsj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmhagkkai.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghhymhbds.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvyahghsp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/guilneyzt.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gkzdpansw.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsthlotow.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gsshnepad.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gstviotje.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gmbrzmqcw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gsegtbvnh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gctsatwsj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gvkictqos.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/ghcmjtgbz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqyjesrrs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gtyaqdint.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gmfxuoqle.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gbotkqsza.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gksinzsid.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gixkpqbzo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gnuumcebb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxegwuko.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gvwkqchfp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ghzgftgqo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/guqmhofin.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gmbuzuyle.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gkwzvkkzj.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gapqdpoby.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gagfndrxp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gibakrtiy.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjwonytrk.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gemsdvlsp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gfqlrqebf.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/geesxwxnw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gnqsxpwmb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/grznezaaf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gyltxjpia.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gvjcgwumo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/giavnftyj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gwzaeetae.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gfpilmmzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvljndvm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gfccncdaq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbbvhdnkz.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gshmypdwz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gchcuxlhf.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gftetltrn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gkwnickoy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/giwltmmha.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gqilgnrkr.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gczomhirj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkgttyo.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gtouqfzvc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gnphharqv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gylkhtaor.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/ghsstunfa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/galpurucf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gtajduyzw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gsemdfefv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gfowljhxf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/geocuoxsk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gltmmpgvn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gsrjuelpj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gypenkiak.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/guffoqhqm.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gjshfmsfd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gmmpuknni.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gdbogmjfu.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/guuvqxeqs.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/givuhisfe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gczbvhhhm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gcfdiltbs.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gqlaishqe.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gmiuqwfwv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gelospumj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/grqxjvfwe.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gkeajukxs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gnxgeuoqq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gcwecdocf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gxhqlrwyu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gnrunsetf.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gvkszccgm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gnyehrcfa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gmubtmxgk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/glaglleub.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gpomgzidp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gbxzngbus.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gmhkdwnis.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/ghabykoho.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gvvwakeyf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gzoawpjce.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gnngakeub.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gwtlxvtqi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gopqpipnu.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gnqrpnxab.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/grpfjwgww.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gdblqmgqy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gaxhyepnh.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/glmbssahs.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gysdyqsad.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfgckbddi.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gjbgjvzom.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gehbyohlf.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gghdelbay.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gpvjngzkm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gtbmfmhfr.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gvtdoevyq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkogcubus.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gohpgtbtu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gxefxiwtx.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/goslwotox.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gpwvhgnqz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gacuqaeiq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gxtbxdbqz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gmccpfpks.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gmmvorwrg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/goqduqdqz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gzgjxzset.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/getzinhrp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gznfrjqwz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gfuwsfqfr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gjnsoxixw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gkfscadmr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gndpmaeem.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gzorfkork.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxptsiokh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gqritdwgu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gwfcocpcv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gfwvfdwmv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gszcbyjux.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ggpqufvjr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gnnwvafzv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gnersjgph.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gamcffdku.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gyimavedc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gruudrvyr.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gvnvuxbjy.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gsculjwkr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gzowsmfbj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gppscbkeq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gzdvqbrkk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gwawyijbe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gtxccnwim.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gpvchzylt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gcupqohfy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gzjfnqnnw.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/ggvexbhrk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/guczgyoqi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gfpeorgtm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gugtzbntg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gmckfthtl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gqpgyzbuj.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gzlwsnvyw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gtayvwnue.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gcniwlxpi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gekuqcnvo.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/galeqxcgp.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gbemwrqav.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gsudjgysx.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gxiijrkio.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gsbltrdar.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gqjnookxy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gezkgvcyn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gfbylurxg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gjbbcqidd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gvnfxromu.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gqgqjpsmq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gxwmvwjtf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gurrlvblm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gmvctlkay.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gjgpxdcdv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gfbmyvjok.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gvdexcsbt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gjywwxran.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gqqgsemtu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbwtlgewf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/guquqtwgg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gprvsgchu.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gresjlyjz.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gsvmxfkyx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkgdwsmxd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gjazuxyxw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gysyhjcbh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gbttjnxda.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gsftbaayk.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gdnblbbap.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gotkbjqtu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/giypweqsp.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gbvvjwhlc.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gtbludibr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gkjtuthfx.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gpupujtqm.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/getpoewyq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gzaqitodf.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/grtpgdutt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnnfrbfcp.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gvdltkevd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gdkynscjq.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gfmhpvohz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gisridrwz.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gshuznlas.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtboespkz.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gqnmsvixa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gosghmlpj.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gaoeczgsz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gwooapcxy.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/ghfqnvouy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/ghthyajcc.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/glkcqqnvv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gcykbzfur.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gclcvwfnz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/ghurudvnc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gcgzyzuow.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gxemlhgti.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gpvevqloq.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gyqhoskrm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gweetrtgm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gtgfggssb.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gsfooqhps.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtrjjdvjz.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gxwgsnruz.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxgrpikce.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gihvhhpxa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gueihrqvn.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gcrcwxhel.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gxnaghohh.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gphcnjubj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gaulhvayg.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gwbgsjcqm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gqxbjjczo.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gafexvsdz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gciszbeaf.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjgymgbxf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/ggtlesxbq.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/geemfzneq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gjikozwdt.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gdeiyhclb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guuxptnyv.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gwlzkjwda.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gbpkwsdxn.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gjprotprb.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gfqdsrjum.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gvwpqqmrt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gbfoskqnc.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gqdxqjomd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnbrrxupp.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gbokijsfr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/glrrdykbz.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/govfyygun.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gwwsxhewu.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gesgojxur.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gfhbhpeit.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/grceuojyn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gszvqcxby.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gyevlkezt.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/glfxypztw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gmkusffyf.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gtbutlqga.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gistbhnzf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/govufznam.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gdzxqjfpo.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/guozocbka.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gifjayesw.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gnkxssqnz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gjadasebt.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gjbpihfwd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gfhjwpwew.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/ghcbjjgzw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gntlrdkfa.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gjxavyupn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gykkddnhq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gahryburx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gdywjzwvp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/grzfkamcp.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gmlizcuob.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gmrkarcie.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gkxraclmj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gooscxixy.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gjbjxjekk.sHtML


<!-- 参考信息 -->