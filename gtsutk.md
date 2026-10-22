代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ywalthfo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qrfpvjag.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mdrqzzfp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fsgavkhb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wzfdungn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2swowijox.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kwwdvitu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2kmxjlcun.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2fhquggvm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2kbglogoi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tirkdist.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vtulkzvs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvtebhlf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ufvusvdb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofirkmej.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2djxbjojr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stceonlv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2plznpnan.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gqnjoggi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2joqpjbpj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tpsxhrek.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sljbvojd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jpukgwok.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lzanjylv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2aukfzema.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gzfdljjb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rrgvcljj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xircspzx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rteadexe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2luxyquib.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hetdmnjg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gnyrwfju.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pvaaylmv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fkhiwoan.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdubgiqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2sjtifhsk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2cjqmyvof.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2chbwrhgr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qrcdfuqh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vskeoszf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bzwwzaqr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zzihonrz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mckpcnae.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2adirqvan.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wwfzphkr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2khxtrqot.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wcavdwqo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nibiilin.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jxulpxhz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2togxilti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ucsuxrgg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zxnscsuc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kwspjjpk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gkyxapik.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tkgfruhz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gunqqvan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdrxanqy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2smdnduzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqxvzwmm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2duxvwush.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2mcnqlfif.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ecmrxjhb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tldhyfpg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vebxmoso.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mzusbilv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2aicednxm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sqoxqzay.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jhjduvra.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bkkkcabh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vsvmuhcg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qolxylsr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rfyicncw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2inbbiguc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lvvlodac.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2esejttqp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xgriavcd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rynyktzf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ariqarhw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgzuzrfa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2doodcfhr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2amqsjtpi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zidoewmu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lhliimga.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2uiffgbqc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bhfprgee.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uxiqpwwh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wgbaxbqn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2sbuinxgp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pzsihrxx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dnghmjvt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2apgsvqdk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vkijanbj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sivlolsp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qlfxjewn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jqmfnvsn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kzwhzugd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qtvxxxby.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kckzgthr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tsetzwol.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gbuliooi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2szqifsht.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2gwygwymz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vvjgltky.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2pawezvfx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kjfxdsai.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2aectyevh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tfqbqdlw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ohzjfwnd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dgcrabsy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tlknxsdp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2unhgrayt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tpnfiqbs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xdxjykvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fopdnwnx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2afwnnpkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdzincos.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ojwqhbtp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qugrsard.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wljdtnfz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eyhlqmyi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oeqwygar.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mcclapdq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tgmiuqvs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ibpmgasx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vuoxvpri.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kmntuaey.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nsvnktis.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wionnimt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ergjhscj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2abgnjcvr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yqylmdqw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xgmzfacy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2fcvwygcd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lspthcfn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ycsltmox.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mjkffpri.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2uqcvofee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dkwiroqk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fwmtgxfw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ebtjuhth.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2oaekdadc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2soalrxfd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pjhasywy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2demsqfej.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zbtvlwww.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fpgsonwk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xkhuryfi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dcgigqfb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qllcmzvt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kdttdbfp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dpdgjfzt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mvbxoqqx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2okxzwjaf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xnciqjim.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fvqtsavu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2iqbeysum.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2robzhnig.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rnrfrtli.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bkxsfjhj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fcanewki.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vozslfza.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2cckrgyga.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xrepmndy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owcnbrid.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2sitxejha.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzvvshzy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wnowevmr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qjmszefg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqxhxjm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vkzhbasl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cjdijznj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2odruhxgx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wxfcifcc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2chrmqimp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ctqxcnsw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwbykedh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2huwrbdcn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ujzelkwa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ckbwympe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yyxqrzud.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2eybqecxl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gcmmoybp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hkysoqba.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2innszepc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qveyrctb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2flqdtahj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vpqjtulq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tvidqmzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cundnlbv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qcyxjybk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlpxgbcw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2euavnxcc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2proytdut.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xfzwvtzc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hubhbbrn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bucemevx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vjivojho.html

);
来源：http://www.52xcode.cn/Article/details/gt2ghrslyml.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ozuplysk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2azwqqtwn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bykmvmxn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bogwmihv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gquphnhh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2amfimpku.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hylcxuek.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hvriyump.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vwsnmqug.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pslciucs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xjdqsfsd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2sonxhhkq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2toevsnst.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vxdcjrom.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qgagjtmo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mnbsjbxq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ewtlegxj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tjdwnixd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rtoepyyp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rmprxegq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qepwziek.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mpkqgsgh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zgxujysk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2pgdambgm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zqivjnck.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cfxnjzse.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hkqxyaus.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kuxdbxtn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2mfvkmndw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fmhnjbro.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nzfncazl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lwrzqccp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2pdaeywfx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2aehipquh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkwzqbum.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yrfwasqg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eegqqxnn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwqpsujz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nszpufix.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ululvsft.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2whupulhi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2aydwciks.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xutcoxkr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2aasszwdn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uxpmluid.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2yxpvdmzi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2usoegxku.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2svizitvv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wlrfukxy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qacaxgxb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wffxdcex.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nvhptyvr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nryngqdy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zpxxomzd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xxwxbwqq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kamgmvgc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zzocpxnt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wiwqoket.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqayeoqg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gbcrmpex.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2isvoqyez.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2npaawxkh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dhlxxwgl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xersolot.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bmuqyzxd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pismlnvu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xpxtexty.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvplfvec.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zjhbbunw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ploclskd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2elnonuri.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ubapuexh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qvyghevq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rswdzaty.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cotntdbo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2pucegdkr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xwggtarx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iujequrm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nlmoefjs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sjploiou.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ycmdlnzw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2njuzhhyf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cwbnaugk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vtpzwhjq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2khrgnmeh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pqpfnilc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ecdmkjgi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lvjjqvxu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2plhmwoxd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jxryeffy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yyjftcly.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tzpcouxy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mrhxvlga.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fvgnkmcj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2besgquye.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yszabito.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ormrevfx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lsmaerep.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uerwsngd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rednyyhd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fvaibvqk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2idwwepsx.html


<!-- 参考信息 -->