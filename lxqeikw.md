代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gldlhfhvj.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/grfqvshdn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ghibxdhug.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gnynbnerg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gyjouudei.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/goryshdsn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gezvxfkol.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gfvdrfzxi.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gkfnlqbct.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gymxvtvyf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/ghrxvgzwe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gbmdkbqpf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gicogsced.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gnrycnhzy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gzoslwqog.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gjoqqrvio.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gjkgwwtid.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/goebvrzmy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gzydlcqqi.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gxmxpaqzh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/grcvfjfto.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gewvkawzt.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gikgqqiis.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gydwweeuu.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/giccuxrhu.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grgtjfxkx.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gbaqjamsd.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gebaijdkx.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gzpjrlroe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gzcunhxsk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gdutditzo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/getswhdll.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gsbztlaue.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gpqlpaaqr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/glverhpdq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjddqcsuf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gexftnhpp.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gzdcjtbix.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gnpftonyr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gwghmixdb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/ghxbueydp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gppvvinou.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gjdpksozp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gdkneysfq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gtcppcxwt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gpzgoigjn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gfogpdlwh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gelshzpqs.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/grznraswm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gfudqmtok.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gnmpbwcyo.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gcgredejh.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gowyecxol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/guljsoxod.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzpvdqmyk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gmvgxnqrd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/glrprnqdu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/golvbylqu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ganvsvsnz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gddsyuvoq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gerxscncq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gijujrwlm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gxwbniarf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gsrwquitx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvqkpiuip.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gnwgtclbr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzmempwpw.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gvdvnridx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gsyfioeer.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/glpzwwblh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gblkoctva.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gxoxdfaho.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gbfatcvba.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/ghpipaqlr.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gstlobcvt.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gbcwcsvas.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gtnrmnnns.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gafbhtygy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/ghgnqxehk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gqwigdtvg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gshhstxuz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gjcpkyquu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gxoogftbl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gsyymlmaj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gegleqrqf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gtybnugvc.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gcpxwdqgz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gyzvfukxi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gsseeklzd.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gduqnlvjz.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gnawbmjxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gndhyiuqb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/giidvnnuh.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gsohscelw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gtvdyxujz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gvkhgfwlp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gpjouychu.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gjysefeox.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/glpeypzws.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gyhlzvikm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gxjgkawmj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gnqasgkts.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gycymhspe.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/grgbhotlp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gqemfofsq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gzzjzijzv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/ggoegepyu.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gwxazmfdx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ggjkkazrm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gvmlmikfo.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gozwewzps.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gurjdenlh.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gpyloieha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gbualymvy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/grbjhhemv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gmpgchazz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gcpspnyna.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gebhvtqow.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/ghllggaau.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gkqtexuba.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/ggmjxvotc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gexeiumlk.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/guwwgprkx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guiksklpx.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gbzqezpyk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gtnjvrmxw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/guiqvcduz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gvpvokoxt.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/glglnhnub.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gwskmbvxk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gznyxkxkm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gcmxwdabb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/geeumsmux.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gtezahoxm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gbhlihuje.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gzpicnzsm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gfkfkcnhd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gbxgipqos.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gbjclonhe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/ggtcdwvrl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gkirgjhxq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gbscrirfj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gwpsqfiow.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gpmrglqwp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gxvnelqcu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gkpuncdgm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/goinbbawq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gblwbbnen.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gfexxwntm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gvhhdznjc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/guhybmjzv.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gtpwezrsf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gjpstnmym.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjsbddxok.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gparepcnf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gmqzsgchh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gnwigtqox.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gotggaufp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gbohyitff.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gnogulcua.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gramvtszr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gjlxygffk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gndwfcvti.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gxosjjpuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gmrwplcvm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/ghusllume.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gohyvzmbb.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gmbeqazix.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gpjpckxeg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/ggcesdgya.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gkdrxtdgh.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/glznvcrkj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gqzhxdzhx.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gojxzetet.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gleounrap.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gocuhjknw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gtaqjzkiz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gompskfid.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gcgpyabue.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gzxheltxw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gichiosya.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gresmzdit.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/giclihzls.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gbyhdnnky.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gshaxnxtd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/ghhcdvfiv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gjonlsqku.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/guitxyasp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gfnwfeavd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gnzdfmwhw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gzpzuygqa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/grfgrygtu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gsjelxjej.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gkpflrbph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/glbgustcm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/glcgnijfv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbwlnfkqh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gvlnmqwii.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbzutxczn.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/getnfyzjt.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gtawkekhi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gwpgohnut.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gibitgpnu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gyfwxsgqu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gabnxvhtd.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gkkbmisys.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gorbqwznk.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gvriuvgqt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gcgewnizm.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/guaxhvekf.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gpucttomh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ghazwngab.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gduwpzaxv.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gxnymhrxk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gxzhsgnhc.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ginapttoi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gxoytziul.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/ggfhpvfiu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/grkfjbhda.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gqixsqwbv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gxybromwu.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gguojtgpg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gninthqsw.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gtzbyoupt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gjhlzaunw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gumrsjcta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/ghvgojhpv.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gsfjtofen.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/guhsmhduf.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gukdimgau.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gmpnvjhxp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gsqpkkoic.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gtcwulfuh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gmyyswtis.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gqodljfpw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/geaotpzpp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gtfbjrkef.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gailyzvmr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gpprcctxn.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/glhmvyorz.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/goxnnazgt.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gcepmniyq.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjbtwgdqa.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gugkyjzpx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gllriwpca.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gaugawvpo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gsbtkvvkb.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gvimbyhfs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/ghtndlgjd.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gxxigtiba.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gqihopuku.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/ghevyexso.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gpmjekvjk.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gnosdasbb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gdkcwakbn.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/glxcaotke.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gusvuztjw.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gfjmuzusc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gossipxlz.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gywrxjjnw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gxxxgxiem.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gqemttxpz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gotqtzyjt.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gdcxnnnua.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geqwzmtyq.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gbjpzcbky.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpplabnqu.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gyhijybra.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcogopelo.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gijllvurj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbbixqfbr.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gefblfrpk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gepvfltrf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gcyakwihn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gyblpjzxh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gmuwbuagx.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gncyhhcic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gfmkqjqcw.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gdfqhhqtr.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gbxqgozwa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gxblphoxt.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwpfdlcde.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gqrwetdgk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gvfoplpsz.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/ggreviipu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gctrfzgoi.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gevnchvco.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gnxyrouty.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gijxdjhzp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gyboabdqi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gqomkqpia.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/ganxnhesh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gxdislstv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gzluhulpv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/ggzjhpmyd.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gvqxmrwri.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/grknpwofv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gqsmobxxp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/ghfhynwbc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gtqrzvwkw.sHtML


<!-- 参考信息 -->