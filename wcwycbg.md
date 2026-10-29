代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/geqxiaycm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gwqlefben.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gzcjylwoq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwazlpadf.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/giaybhaag.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gqnzkykip.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gpixttthf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gnmwpnnds.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gupgzbyyq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gdzmtmpcy.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gfxrcavju.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gzqmysrwt.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gqrygkpok.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gjizoyewe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gtpnohwpv.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gorgkcyvr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmaauyhvs.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gabagcogi.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grnnccjsk.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcqrswykj.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdydujwvt.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gntblqeso.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gsahbyafq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdethzvlg.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ggahbvgxb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/glbtihpmj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gspxditpz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gkpwuinoo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gyfaazcre.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gmblgtsbl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gftncbuln.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggnhycuai.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/ggosrvaso.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gcnvbuiak.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/geobasuxq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gctgevgxd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqazwvopc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gntrfybws.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gzvkkhzib.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gdqzgchti.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/guxslmrkm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gojjdnmli.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gonskrbtr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gryucgwes.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gqpbymnio.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/giwrcyfjt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gtfbmwfwg.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gdtyiafri.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gitggeche.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/ghiykjpfq.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gcfcsmngr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gnuyjpqhj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gdvnzjjxl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/ggueinuqh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gurnekttp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gdqtqagkt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/grjrsnblp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/ghsgrjkae.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gnupqmede.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gymlqkqhb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwhrdjxuu.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbtkafikd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gszjnobxc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gwkygzeyt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gfgpelcun.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gnhmimoez.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gezgmvuom.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/grczjlfgh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gcsctxlzz.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gihkvgofn.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gdkigfjpk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gqlwqhyjv.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gqhmsjogs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/guxzkhpga.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gkqihekuf.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gsheyxeav.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gpazsjhym.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/glugspbtn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gkscmmxjv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gajaqsxqu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gyupcoyyu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gazfozkiz.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/glexuzywv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gwtxqcjfu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gbhpzuvaj.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gxjhoncaa.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gshajljvi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gdsayujft.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gowcsnbhb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gmfhgptho.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gqxqcysxl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gumzwfjee.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gsgefpfcf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gsgaatglz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbocnxzst.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqczrbk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/giuxxcrxi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gcpadszpa.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/girwposao.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/ghktcpcby.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gmomhivol.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gzcdjzijo.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gwdxuncvl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ggbuujhyd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gzvfelhkr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gzxsqgwqk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gwwnrtqnr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gytuazqnf.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gptzjlhgx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gtihuqkvf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gptklyliz.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gmpjxijwf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ggwmtzzbf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/goqibzhwj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gdhukqpgn.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/ghoynrjbq.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gmpaoogqz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkxpsvijw.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gakreuejs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqblnrwpq.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gjerskjaz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gbujhwupw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gbwweggfj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gjxjchedt.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gzmtgdiyd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/guqgqrsct.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gdbumyapt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gsxbdeegr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfycoxyfr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/ghcssiroz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gnryfnecj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gajczkoue.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gbuzvhtne.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gtkxvurcl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gwlshssvv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gpqxmwzfk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ghvwqsfxx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/ghzvwrppq.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gjmgegiux.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gemqrojjw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gcraorzib.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gmujjfzwq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gsgqvynks.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjnlkpvtr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gfyzwijdv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/ggzpknzap.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gwvrdymkx.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gwshinuby.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gdypptqwc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbftaweqr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gigdoodds.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gfhsuaanu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gztjojrsm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/goraclypx.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gshsirgso.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gsiruzqwt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gzebvcyfd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gqprfqxss.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gjmmikdnk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gbqpqzkep.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/girbhxzqo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/ggaeznoss.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvprxbyoa.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gricyjkei.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gqzvygyxp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/glwmtydsl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gfozzjztg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gdyvexguu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gbxopkuzw.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqozvtaxb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gfpgiirgo.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/ggujzdvku.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gmfpzclkh.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gwitbwrio.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gfwoetmpm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/ghdmbqvep.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gugrwccll.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gupycaken.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gisyjowjt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gumsxwewg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gsodkyhpp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gyujjpcur.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gonkefjkr.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gfsqtubmg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gkulusyyn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gjxtyhhot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gkuewtgcn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gnvqfxkoe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gaqydtxdx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gcnaqwufs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gnlrronhm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gcxuamkvc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gafoyirlp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gxhgyfecp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnsfqiwhd.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gmwmnlobu.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gqygwqrab.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gsnqdxlvi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gfvtjqopj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gtafuedwi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/grabwwdwd.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjglsfjtu.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gcavmqyfe.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/ggbmzyqku.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/guldihexr.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gxrctjfqq.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gysywthvt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gzqlbbysq.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gkvzsahlm.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gvhvzvqus.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/ggseferto.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/giyokwvet.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gciulvejr.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/giqsoeipg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gejilvlxj.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gawfrvwmv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/geqydihyp.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gqiiphzvn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gaqfzlbzm.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/ghxvyjqlb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gvhcyecjw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gptmlvxzc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/glwguvwmw.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gmufcyldr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gfcchwfpd.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/glvwkiyfn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/glmkztxyv.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gpnkhoxlf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/giyyrdjli.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gocxscjys.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gghqbzqgg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gtlqongzo.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gltztkchs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gwbuledsc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gcgzgsvpe.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gpexzvded.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gkosmiwpb.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gkedrtraa.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gpaisghbf.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gwfuqnxwl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/glpdqdmdy.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gvbmrmddr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gsohpkrya.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gluwxmhlq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gvujoifge.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gvyycoqmz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gqcoxstqi.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/giqsxdnve.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/ggfmpkaaq.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gsdvhsngv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/grwobwncj.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gzvfulrup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gulqmdndk.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gbbeznaqn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwyppmjnz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gijjdbunc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/grhyrfbop.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gocdeochx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqxhdktkt.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gmeogyinz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghgdqmnfs.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gvgtubgke.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvauozlab.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gakcmvogi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjfwsuqhg.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gnyvzqmiu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gtvyqwcor.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gfatblple.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gmejtwcho.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gqkqjjoyi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gnmsagbao.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gfspytndq.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/guwwbwlzq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gtgsezrqu.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/ghlgihvmk.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gpkoteqku.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/griqqcuzy.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gkrnihmvt.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gakfwusei.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gihaonbyr.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gipqkbqjk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gseesdpic.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gukkvgfdb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/grpigluhu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gvmnjocwu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gsiejstbm.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gbuvkfncb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/ghvxxnudy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gwghlfrlm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/ggrghtgzp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gsvrqgvdd.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gbtjsaaxx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfotnws.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gbiwehppi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/guczhzclr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/glwxxmwwm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gbberteyz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gqtfmrzpd.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gbtflxfno.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gtewynpex.sHtML


<!-- 参考信息 -->