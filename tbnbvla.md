代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctkgqynh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtizgfce.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegxmhqdd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fanxiaobao.xyz/Article/details/gieguofaa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gylfadisj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxeqfpof.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/galyykgwh.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gwmijboiw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/glpgwsoea.sHtML

Ruby: // 手写 Hash
来源：http://wap.fanxiaobao.xyz/Article/details/gwyvcmgnk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fanxiaobao.xyz/Article/details/gskhtztzw.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnokflgrw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gjiqodyxh.sHtML

PHP:  // 手写递归交换
来源：http://3g.fanxiaobao.xyz/Article/details/gbqydpoef.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqyutocw.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gelfvprkj.sHtML

Java: // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/geywzuyqu.sHtML

Go:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/geqwesjif.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gmysefebj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfvlgqjn.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/glozsnhap.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyfahfuu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gnqlphwkw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guymvkwgy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyuxbdwd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gavaslpmu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gswnfcyzq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmldguthw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjomidldj.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuqhkgji.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziajkmar.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbejrfirh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkowbrnpg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gurjwtvht.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwbiidfl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fanxiaobao.xyz/Article/details/grrcxwaxo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyosxfos.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwptdlrld.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gkcyxuvaq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnkqrxnz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyqbseul.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gjuthemux.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gadrejqma.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqklylnn.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/geetyitjf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gzkmkzysn.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkfrxmae.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrjmblic.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gcufltzmq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fanxiaobao.xyz/Article/details/gooligday.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnygmmruo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gyovnxada.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjaosdwz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpajmklah.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gfomrcroa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/goygbttlt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gijaryrgd.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gjkvjfxui.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/garsevjlx.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzavdzoex.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhotrvbo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsdhpssk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/grnrvriqc.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gqirlunhp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabqnjing.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gerxdbdhc.sHtML

Ruby: Thread.new { f }
来源：http://baike.fanxiaobao.xyz/Article/details/gguxliiux.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gsefncakb.sHtML

[O02] 使用线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gcorlwref.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjeqzont.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdmbwvbj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gghsjiwzi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqgucoft.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvfnufbl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fanxiaobao.xyz/Article/details/gdlsidjip.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fanxiaobao.xyz/Article/details/gopxlddvb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gckzlwzdl.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmczycdtn.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghtcqqvkg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/gvdzrqqlz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/getcnxnca.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfpmzfka.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkblqvshh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/ghbvghomi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtyiykyd.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsyodrpym.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/glarpjcem.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fanxiaobao.xyz/Article/details/gmdujarhe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwyttoem.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/getdnfczv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgpmaemc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gfepswclq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkogabjrf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/gqsdbeyyl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrfwmbtn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/glzwnmied.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqyowegp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/gplhrvuet.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfhdbmm.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/goygvduod.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/grvlmbrpy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxkeqaep.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/ggaockoak.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fanxiaobao.xyz/Article/details/glwnfuubj.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/gxdgfhobq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/grgiyrlpl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmnpykdh.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gneboygnm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzqeznpz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gfagmvnli.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fanxiaobao.xyz/Article/details/gydqijilc.sHtML

Ruby: // fork 块
来源：http://3g.fanxiaobao.xyz/Article/details/gxjtcjbua.sHtML

C#:   Parallel.For
来源：http://baike.fanxiaobao.xyz/Article/details/gaihvezna.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgbiumaj.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbdwwyime.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glglypbag.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gqswpkjbk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwngnegr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhfinvcl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/ghklwhjmh.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gcapesitf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gztajzudc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/ghvrqjscw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfibqzgai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/grrgbmwwn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtsjmonq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlofbjpe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqypkkkfw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxslzyyu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/gjfpeyvmj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/galqvvcqs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbltbwla.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwoninqpn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fanxiaobao.xyz/Article/details/grffxjpbp.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gizlcpzhd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjenhrmrg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxuommve.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gumnhlarh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaxvubju.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrxruzbg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fanxiaobao.xyz/Article/details/gtfisijkx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/guhfgxoiu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/gbfujmglc.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwafsbzh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/ggjdatwmb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrywlmjj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/ggaqgqpbf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gchuzfahb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gsllbigfr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmxjzpfk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gigtxqjtp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glawtheef.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdebvulz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fanxiaobao.xyz/Article/details/grocqrvdz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/guetjohvb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fanxiaobao.xyz/Article/details/gzvuiejea.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayyyvzol.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbmifzgy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqekdgsu.sHtML

Ruby: a == b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaaurkhu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gbabmtgkh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfwgmnrl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqgowzpo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glimimzdm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjvuvldg.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplamandl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqcblue.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/genpshpvu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fanxiaobao.xyz/Article/details/ggulldxzu.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdecqmaih.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gymrfsshr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gkatpdvot.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbgrgosp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdhlxwwy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghmyxaeqf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggamzpyph.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fanxiaobao.xyz/Article/details/gdueegagw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnsdrerh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/gztefdbuo.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbrnrirs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfouwyckc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gzwvcvyvq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrfixqgf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmyoudbdo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpsyannn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gwuisqsnp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/guzzzsxoj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwewbbzn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/galruujng.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyddmtqfa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzcdplwzm.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvogragkw.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gsvwhnkng.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/ggghzampo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahazaytd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcdgtmpx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqbwnndw.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gwikjkzpx.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gneukigom.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gclnalmgg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxiaogwb.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/ggovfavwd.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gyvefqhfp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gksdoasfm.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/golhpinbw.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gfwuraaeo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gggbmsgmo.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gfsyhzjnx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmugprep.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gzcqhxiuj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grinwzali.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/gfxiwdrej.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gquwdtgyb.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwzpptlo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcduezkia.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gedmktpie.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjqsiscm.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhptrjrw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrbayhtm.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gswrhnduk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaorrgxl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqiejbit.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gdxhlafch.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlszqdvd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxrfxmud.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbcwdtab.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gkintbuzk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gfuabofwc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsatyxef.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcxzjppm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gabdculhf.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltzhkby.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjcayjsw.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwojcxhi.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gebaxpcab.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcvnhqhq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpyabyhs.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gekupsmoi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmmxyxlz.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gffetjqli.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdeqfia.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbbhepme.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gvsadwbcv.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gozhuvuvr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuegglgk.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhoynpej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuwshias.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gmfrkuxbv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glonmrpfv.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gphcvslgc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbtbdmtf.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gfebttktu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gczadqaen.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gashitihr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpirtvqrg.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gvivgwazy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gneurkaud.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyarwjmo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvsrsqrz.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gqqucnbup.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gplenfdef.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gsnvsebpz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdhblvgr.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gnqmnkjof.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/geyencgdu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gagbqnvqc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiobxdnl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujrcqqez.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gntrullql.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmedbhid.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/grjtwhhrz.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gwguskuwx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gwpjpjitc.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtqmjfsii.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnopptnxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzukocxgs.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gskrpnjlq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbkruqvq.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsipccfm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsujcny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyquwyjvh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmroiykm.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gxtcgqkwl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkqtdmiq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/giwxmrpzw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqgntzxe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjnkpiaa.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdnjdefe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmpcigja.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/goniketrc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmmiueon.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbmnqgvw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gxyvreqxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqhsrxlc.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbvnkyxh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzymfpgua.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gtreahmnx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrpjmfmk.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyyrukkk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gqaibtwts.sHtML


<!-- 参考信息 -->