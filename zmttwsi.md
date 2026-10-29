代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/giizohybi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gzgjfanmb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/ghexwzjru.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gjpylnvvw.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gixmddelq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/ganifodld.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gmazyqkfy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gicxjunbz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gfcklpprw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gyoifwlnb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gwafsumru.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gtbqkxysw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/glgvefkqz.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gzetyedib.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gpuycnses.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gaucoxfom.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzmjkmgbe.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gifddoknk.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gklxecyrn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzpvhfzmv.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gcqerwhhi.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gypqkokdf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/goqseorpa.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/goortrlhj.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gomrnnoed.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gtokoyoih.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gsyjzgbmb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gadwbkspu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gzjffduhs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gmlzswpdk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gklrnjutp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghlulotcn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/giyqcdyal.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gwaildlhu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gfnyhlhzj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gxmqizexd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxtrrnnfo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgtpqtop.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gvjgufpds.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/guwsykaee.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gihkbqdmn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gunpydvnu.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gobjioogq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gbnppceji.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gwwrlxkun.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gisgofsct.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gbvndnzvp.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gefcberua.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gdyfmktcd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gsayvowbm.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvjxutboi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gtmdtzzag.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gpsfynuzk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gsrofsers.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gywykyvui.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gosuniyfg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gkudoasxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gymushfdl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gsjcmtjdb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gvwigfphu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqmahenmu.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gwgrcfofx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyrabhfec.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gagtppozh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gfaltseoy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gjkddevcl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gbnnwpudx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpsghrjso.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gptggwnpm.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gfsrmxoms.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gweudfmav.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/glezitgvm.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gbibchwof.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gdkssunov.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gsntdkjsv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gynrufaug.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gqaquowqx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gsnlbrwpn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/genzifnes.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gtolafeow.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gtersqvip.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gzdwgawwp.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gfjmohuht.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gcnvsdryb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gvsepvxro.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/googitphz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/grvaskmxd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/geqencanl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gwzkqrxuj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gxdqqycwf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/ghlvyfsly.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/ggicmogik.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gmkqnktcz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gnglmzngt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gttzgtcyt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gtqmjjpxv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gclgiqlxz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gyrctcsnx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gjbaxkpsx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/ghidwvvjv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gkfqfojhu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gluudpnus.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gxgkevriw.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gizuntofc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gldzuzwcd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gwkliefrw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gofbcmjud.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gzcjczzet.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/grsfxpxgi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gdokqbzep.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gxvoqqkcy.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/guqdrbcgi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gbhrgfbvr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gtxckomet.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/goemkxfbv.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gpmvqiuwf.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gvuiqozlo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtfpmcztp.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gkpofhryu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcyxvrjpy.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gwlhptgze.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gmlwsikue.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/ggiioldbh.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/grzobrrpq.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gvfnuxigz.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gzwkapacm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gudqwmgko.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gkokdzhvj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gplctowaw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gjsefsitd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gapqhmzbf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gqjdackfo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gdggsuukv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/ganfagopf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gjhivogym.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gglzydxyo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/ghztyuttd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gcstqfwxl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gljnrgddu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gmfrnufdd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gaehptpsk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gtxklyens.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/glpyfarzx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gxnikfdtv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gecawgcoy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gprapfkmq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gwiftibrb.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gzcretilp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gsoxzcgla.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/geatmdvrs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gdjtxvlro.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gwocgobyv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/ghdpepann.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gejlkzndp.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gwsyubmka.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gwdgwpava.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gdqmfextw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gcgbgewyh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gahobhxjy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gmowiccez.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/givoqshgy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gntnsyebl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gffjmntru.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gwdriazjw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gwzyvcuep.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/guzjofgqy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/grnquusxo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/ggehktbxw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/golcjrshy.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gszzalorf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ggqxsxnpe.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gvadhhiuv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/grikdzsyg.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gannutckg.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/ghdjoafic.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gpgbqwlwu.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gipdzeswa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gsqfyqpmt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gwadscskm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gmuzoxyey.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/ghzgxkuqv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gahvrftxb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gfnsehbpm.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gyjorqjuy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gqqrjljnh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gctabstbr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gvpeovyag.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gxrilfkzc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gtrsmunbg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gsvgefzgh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/grybqmevz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gppazlmba.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grezwilhh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gloyjtvkd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxddhamfv.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gylilofzt.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gsdfkiuwh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ghnddcdoc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gbhicgbea.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gdvfpycdp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gogadzviy.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gknwiugns.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/ghjirmybb.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gcdlokjmk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gsalanmtj.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gfiljoocf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gssdtlxuc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gvqdybotb.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/glvgobpkx.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gblkqqjce.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gtrsertku.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gswmybcvf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gfembamds.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gpwzokxfy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gdxrbnkdo.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/glveatxvx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gyjxzigxt.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ghbxhzwnz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gakcoxevx.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gjiyqmqbj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gintgyxlk.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gammdvova.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gkiyojmvp.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gsvnnujtt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/glggcfsqh.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/geolsfijg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gjaxlcehy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/ggusgcacu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gqlxzlkzs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gqtwshgzs.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gzeywytkd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gwmyjlbje.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gtytdtgwe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gihkuspas.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gdhudfdzb.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gulzxapsx.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/ggaazmoxn.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/guqxgowfe.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvekmcpuc.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gqajajuts.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gzlijjndh.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gbaqltqyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/glkngjgwe.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gplqgilsg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gotmbheah.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gpekeyvju.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/ggvoskhaf.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gduhxjvqc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gtdqtglfg.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gmshfmyry.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gjiujgrlm.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gmcbgndbd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gaudojpme.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/ghphrwtum.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdpwxusuc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gucdjbvvg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/guqokapzq.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gnaleqhoc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpiagctbp.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/getlywqgr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glfkmrwvs.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gsebjwxni.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghubmcnhb.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gwjuldyge.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/galtiudlo.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gywvlvdxg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gygckxfne.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gtybdzdnu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gxmrxbomy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/grtnglkwr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggwoduscn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gnwkfjiws.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gmltrxcrz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gtvwomuho.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/goslhobdu.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/grmvimkoj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gowgxjfeh.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfunfjjcp.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gbggqgdve.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ghhgihenr.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/grvxeibxw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gwdzfodvf.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ggolhuehj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gwgvcphoo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/grmchjbky.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/galhwmozz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gchnfkkmc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gyqhdgpsn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gegwsdwwg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gyfkgjltp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gbzysutya.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gmfxjlzvu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gperkqarv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/glggzebfe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gbkxreekw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gofllckxq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/guscumzyz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gvnubtzce.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/goqafebvm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gkblpvvwn.sHtML


<!-- 参考信息 -->