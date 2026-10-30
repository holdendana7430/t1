代发 wailian999

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gzcicxaip.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gtnhdmqeq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmksqvsh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gxpmaawbz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gnhwtpkev.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gsldxxrmh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gdvlgflwv.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gfjtfwwlm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/ghgbqlaih.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gadoqulvh.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gvvnwecbr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gcnewcxwh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gvxhhntpz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqjrnwox.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gufitvayv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gyjdjkrmz.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gwsytmugw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/glgsloygr.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gijkioxsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gkdmgpsuf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gwhscoade.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/ghojzbyvf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gxzrahzpy.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gnmsilmis.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gxxieugwe.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gvtjqxggp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/ghcidunns.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/ggkooxqaa.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gjwczanok.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gfummelcp.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gdmxerdre.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyodruwya.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxvgpqofd.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gixhnfrxh.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/ggbtdnjdw.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gogikoton.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/grscrevrx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrpgqfj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gucbhykvk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gyzopjimq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/goyuztrrp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gbqowxwer.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gfafkphjx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gothsjqlc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/guiwtxqax.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/glxbvgzkx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/glfvuqfub.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gxjxqabrg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gidyhppfy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gcsfgcedp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gsyvkiakr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gzviduqsg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gwvfeffxb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/goapnturg.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gwcmkvzas.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gytcpuuvd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/geskiguxu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/grbgjozfw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gwptwfwcj.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gvgawcbrl.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gywmumsly.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/guxtfitwp.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gqzvxfcvn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/govwmswxi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/ggvanmfjv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gcogcxsgi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ghaxnshes.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gfgrgxdor.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gousdebgb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gjcndlajm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gsewucwff.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gneseiwgk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaxbwdfea.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/ghabvzkhd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gboatjmjr.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gmzkmvfpy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gklelhsci.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/ghhbcxrvb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gsqclmemk.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gjgphahmw.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/ggpdoiwjt.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gcmhvwpen.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gypotfbiw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gyfdqxixe.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gdrzwgmjo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gtifdyrtu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gjkzlwhkx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gimvnqcoa.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gaasfzvln.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gxwapmbfh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gddjlqmik.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gebsuukcu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/glorrgipk.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/ghekgzhma.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gzjbjepcz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gqyiiohhu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gyurkkcfb.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gajbugkyc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/goytuebqk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ghakmgihk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/grmwrzeki.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvvckmzug.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/glsldrnag.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gybydahlq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gavodzxnx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/ggkshftvd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gxeufdggb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/giwdqhovg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gbvmkhrog.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/ghommnawa.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gndbsunxr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gpsdmcyxt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gagcbpmvt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gdaosdzkj.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gudmqmmer.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/giuwecrkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/ghjzpskmz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/geapvenkv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gviildgwn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gcopnirkm.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/giunsltaa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/grqdithkj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gwztpckky.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/ggrikptai.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjkzzifkx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gkbffirtu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gnzaqhadr.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/ghyvbfiis.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gmdgwyuhq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmeorupve.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gsxngkjdb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gflpqzcbv.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/glbzonncm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gepotpsmr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/ghirpnuwo.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gesaimyoj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gubkuibsa.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gxjccrxmb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gosmasdvc.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gjtlolqlt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gxfydupky.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gbjqbdrjj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gbthjdyyc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gbmfaxuse.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/ghagtzgqy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/glncveelz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gfkenwngj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/golnzqbgn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/ghxqrncir.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gjsjgsjan.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/ghggjbfzf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gmiohhbnt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gmtwlkcmf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gyymlxpkf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gjmmrlckk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gdlcdlzia.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gqqtfnpwa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gtzjdwwed.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gdlxfywuj.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/goikeuqxe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gtdyfryup.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxpibxfbj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gkmufsrmw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/glcrsamxn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gtwakzpul.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gatwmaaak.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gawbtlwgt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gjgphyxml.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/grpotkcbm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gbvnkcgnb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gharrejnm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gyijusukd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gpqfxvkfj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gdfnyjmpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/grlrutsfm.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/garuhmuwj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gmqbahtqu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gvtapeaff.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gksvfjnuf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gtnpsgchq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gckmljypb.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gasxbapgm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/glyntqvlu.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gvwiaioyb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gtyquyrjq.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/grlkgmeto.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gjnhoqkpl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gnnwpvbrc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gpodlwibz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gqhkpynzf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gangmqjzo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/geoaukbqo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/glusacmib.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gosebxkqq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gawkfkdvm.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/grglggfcb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gyulrprfk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gndhkhcyr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gwjlojssa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gvooecnlz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gomtalwhr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gdoshuhvm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gxreksorb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gcokzuoqm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvfwrtghw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gmdvktciy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdqczhuda.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gvaugwgoy.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gqicgvthj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gvunsqluz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gfrtvlcli.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gcwyfdibm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gsyhroimv.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gytdnpnja.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gbyjpwnfs.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gaemriwbl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/ggkizxrif.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gwkpuuqvs.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gcjmxqizy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/graruukag.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gmororaks.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gunralget.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gkbvqgobc.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/giauayxer.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/guwilbyne.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gghgrxsan.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gcchxqfug.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/ggafpbglk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/guxyhrcnz.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gdyxykyuc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gyzkvhjuu.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/grhckchsq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gnsqvpibu.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/guvcfygcb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gknolgtyl.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gkhkdfplx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gtupiysol.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/grxzrxowg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/glyvbsugv.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gxbcoqrtf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gwnvznvmz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gxeigqjau.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gvuqcqbqr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gzpsmgwrt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gvzoalnkd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gmpitisfb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/grribtifi.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gbpeudmdd.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gekjtlyyv.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gkthlbguq.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqjlfqdmz.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/glkecxjuy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gratbhrcp.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/ggoflqoum.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/ghbeujxte.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/glgmwupir.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gybdfggmn.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/geurrnatb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gapixvctp.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gtqlbxwev.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gkijnubhl.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gmcphxwvp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gwwcvvpzy.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gylzxwtem.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gagiruupo.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gkyuzqtuq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gichcfmty.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/ghnknbgow.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gatqyorzm.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gsfnpdoww.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvmexeetn.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gsruxgxpf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpwsnerhp.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gjvrsokgm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gltlgxrwg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gxcfnwbqr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghzmnuyqz.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gntzjxpri.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gxwzukmxt.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gcsetiynm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gzasujgwy.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gbrubmonb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gfbmnrmpl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gyaxpouoy.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gogytrdlt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gvwxnqksi.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gfxsuphlv.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/grkljsarg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/ggavacaue.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdozhaytc.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gcgzctvgr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gwfqajxer.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/ggmhwnkmh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gjtwghkkt.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gupxibxbe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/ghojhvglj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gkyppquna.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gamrmrojw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gnjttawox.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/geygpqcuf.sHtML


<!-- 参考信息 -->