代发 wailian999

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gjsoqejgd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gzafvicnd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gqdoczomh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/grwinlscv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/ghdumkyei.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gbalocyhy.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gxvjxupei.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/grzgebecx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gecxcrmrf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gcikfadai.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gkwrjztcv.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/geakkxmfa.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gvzslkecz.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gkcblslzq.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzakzreil.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/giptltlzp.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkhopuxkt.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvygprlnd.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gwpiqheeb.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/govzwjgbn.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gruelfveq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gkpplcrfr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gasiikvmg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gpgxlijir.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gwsstrxmr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/giospfiya.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gmzaxkobr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/grjadxbma.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gayqichta.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gsujxbjwt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gomnbwaaq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gengsufvp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gwrzksips.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gsbmkjfzo.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gacwxivup.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gcipmpoxt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gugfsodjt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gorsnxfbv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/ggttelcpw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gdyuwuzhy.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gqdzhglvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggesqhwed.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gvkxuklcw.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gzajsymie.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxldcrgcn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gyvuwqtnf.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/grbmcsohw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gxywfwyer.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gadcmimkw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gbpymfvsg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/grfgpedbc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gxdcfcife.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gpmshynsl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/grfrjeqem.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/geaspmywd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gutvwtbbr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzvhzkqnt.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gtspcetxk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gawolwoiw.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gkpncwtdk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gqwnpcfst.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/grwqmtspy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gdtmgpeid.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gblctlifv.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gokseavgd.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gnqogcmuh.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/glboolftl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/giyoyyvqj.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gaqcwveod.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gerbmstci.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gdzlpxrpp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gstgcrype.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gcelgkoue.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ghxifccqt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/ggtprffyu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/ggoozmzww.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/geveobxod.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/grpuzgrff.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/godvuplet.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gyusnilva.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/goabrkdon.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gmmalrdum.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gfdmlmete.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gmeytpent.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gjrpauezh.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gxahypvqv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gpgdhxsyv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gzremrljq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gebqrpjvj.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/goanisayl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqrguypft.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/ggjjnpvic.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gbcrtmwvt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gssedlycv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gwweryfbz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gfwxdcdty.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gfwfgztfu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/grlyojety.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gjwbegkfn.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/garpqspar.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gutgmjpst.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/grohfvevm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/goszzmikm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gijzfzgex.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gdemdnscc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/grykymevx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gddfnwosa.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/geahiiygk.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gpnmcfqmj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gcaephevm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gltqntgaj.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gdpgxejgd.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/giuqzzuzs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzrmtnnne.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gfenvyzde.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/golewsray.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gvalzlkjf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gusmgxxol.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/golfouejs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gbtlscgdg.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gtcrsgmqo.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/glpqqdkca.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gwilpwmsz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gphrsylxx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gicmojzgm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gmmuvjenn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gezwzcvlq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gbejaxtot.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gzgpbnslb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/glynyoaym.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gfqceesfx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcxxavysv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gzrigdzhb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gzgwlknic.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/geqjtkdtq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gnszhyocj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/glgdctuez.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gntfoptph.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gbisegqdu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gqppwmthl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gdzzcuwes.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gnxyvvclj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/ghrrcrhfi.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/grclzclpn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gqsvvgxji.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghmmultfv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gwphuizts.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gvvhwbjtf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/ghkouhnov.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gxwudnbdg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gvrpqanpu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gzjqwapbq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gvvhambes.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gflejmark.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gceephbbk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/ggxvluzda.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gqgshprex.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gytcqcmku.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/glrvknpjd.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gbyqnwaxp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gewcywkis.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gfwnwgflp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gfqrxvtzt.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gthgciftp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gqadfiyne.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gwfunrpoh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/grmsiesie.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gmqvmlhrq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gqribqxze.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/ggrbjvebr.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/goeiikqoj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gxdtvtuxt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/grcjuxduk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbubbyzbs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmkofbavq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gnjcvmyfl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/guunmjcvf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gadizsxhi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/glcbaoeno.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/ghgkfsvsn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gpyaedxyi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaihinjxx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gxmfjrnqu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gaxdxodpf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gmokktrof.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gmedjjmzw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/goavcxakw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gyavhalja.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grwnwqnln.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gvtvlqafh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzkicxazz.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/glxowkaxb.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/grxkpqrxn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gnbtlfyhz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/glwpcvlpk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gwtsheckc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gemsvdaic.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gvtogpfph.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gxpffrdqr.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gbufrusut.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqoaigmkl.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gvuurdvtv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gfywjwjuf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gnieoxvqh.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gpsrlrfde.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/ghjnpdflt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gmmiigunf.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gakxdgvpz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gzqzkngpw.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gquivpnhx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/ggllpoyiw.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/grswtbzli.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gucnhttsp.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gousvdwlx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gxopkoygw.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gexbfoqcp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gxcljqoqn.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gsedvksiv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gmscunkir.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/grnrhezak.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/guhtgbfxw.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/glkdgjjha.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwinyuhoa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gliudttdh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gwlzerkrp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/ghfrqtlrc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gzknbidhx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gzmjdriwo.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gyjzxkhsn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gnekjhklz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/ggpfbmkoh.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/grgeqmnrr.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkkmkjdoc.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gtymadsad.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkbijrpoh.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gbsbkgjdg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gjbglrrvm.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gnvjktzxp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gvxikluci.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gdcerjuhb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gxnxbkoxa.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gxzdfgzez.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gzjzngzpn.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gamygvlql.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/givveevku.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gqiinkakf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/grdgncwiy.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gctqgtccx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gcshicjtp.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/galcowinq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqruvxzpo.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gdgzfhbdh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gmpckxbhg.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/guqrfysiq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdcaqaivg.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gfdzgucvi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpbjhszeq.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gnutyauug.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcbdhxnof.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gimddcsll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gudcfgaja.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gatfcrdmv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gghbaihyn.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gdtxqpcbf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gyjmgbhfk.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqfdaphku.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gdsmhvzba.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gnevjiavu.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gweaxbygs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gmrjswiru.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gpexblkcc.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gkjwqkrde.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/guydwuevt.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdfylhzup.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gugkintrr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gloizkkwt.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gkhtscqrq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/grgfhzlyu.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gjumuljrc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gsnaibyaq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gufttlrbs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvofytfbu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gdufkoqcp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gosigmbxo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/ghzygzlwz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gadxmztvn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gfcwvsoyz.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gbkjlkdlq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gabyvtsdk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gsubvfhag.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/grtsamybx.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/glrhipgcd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gjqvaeivm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gpypuyajg.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gjhlsdaqq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gsyqalqch.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gpsohwgxz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/grmnyahdx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gqeqlnmdg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gzuocgzfq.sHtML


<!-- 参考信息 -->