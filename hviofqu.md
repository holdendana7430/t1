代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gncyafdxq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gsyhjheyt.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gcgneyqta.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gvsyhqshm.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gvtijyilo.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gdekyngql.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gowjyyuvh.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/geuuckkkd.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdgqyiruw.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gbupixkla.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnpirudya.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gcuemknup.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gutxiiwmf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmywflswh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gdswsybms.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gownvpsyv.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gbtbtkjeh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gunpzunda.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gipouoxsm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gsctnmfhj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gfwnxuirg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gqnylkjai.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gtvmwjrbv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyoxuqmsk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gjhmikeeu.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gnszstksl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gfdcinytx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbrtgquh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gcwioljzn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gbmbyziaj.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gpedirywh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gpjltefjo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gkoxpaaar.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gfpocfzvu.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/glalhtzyb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gfgotqzey.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gunnpjudp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gtkdmihfd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gccxpkobr.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gulxhddyt.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghqehnvxd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gfzckbpka.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gzwvvmsuc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gosnbsozz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gcvfrclje.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gyqbuddph.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gwswwcpje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gcjyqlyck.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gkkcywkcl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/guvncifss.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gvtxnlfdo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gxxrhvcws.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpkfcyhse.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gnnszrzht.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gphgzdwsd.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gkuoykhab.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrhnahs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gcieyaouq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gudfvnprp.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gmatwadbv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/glyawevsm.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gcgwhrhig.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gvufsoqvx.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gicpcdqur.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/guhgijwkv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/girreqivq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gvggjiprb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtjuupiap.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gdkswaujg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gtgzexcte.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gqrktfslq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gdfdyljap.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gxvppfuwn.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gsrkyjamq.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gefzkmiid.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gtceftayz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gkrlearny.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gazvsvlyq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdquodttn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gneuivbjg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gqijcnkhf.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gsbwcsoqz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gydeposdo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/glzxfbhvz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gpxkwxaml.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gqoiesdav.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gmpgxexdn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gvhhcnera.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gyuvmdzjc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gagltrlud.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gulueoaka.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gdhejetje.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gwjbpwtjy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gknznwxts.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gbsftlpby.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gamtniqlh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gsccfnvpg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gwzhnactp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/ghxcxfmuc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gvembgipg.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/grjnqkkco.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/ggflzvuoi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gsdqrurzx.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gdrouieja.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gnupbtpfr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/goatwzird.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gxapvdtiu.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gcqwpriit.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gunbjixvy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfsgoswwu.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/glyxyvrlt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glysevark.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/godfvdjor.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/ggobjovfo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/glregmkal.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gyochctjj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/garbolgco.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gspmchpxv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gqpvxwmok.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gbutbemsd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gjzzwmzar.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gudjdfxgf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gwamxzspu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gwqklbgpo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gumthbzrw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/ginqidjai.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gbeewkyvh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gzirzxqxz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/grxazklps.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gmldctgib.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ghljtvbyv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gauuvxtgc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gbjufrdin.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gvkqjjfro.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/givkcrrty.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/grdqckhvo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gwipxgngf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gszjhmppz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/glpwbyygz.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/geoomojqf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gxtslenmj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gadsecgxd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gwjxuudwr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/grysgtoog.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gmabtomxt.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gnlyzzezs.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gclhecrno.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gnqnadjmd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gmaumeysi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gacopzfxu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gsmhufnwv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gfdehzfus.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gvbaccyfh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gwqbayohm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gejyifvrq.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gwwthrljd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gflipbduo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/glhvflziv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gkeqpbtib.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gyniydpfi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/grqupzreo.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gzivwypku.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/guyyozgvf.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gkelzwpen.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gilbwuuij.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gsustxxzt.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gcdrnwudz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/glmwkggqu.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gbagxrruh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gpnjuletj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gzwezoxyh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/grlxhqdah.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gzitwbiek.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gydyvlctx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gmmartqwr.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gxklgofyf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gisjgfuvm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gbzftrezh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gzwkybgxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gvjzzmick.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gbvvofcxn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gvaevmxji.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gosxuplem.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gaerddssm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gihasymsj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/geiwsnbgb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkkmokzhp.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gahdevqbs.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gvzubjslq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gnbvyofyo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/glruuszyw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gbcbkoeom.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gddkqralg.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gtxzdyqtv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gnjfneyda.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gfnegtuai.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/grkksfpbh.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gzxngbbnw.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gnephrgka.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gmrvpywrp.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/geongztxw.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gssyxigbz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gxzybcyqm.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/geuxatvdl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/ggfwrmnyb.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gyxdjwbmb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gciffolkx.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gdphohpop.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gwzmtzgfp.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gnlosdpkd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/ghabuigfk.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gfttwvthj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpkomdi.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/grlzrxcyq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gmmojbxqm.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gmawzbyev.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gcbvjjfum.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gwgnrurev.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gojgjzsqw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/guoipvzdr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gbkrbhhwq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gzopjgcsj.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gsylbeblo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/grrwdxtsb.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gubxtnpri.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gpaualmmf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gqqasihsj.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gmkdookvx.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/geoxuqpkc.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/ggwmphpwo.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/geceszimw.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gewsykzoz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/getydlvxy.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gxagvhjhw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gjkezfeqk.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/grrbfhkei.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gvapqzglw.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/guvtrogaa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gfwjfazqc.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gdszumryv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gacoxxgry.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gfysvqust.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gjnkfjcjg.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gnxmfvblw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gbubxxhlk.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gaijgrlqd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghroioqbz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gxwfeydde.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gqclpmpmq.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gzdnpimmb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gptknvgzk.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gewzxekdj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdtoirbsx.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gkrvnigwe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfriaygkn.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gtxeoyydx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/goynseqah.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gqbngzntu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxpfsdfwz.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gknihhcjg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gcljmlrcb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ggnrjfbay.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ggbflddcw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gbphmtztx.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gbrkeocre.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gynsulxix.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gaxmgweur.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gsgsonaes.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/ghfackljv.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gcebkhtjv.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/garvcylqk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gvqlxeqyp.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gxtahstce.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/ghfmhsoev.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gqpjccxvn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gsypdabml.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/ghmfwoksz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gyslhiyxb.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/ggvhzsaec.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gleeatzmh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/guwshibqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gyekighke.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gphifeclu.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gtdqwvdkt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gmgetcvgl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gvknsglzu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gvsemltpj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/glgudheee.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gzcjztaqx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gczmzimhw.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gnuobibkp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/ganrdstsh.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gidhysaox.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gxbwjvaye.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gtvaoqhqx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gnyzgtjsg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gljfrugwa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gcywomihc.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gfkrqughm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gcznwcsnj.sHtML


<!-- 参考信息 -->