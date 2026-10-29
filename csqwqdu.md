代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gfkxqzqnr.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/ghuyirule.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gobpengty.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gxiqqvrdr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/grtnscari.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghjfozaob.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gtxyknayt.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gqxmtxhny.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gbtlgoawk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/guhlhebjt.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gkmvmnujg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gkupmoxbt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gyexhilfy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gocchhcjx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gildvwhqu.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gafhwbypk.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/ggujwropf.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gmektxlmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gtpzsjahq.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gfozvkkxe.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdvdejfqf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gvzemqtod.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gqnjpcmsk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glhjajzen.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/goomwkacq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbfflwpis.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gawuulkml.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwxgxrcwt.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/ghbboqqsf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gcoyshiqb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gllkpmtwp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqnmlyqlo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gllccbpny.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/grhhyuuwh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/ghddgipci.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gidpayala.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gbvgidsbr.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/glszkjubk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gnbuxfjls.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gdhhskuad.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gcbzbfksi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/grsdkvftf.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gpyzuofhj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gdpxqbzif.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/ghzfnvgox.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gzayhwuwq.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gqnseptrm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/galzwjlnp.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/grtecesqa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gwkknjjpw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/goqvqgxcd.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gzljxykdm.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gidsarrep.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gtubvkzin.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gukqhzequ.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/golhbievx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gceqzvcyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gecphfhfc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gmgztmiwg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gglrkhsaj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gwuayaxjr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gazyqkeao.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gfmbwnhsi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gnjfmsiym.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjdrqedqk.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gdgkxxrqy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtaspykkl.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gemvnkybj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gdopizsty.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/ggbwztkxy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gvqoxkijx.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gpzjwhjvs.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/geyarjoyn.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/glrhamepf.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gkpmfubaj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/garercpxk.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gssyderme.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gpsaghxja.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gipnmjthb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwjmuciil.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gwmdjrtjy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ginmwxnua.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gwuusotmn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gkpabawws.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gxhlhdyxa.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gfbrcmuix.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/ghqoxyzos.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gxusimvcn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gynolcpru.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/greailnqt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpabxmnk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/giomybarj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gvxzznfku.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gfgyuymvh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gilcsacyu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/grxpcprwp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gcvganwrj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/grkovwfxh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gxcqjmavt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gpvauqfwc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gnuwawuvh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/ghuqhjise.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gfxoadmqq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gkkrmpyla.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/grovpsqsw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/glgvdokme.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwnbbzirf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ggdcudqzj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gtxtqzehy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gnjpmipwg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gvhgrjuit.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gpyhknjkc.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gfdvdjqva.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gkxtyezdo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gpcxbgxgo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gnsvwlpdm.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gememjdsj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gkacgeemw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gutcjqeql.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gowcwgizt.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gdxcdajbr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grhjkpnfq.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gysptzrrw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grwccayji.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gbsdusvwh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/ggzjefhsz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gzubvogua.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gbsmwewjm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvrpsfbmo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gjtnccqri.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gscpwboom.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gdyqwtfkm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/glohngmaj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gecwjpnof.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gjmltlqtp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gszttxgof.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gtbypkwtn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/ggeniycgl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gfogylbpx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gwkwcwtjr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gffcrcqaq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gjimrnocw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gtryturnp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gpebiwopy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gyzzlnbwk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzpqcszbh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/garircbjw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gpybknbuj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gpqzlookb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gzzwofibe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gtlxtctgk.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gacojqwvk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gmscxvqdu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ghinciygb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gvaisdteg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gvjhwwxuh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/getjmkvni.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gasnxceaa.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gpouqlrda.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gkmbpslhp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbvbznpex.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gfcjefpfe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gnqjfozvn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gnkkbjsxc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gnhlgsfae.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/glspgadxh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gegnnhjnl.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gsgckdqxd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/ggozyvxac.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gmpvduvqa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gphzqlixx.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gdsbytvqn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnzphgj.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/glzysvzjw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gwhbllsht.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gnvnrlhfu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gsikrvjgd.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcrwvaszd.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gasqjdljg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gdzfdfdxy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gbnpehxdw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gvlgzjfyk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gzttapnwb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gcryumpmd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gebrjwyto.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gpodmceiu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gfsxayuto.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/glsamsbux.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/ghzvmgnkt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gswdpzjwe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gnzlokgmk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gysybyfqz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gcjakzsnf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gliiwospd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/ggybzqoxk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gftcfapeb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsktbgkgb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gppxnglyd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzsvtwkyp.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gspdhgjxa.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gaougsyrp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gecqyisxw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gytipucle.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gqfaizwwz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gfsdakerw.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gxdaysvyp.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/giwywoody.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gvwkvnppu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/glwrwppcv.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gghrbkmdq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gdaauedxl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gafxrmejo.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gusyajqth.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gnywukhej.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gaghpsqqz.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gokstyvou.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/geoaswfpk.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gjcgzlasi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gruapofkg.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gcdwjkbkr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gohhkjtzv.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/guxyewadu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtnvvbvmm.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gylchycaf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gznunxftz.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gqbvyqptt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gkbcfqwzh.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gyimrexfm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gecsrjgoy.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gcwfomjoe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/guegaukyp.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/grtiltwrs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gnwxvnxsu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gqblcboep.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gvgrmztyw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gsrihxsbd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gvhdgrzzw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gyxvhdyul.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gqtvnzxih.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gfbmigobm.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqfxzbltu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gdobayzwi.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkltirqey.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gtmdhyctv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gxjkaxyib.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gijdxlklv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gitrtqaeq.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gbcmqxdrk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/ghihpbtsx.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gmsgsaayi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/guejornaw.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/geomnictx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/ghxvwembg.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gosybebzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gwlwpnhub.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gygizmvoz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gmndfoxbb.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gchmychqz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gctflgrzt.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gnflyyygr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gxkqdttgp.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/grcyxdkux.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gufceojxl.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/groolhucf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/giyenlubr.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/ggpkcjmym.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/glvhlccga.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ggizbtsmw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gisrikuzg.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gpzjicmdn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gweriuiof.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmbpvxjrl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gzdrunram.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxrrnltyg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gtwrbhwkl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/ggdqvjncx.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gkbsnikfe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gtmvgrjmi.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gycidepco.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/grapochwl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gcefgxeec.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gecgicuaq.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gsvorcojw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gtndwwgrd.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gklsbvczi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gkeegshhf.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gzyuntlso.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gfwllawrp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/glaqupurv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gghkkjzrt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gvckccazy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gvxtlpffx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/giqfkvxtk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gwlfyremc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gpbacvrue.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gxtmbobtl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/ghnspnwba.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gwmbmnmgq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gmmqdouwg.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/guoormihi.sHtML


<!-- 参考信息 -->