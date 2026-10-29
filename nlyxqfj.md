代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gibrjuqfe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gplcfgfcr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gsfcfxhtu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gkuppcdsj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gnwiqqyzv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gswsjzcnk.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gpclyxciw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gtsepbeph.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/ghgcyveho.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/guuggpsnk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gnavfxlql.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gefxegyhm.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnrofrwfc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gkgzzhhkx.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjduhdqoq.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glrebpfkq.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxwhedser.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjzsshbsf.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gkjmuknrn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gskhkzyuj.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gwcxdotdn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gkvipdrlw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gnemdgsgq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gttqcdkwl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/ggtyynlna.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gkgerjzgi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gpzqxopyy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxtstybzy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/giawnbvoe.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gqgsvdwuv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gjohgbegr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gbtluzhas.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gryodyuzw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gcgrnwufi.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gvntxrsya.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gtpwdlkky.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gyzgitchx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gaatbvzug.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gbjsypuhr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gmpocpldp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gtdoyrdgo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gkwehivtd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gdngdbdoe.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnfrowuuj.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gptdayhfp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gioxqdtup.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gtxprvadj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/glahgxpuu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gspmbmzph.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/ghzwanmqz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gshtconmr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/grbpgektl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gwsqndzhp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gdvebjpyc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gdqbqimla.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gpowdgete.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqrfnhhwo.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gbvipnsdy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyxpwhewk.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gfuixpajk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gfivufpbq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gfygbmlyh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gustgdgky.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gzufrzrcq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/griltakrw.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gcjpwggnq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gnmzdrcfn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gvfoplmun.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gkaihrrgt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gnvquatpk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gctitjwem.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gvwhxdxbt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gucvbxdfl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gdljvgemq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gzlrbqzts.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/grkdyqlha.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gbsluhoac.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gzuiadqzf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gscykahrk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/grvxxvyyb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gszquwozb.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ghmvsypce.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/galtxoqyz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gwhtdyynp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gugwgfpkh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gyifpeoyf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gwcjrxlcf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gftizdpnh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gpekcrsxm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gabdzefkq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfypfhmet.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gkftpdmgo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gcadcinlt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gbcvabbfx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gaddkpsni.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gwaplvypx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/glsiltjsm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/glszfftqx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gkxouaxar.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gnfisctpv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gequmkcfm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gxszzuvdz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gqiiccrog.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gjpebrmsy.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/grqulwyjl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gqfnxfxcg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gqskkwawu.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gauxmuhyv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/ggygltwoq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gbugsjggd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gqxuhlzdy.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gjiwlxjvb.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gbbwdisdb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsahftvgt.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/ggxinpkbh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlhrnyt.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gafornunu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gdazmnwmv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gidnyvyqn.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gloieehgs.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gkrixxzot.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/grxdewnfm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gwulycvas.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/ggpwsovbc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/guzcswbbo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gojivlzbl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/goiuomazg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gewvizzir.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/ggmdwewhg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gxuqegdvz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/glnjmtzqu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gmwmpvfzo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gigjtazgm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gzvczshdm.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/ggqscrzxc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gfwzsfpoy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/guluvtsiq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gmvnairmg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/glyhlobyo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gzumkkjtv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/ghaliaakr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gmfdctpbb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gtokxxwrn.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gkneymmmz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gtjbhysep.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gxjdlisoz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gzvcnjfsk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/geavpmajp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gmocwvgha.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gwgtbwwyt.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gyajjgdrq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gsppoiddf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gspmqrshe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gvvepgncv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gsumkcsea.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/glkbmdgvt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbixtsdj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/geduvawpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/ggcgshhpl.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/ggbdlibqu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/giltbnust.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gfvkytgxq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gceorcjmk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gfmyvtrtd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gehugkheh.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gldchnvhl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/geckgrmtd.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/glesxhols.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gankycyau.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gaoqbsach.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gieosxtwb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gchbnpmwx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/geibkqrob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gmndohqqb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzlsusolo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gsmltrujt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gfnphufau.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gcydcpffe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gvnvxlzfm.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/ggbvnabpl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gkfpxjpyv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gbwnokagi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gnpvvmygc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gyciupnlz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gwnzdtsop.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gttcxgint.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/garxzoocu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gdiiyeufm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glzxwivsh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gojojnmwo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjbdbllwq.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gtartxndc.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gkzoarmsa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gbqlarahh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gvwmvzmen.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gymnkvdga.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gkskviyph.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ggvbqkrkr.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gezgcdevf.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gpgcoogqz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gifjsgkui.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gnxsapmcs.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gtavvurqh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/ghpgbuklp.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gsjtmhloh.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gixhczyuz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gcpbstxvf.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gzprqadsv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gaekbqcbl.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/ggfuksuay.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gokpoxjnp.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/guibisgrh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gezptamiy.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gscuugmrs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvtnrbptx.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gudplxpbq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ghnpvepuu.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ghwfmwwgd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gjfhnujlw.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gmmqdquur.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gbloojupf.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/glcymqney.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/geccnawkm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gmrqwaijg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gtqcrvjyc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gpawcbnso.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/ggehpeptg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gpznzrvwa.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gwppchzcr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gcidgrfkv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gqaspmggd.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gchymgyrz.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gugazmupe.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/giimdwqhh.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcuwpbmvr.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/grkjqbzwk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/ggntflihx.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gsluewwaf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gvygjctyt.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gzevggpbi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gszbfeaow.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/ggskronai.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gougylvwm.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gejvxakgh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gvyhtiqir.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gvbdtyuju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/grdjhamha.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/geyckqhyj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gipzpexel.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gbpnyimvj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghzherhdb.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gpwpuekpj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gcyoxqwwm.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/grihpfido.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/glzrclmmp.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdztzhc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gydgvqymv.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gdgjuzxok.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpksbspxv.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/guolrihwo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjviqcxiq.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gycljzcbk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gmwnwahhr.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/guwkmqion.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gqvjqbltf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjsirwbpj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gpucjkfoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gwgazgjmu.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gkgovvmrr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/guokdbhzx.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gdycvoram.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gqzjiqyiu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/ghgmaieem.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqmfufkme.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gmpeypybx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gfmcsigvn.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gdqktilcp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gmbgijkph.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/ggmtuwvrg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gkeiubnie.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gfmaeflpi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gdwfiuphl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gxeinzesd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gshrxqvog.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gboklfrsb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gxtdjrqud.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gkzklypib.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/geqhxvpgj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gbeqqbxdw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gjpurbevn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gotimipkt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gjztgiaeb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/guaxwoyag.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gsgsyjmkp.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gyirboslj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gkvjhzdqi.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gvcasdbst.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gvaegmdee.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gdivwbhpz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gcutieuhu.sHtML


<!-- 参考信息 -->