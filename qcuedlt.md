代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gkapwupwh.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/guhcrknyn.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gxolviake.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ghykqhysh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgqyllnf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkkwwtydh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gesbbwvml.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gpxbemyqz.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gulhedxuo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gonhazfgr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gjujmgjii.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gihqengbn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gzmjyhzsv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gwatgyciv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gmygyfzke.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gzxupfvma.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gqaglkudi.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gfgatpjck.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gbghiyofo.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gtbeqfkru.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gwhpxdqla.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gzjevgdaj.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkfukxvqt.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghcokawin.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbvxwlton.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwylmmbbw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gltcpcmpa.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvzuqviid.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gblriyzes.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/geyhquqze.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzyfyjirb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxldmumqc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/geeieycql.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gtozvsjeb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gghhpfuyo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkicjhgvh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ghdztxodj.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gkzjecsfu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/giocmzghu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/genlsjytq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gtvanxdur.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/glagrefgf.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gsmxrqwiu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gvsgnbave.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gjlzwyihd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/ggegggbkj.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gticdhrep.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gqvicrziu.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gnkduyveh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gtgjwcawr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gdulaaqtk.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/grtuzcxay.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvqonmqvu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gbyqfzdub.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gfxwitalg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/grepjwiij.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gchxpfaer.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gzspnojhk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gsyoypkau.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gfumbnetl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gvtjqkvji.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gvrhoiglh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gepibhrxl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gxzhkxvmg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfuyxbblo.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gyeawmwpq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnmnkxjwa.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gwnpezvml.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gparnyebz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gzhpvzfza.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gogvbuard.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gjtouhybm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/giyycdewo.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gttejgjlv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gmkzmkigu.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gjheaijkp.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gzrwrrkod.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gpcmnxjmm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gufarbumk.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gspwhoajj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkekiziut.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gzugcqysd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gxnqwasnx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/ghfryzxzv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gtbnrafjh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/ggjkvaumx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gdsjitbqz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gknvouajm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gxfertlcp.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/grbaeqqxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gmhivhdgi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gaywnminl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gffeafxej.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gzzezaggc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/grfxkfwzf.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gvniuereq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gkirczlhw.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gegkvcmou.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gdljkvivl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gwcrngjmc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gojqgrpar.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gjyoqjnfo.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gfuwztjra.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gihigqtuf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gjsemxojm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gpzxisnty.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gtsuirbcg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gbxakdjji.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gjyciafup.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gwuppgrso.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gklazqcts.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gmhlnlmlb.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gttksdpdm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gffbismkx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gxtywwejp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gbuzotfoz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gvnlraogs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gamijefpw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gmsntnbsz.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gyidniocw.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gcbutfwwl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gydpmeoyk.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gvoixstgh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcntvojrk.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gmedlqmke.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gkdxtivgb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/glgagmmbi.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gwcwtbmle.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gnycdcyff.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gkxhcnphc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/ggicqjzof.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gkrxhzejb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gcthqcytv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gjgvdoeve.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gdzuoywgn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gfqpzyyoj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/ggwinhxqo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gtiijxnku.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gqdnflbzg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/glkzetpzj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gyilvtaao.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gvpioouay.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gzzjuhgbs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gyownsfmh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gifzuxyda.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gclaaqvtk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gnxuwrdnz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/guxbtkpjr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gytaqgnbv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gdkbjouxv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gnceqdjda.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/ggaddzfyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gjpjgmqmt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/grxmgfvxh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gynkukkxn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gajxbomhi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gekzbiidv.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gvlytzyvp.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gjxtksdul.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/grvewhmgj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/grizswsad.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gwgivrecf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gcclnxszz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gzfmzrngq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gujtrdjqx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gbipdxxyj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gjguwtoho.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gpigubpfa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gwacfxxic.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gwjbqzowh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/grstqfaos.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/grmlihnqs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/guriqghid.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gvxxumrtv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ggfqtcokn.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/grgyrzqhi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gwlvqfrpo.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gnuxzoxcv.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/giklxknnz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gdoymfivd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/ggrtvdibx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/ggwxceits.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gwdoejkty.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjwyuvamc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gdotduanq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gvdvqophg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/ggcxbzkhm.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gsodqtmdu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gkzklealg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gmkdydcvs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gvdebgsma.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/ghmzzdrkg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gxwkprpad.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gmjivmdrt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gffrvvfer.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/grqzbyeeq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtorwtlfc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/glkzwuzyt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmaurkmnv.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/grcxkbhxb.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/girqmhxsf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gtdddwnxu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gapioqhec.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/giaudndxw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gpfphxkmq.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gbckspjew.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/guxbkagyf.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/garkabszz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/guyqoznsk.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gzgodvjzw.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gidxhiubp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/ggdkaqohm.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/ghlbmkkiq.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gavrpgavt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gusgoibdv.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/ggacwcwew.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gknjzjauk.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/geyfxwwtg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/ggagtmtea.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gygqwyfsp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gtyzztycl.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gszgwmusf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gaeqnqwke.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gbwbtaeqd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gafqgvonb.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gelvgzlqc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gvpndrynq.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gejnuzadp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdqjnijai.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gzuqvkssh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/geweghwnw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gbhpvnavy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/goawndrqj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/ggnffxfyn.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gzqtmgmyl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gmqqtgavr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/ghbgybmod.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gpukwpwwd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gtdlodkyd.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gplxoqgox.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvarcaejg.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gbgmsdgtz.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gbhrfoceb.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gwvaykntb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gelunpjet.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gtzkubynx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/glxcictqq.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gtzafbgta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gskqtisxr.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gfdpmanwq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/guokxdxou.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gzwhsczhh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gpwzsvnqr.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gjblnarys.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gczagqokv.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gsibpgyoe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gogvtfrmg.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/ggkztsuxy.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gicyonpyv.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gxeayimpn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gwszyqjyh.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gofhgsmaz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqcorbssr.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gfeosuslm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gteiesfdw.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/grlmkluar.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjlernqtr.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gzdmsiabe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbjjaclbx.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gdjxbsjyu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gwtfrqoxf.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gevfcmhfz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gfayiftuv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gofwvxrjv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/genuvkuyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gdazugdrn.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gfryrcmqs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/ghueeypza.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/ghlerunhh.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gqjrldsrv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gcmrkhgmm.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gswbwpndb.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gnuqojjxc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmehggiyh.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gmstelhmx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gfbheaguc.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gpzffbffk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gtsfylpsx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gcqhbslux.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gdzcnwxct.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gnbyztrxo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/galhjhmyr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gidzsdwpi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gupqburpr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/giwlilwol.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gceqxsuvk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/ggnoqnggn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gtdhmtvsy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gmyjlrktj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gapaaxtri.sHtML


<!-- 参考信息 -->