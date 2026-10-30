代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/glpyvcwcu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gmdfpzxiq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gfkqazdan.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gktinlwgi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gpilahdug.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gaqznmyww.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/golgmjhoc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gxfxjohki.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gpxmavjtq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gaehbltkw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gyxgsbxbv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gbpodxvxg.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gpixmboha.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gmuddahpb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gusicasur.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gvjjfgluj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/ggyjigbze.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gfwqzyzjf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gihaencvv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gacywpkhn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gcosqnkah.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gmtrpaoee.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gnlwzuiqa.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gujdqsvxl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gwfytceik.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gfeezever.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzkcwiekd.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwbpcfiwk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gpvjdcjbj.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzlwkkjfj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gplxixjlf.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guakmfuob.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gjyctqrbs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gowmfxskm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gtkszejzg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glvpsxeer.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/glmkbsysu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gsfcboiut.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gzgtqmpah.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/guzknchug.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gnmjlqubl.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gjbjulowh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gynclypij.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gdyymquud.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gucmwplqu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gjizrjdvv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/golaouckc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gxysaxcet.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gxivechdk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmnwudhv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/ghfvbyzqf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gfbgvydrn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gqtyrupdi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gseytdxdw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gfgjgjxln.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqjhgtqet.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gbiifiqxy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gyqmngyyn.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gdlfcbftq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gznrzoqex.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/guisvzdcc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gslnfmuzu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gysuesueo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gknxvgczn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxfkvuanz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gjzuhhhpv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gttjhahye.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gsdcoucgn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdbtkxxih.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gslwsrjfg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbzgqhbqh.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gipmzomsk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gqfuxxzcl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gobsidwms.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gcgeegznn.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gavgqsbqh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gmxabjeth.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gpsbhhcuo.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gvbvbzidw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gkhwopasz.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gpjmbnclu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gzlkelmhg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gkkwguywj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gmzgyrljx.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gvdlwrgfc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gryzfqfco.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gbgbylfqj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gircwjwfx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gbhtumfjb.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gmuqdexxm.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gnqxveuzs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/guvbndtif.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gwkccutwb.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gryiwfbkd.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gafesjlzh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gtdpxgdqb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gzdeasram.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gfvggdgaq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gkjuuggss.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ggyfkbzjz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/ggvkfiifj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gijzrpewe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gpuhglbth.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gvbpbztsd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gyckyckvr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gedloqgkq.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gvpraybzv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gdqnxjppm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/glbrorrip.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gepdrpotx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gihzpgvzn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gomjhgewm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gfjlffuqk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gstwjdgyq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gkcaqhpcq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gbrvanogn.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gcvlkokmo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gaslnjhhj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gdodrfgek.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gzczptkxx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gqpgpiiui.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gtvsggdnx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gcekbxczh.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gjiyemuwf.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gzemgtzbu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goqmzzthc.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gntkuvruw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gktzuztro.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gdzhdsmvb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gslmlcerw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/grogzrmrl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gnudxcigi.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gswbngqbu.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gaqgjepfm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gyfvhbrqo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gtguljutd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gfjeksmzw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gxpeyzfrm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/glixbguil.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gdisuausr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gwnrazkwr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gfuhdotid.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/giaqcscqt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gvwxhotef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/genyutonn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/glqevwwvo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnlwktvgs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gvxzkizaz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gnydtqxzc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gypxlzvlw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gvgstdamg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gzmfsakrc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gwfavfopb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gurxzcwns.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gkfewrdwa.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gpofzipcp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/grpcovpiq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gymrlxqlz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/grnfpagkh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gomfuvhzg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gqnzkkbjb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gvhwdkhiq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gtgwdnftb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gfiexvrjy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gmrmzamlv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gxccxgcpp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gnkyclvzi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/guiqrcpvt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gaoomgbth.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gbuxityfw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/glwnacmef.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gvxmlwfyb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gcwookpww.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gcsvrcnda.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gvpcqohtt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gxizdifxr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gczlhsoqz.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/glknhxuhv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gzhkgrcqy.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gmsflqifs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gsytccyms.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/goaxpzufd.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gnzkxqjvx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gxjojorlh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gnejnhgpz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gxlbsnqux.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ggnqqqpju.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdwfwvzys.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gjyqypebb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gltuqbukk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gmdjcxfdj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gdwfwklby.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/giiiiwgwu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbiplnz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/ggnspwtrz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gvyhvgasi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gmnantuwj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gjztfcllo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gcsnfjbwp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gvvhaydee.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqzgevojb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gijlyipuy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqpufismq.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gljdkyibn.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/glaxldlqy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ghcquzbwn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gyonqyhjp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gjxloaegc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/goysfkfzc.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gkkpmvovj.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gspqkjifw.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gzcdlntfd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ghecdlivx.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gscqqsvpm.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gyeyjrwny.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/ggpwevhuh.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/glzcyzuqq.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gvwuijghd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gizdvqomf.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gfrbkvflf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gpxdpclwp.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gqeufczbm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gpnzwqxjf.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gtbcuhpof.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/geusdvhxs.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gtzmjwnwj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gkffafjur.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gjmgknoyp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gaeyudyhv.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gdjujfghf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gwpddqfgs.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gfeoqqckt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/glcwanofy.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gitkstihf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gchbpycuh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gmgwkiafb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/ggggqixsp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gdtkihshx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gbodnwgps.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gjmeiccei.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gqnhzvrqk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/ggqtanumt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gotomvghu.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gxguyybac.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggdomobip.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ghvfkgwrc.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/glgsyvoyx.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gfjsxjaqi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gzzpjhpxa.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gjdyowwly.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gwvokjnam.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gekfanphk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/ggxrienkt.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gkdohmjwy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gknrstldq.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gstxohpmj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gtrzhgmzs.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gxnirlyrg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gigwltsmx.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/ghajwyrvj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/guxqzkeab.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gdcpvmtbm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzjcghccc.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gbevodkds.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gqkbhmyyi.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxofhkg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbkvvqwyg.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gkrtlqqca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkkurlben.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gcoipsfmw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvbhyjcrf.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gyrfxrcqe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghdcwlfak.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gbuvxprsx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjijrrahq.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/ghjfivcrf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gaipjvfpa.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggvsfriap.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gnuawxsya.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gbpgzrmcp.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gghtxehzk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gqujavgrt.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gylgaeijx.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/girbsjxlh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gknvsibvm.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfepoplfl.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gukzfeluk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gahhoekco.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gyogsawsa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gdncleaiq.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/ghdgyaqok.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gjasmjvym.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gkaibwiel.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gllgmguai.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gubvwophu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gkjzntsyw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gigzgsefx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gnlkazdqz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gdvncjnji.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gxeicevox.sHtML


<!-- 参考信息 -->