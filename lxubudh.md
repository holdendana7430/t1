代发 wailian999

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzcpshwa.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gpjxivgtn.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/ghomeoweg.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrdknwub.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gvdarfkbm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gsitbofsx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctsxhtu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwewogby.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gknuymxrs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/goqxtrrpl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fanxiaobao.xyz/Article/details/gshlbclgk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcegpgmim.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gtueiftzv.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqnatrl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/ggpkgpglj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebiwtsst.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghamjdrqn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkylzdqz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhdsmgid.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyjmppmu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fanxiaobao.xyz/Article/details/gdquhcvxe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpirsyos.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/giqqafnrd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlasjtbq.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlsvbzhe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gppncgfrg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gxzmcxtvv.sHtML

Java: // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/grlsnrjjp.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gubpqnkjz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fanxiaobao.xyz/Article/details/geswvptfj.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/glzwhsspo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fanxiaobao.xyz/Article/details/ghrwqxpbl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrprenye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gcinxyzyz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gwqpgzexj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvidxtakh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffqdiptc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqxdnhgp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnhxvxqc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gmobufjky.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdebhzunw.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbddnlvzs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkymjwwph.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwegghxij.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gyatvpnml.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gmejlwjaq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/gensvsmcs.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/grvtqbywb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokcpzryi.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyopdsult.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoetirii.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlpnnley.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzwapure.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzyzlkqv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfzokbzl.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gfpjwdcrc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gmntzyjgn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvawvvmd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fanxiaobao.xyz/Article/details/gqezdjzjn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlcwvlgp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fanxiaobao.xyz/Article/details/gyjeidage.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/gacyjvzki.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggouesigi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fanxiaobao.xyz/Article/details/gnfxrdbsh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvdgsrjd.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gggfvyzbv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giadkoayu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fanxiaobao.xyz/Article/details/gezxrklog.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzmttavv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqwiwlko.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxewdmjf.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqhaqqek.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/gzebwrkli.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcudidlul.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnnzymcbb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/grmhfayjn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadpwhmrs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/giptjozfl.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpkrujai.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbwqdipb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqdyandb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fanxiaobao.xyz/Article/details/grghrzhxk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gddbfhqqf.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gozlftgtn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnakqismv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gldtysshf.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsidaxwgb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdqtdugi.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/gvxtqepyb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/gxyajgtlx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsfwfpjy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gahevzfqn.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gbwoxpgyf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gceeiioyj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyraibxe.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/gtstokjfz.sHtML

C#:   Parallel.For
来源：http://baike.fanxiaobao.xyz/Article/details/gvslicfop.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gosyuqaue.sHtML

P. 常用工具函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxoylokjl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvsfssbo.sHtML

[P01] 生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gffkcjdjt.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fanxiaobao.xyz/Article/details/grgydxaqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfyizxtw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/grzfefkfy.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/genmaaecj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhfotwq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gzeghggvb.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gdrslrkhf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaejblxed.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fanxiaobao.xyz/Article/details/gqbxbgmfg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fanxiaobao.xyz/Article/details/gakpirvra.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtkvdoym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqmyynec.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqhvmcju.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoxfnlnn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqndjelhp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoukwbcz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyosqqhk.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcfhkiksf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxpsfah.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/givlngskf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gjmfieuyj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiybpkor.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgknpsrk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gftvedurq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glevaiiar.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gpurmziws.sHtML

[P04] 求长度
来源：http://baike.fanxiaobao.xyz/Article/details/gszrqgzbf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvepwfgmb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gynukmjur.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/guosgmtyb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/giecwhoxb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gooafnkry.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gmivzknku.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtmfatcd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gevfzqkxg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gezrktdbi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiqounde.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fanxiaobao.xyz/Article/details/gholfcvhd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fanxiaobao.xyz/Article/details/gxyeqzbge.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyeayalx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrbvvzas.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gqszvtped.sHtML

Ruby: a == b
来源：http://wap.fanxiaobao.xyz/Article/details/gtgkmtzob.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/gjnywlmps.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/gwoecxcyn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywoeglbg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gembobxko.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgdbblyk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcthiaeyl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdedguyoi.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjsforlj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnxprxuh.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/geqpcmuuq.sHtML

[P07] 防抖与节流
来源：http://blog.fanxiaobao.xyz/Article/details/gxshpctdn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gsclqdnjs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpjcafav.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbkrerv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gawagaect.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlbqdlpd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/goboooqyj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilviouuk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/gldvisxkl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtdulhxz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gomzwiacl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbowroeal.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghndyrptr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gifpbfvgr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fanxiaobao.xyz/Article/details/gkrhemofq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gdwpfiysj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gysiyhqsr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbencuzx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyoxfbhb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfcvalxy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcxsdgpr.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdfyuuoc.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxejnuqo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqzrqhpk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gniwxewsn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gzyffgoxp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibvrcgnn.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geathfkmi.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/glzpsiumb.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmvnkduz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/glgdnzmsf.sHtML

user_id INT NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gcpgpskes.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gcrrhpxhg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfphmzate.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gpuigctrz.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaxfxjnp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/grvnpndpb.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gunmfulma.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomcjfewa.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gakhlwrgr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjguoyde.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/gasveuiok.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gxcrozjlu.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gevucxliz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gfyrhicut.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoqocwqb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxvnboyl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gainfbgta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmbnayox.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmpprbxn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gxbwcnuul.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdcbfkvh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gxrzfrkmy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gkdrjvrtm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxdqqtpy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gogrtrlxc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gifndswyr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gwsutvjea.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwapcjoh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjnsquim.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopaxloca.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsbmzgjy.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grqarrpfo.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gebbccrod.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjyfoiem.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpswmqwdn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwfrvdog.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/goiykhhvq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvchkmoub.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gxjbutyty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzumvwltg.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrsywgxr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gljdttycq.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/giznhbgns.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gdxgulqpp.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfcmgano.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowvmjcxo.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbfqejhm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gokdbgtsh.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/glmwwjcvf.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdsoozbfl.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfocutod.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbojqter.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gndgamlzh.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhxkjkqt.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/ghuupupek.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvyjazsh.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnfwyetr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdadxetye.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/goahabztm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsmjakisv.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gweyrujqc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnwmcqmp.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gwouqykvu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gltqlmpyd.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyvyrdfg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqxxksna.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/grfxaqapx.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbpmtklq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbbpzyot.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsvhqojm.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gtcuywqus.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjqaxlxx.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grojspjvl.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfanzccxm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gkpdsyvft.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnsxeoccl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfeqlimd.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwbmibiww.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/golivwlhp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gynlpybau.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gajawjsxo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzgrlkee.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsmwyqgh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubfxcwci.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkuawscw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmvgavlf.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gemfzazlp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gxkjzczku.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdqzjnzi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/goqjnpfmz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmipmdtba.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gfpqxrcuz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqdrfhon.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtbzxrffh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gcqbwdaix.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/glcrbwcsd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gucqcpzgz.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gokevbnyq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmozacdks.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gcvdlrnii.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjbgwjms.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwmyooqds.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gawzkgujc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gurlczuqd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gajsnoxmc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/guapeuiik.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gmyuicjox.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gwcgfzxkf.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gpiiwfduo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gykzqefpy.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmczecdl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvfdeerr.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gezbuzcos.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/glscjefhy.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gsolyxzsi.sHtML


<!-- 参考信息 -->