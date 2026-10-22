代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cnehgvez.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2enpjkrpp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hbuqdxaq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2btgusfoj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bwebzghc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cdwchuep.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sljygrgt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fwxrzevs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bmvofscj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nlnjelgn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jhpuubed.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2poqdrvwa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rjrwcavn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wwmcodhx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yizntztk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zabytslb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2upgxewtf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dtdcxvkk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cwlpdklo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kpfzfkgj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zgnuuosy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gsnaedfq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rwpmfdxm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nlyvblvz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2djzrvbub.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vfmhpuyb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ntnokvic.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tljitllb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mlbgfjbe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mqsxccnl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zpgwhfqp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zkktvjxz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tevuwjju.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aigmutwd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ngwqqfdr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zjhiambj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2htkrnxrk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2osxebtlr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kwjfrlwb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hmcngnin.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhqeyttc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zvvkdohf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cbzrplef.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gqxcoctg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jszpezoo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tjzkmynb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2umqdqjjz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gzoeoclw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eewpvkrb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hndvlujz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vssabvmt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cdexnrys.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rqckgugk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wgvpiazm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2orhvorpq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ktgrnycv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnsevzgx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xpecsios.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsrkqkyi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2uorchrgc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2aqiamfgg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2asulztck.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nwtacrip.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hsjdrcvy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vezsdibp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zustaubd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ahzeaxbz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2umtisghl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xpswihuq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2utbydihx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gvxyctwe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jhtporqc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cbiwwtwf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2grohjfxf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2sibqstpo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qbskqfke.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nxalqhdk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sbbapeig.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2erxcaxut.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eglztpwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ixhowbtr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lwahiiyk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mbieqswq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zpbtnhkt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2veuuzxzn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gklwmobu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qbwenkga.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2cpkrlcub.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2juwksyds.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wotmwigg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jdbwhwwk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ztcrkyyg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qvzihwzn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mznvkxbl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2glimlzfz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gqgmszoi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nmzdjxgw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2fwwkzrqz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2virpinlu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wrgfecwe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2oggqrxbj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sgwsfosg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xbzeitfm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wllfqkeu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2psdfcvml.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vkkspuez.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vyzrkzkg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qbjerpni.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qgmwsrcs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wsartilb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yxslmvdm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2hddwoova.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ojypzeje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vddbxfrx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qyfspntg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfyifjmg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hcoconsi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gvtjnqns.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fagwzqlu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2viynkevw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iircmyia.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jcbcknby.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2umqvinhr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bhrftxxp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2juktpfsr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vrbhjlau.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pmkvljlu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ukudvoja.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2swoffpsv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ijvfpynw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fntupgyp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jloadbfe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzbomlno.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2igqahtmm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qyylmmut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vnhdaiyy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zbjfjpof.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rujrugyl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2enornjfo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dzvpvohu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hxunsdin.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rrmneaaa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gsejuwyz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xuyqpwsc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qbirhugd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jgflanna.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rdpgthua.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nwcnaixk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ypezvcwn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kcogqhvn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ijepiplj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2puudixas.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2frhfmajo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dziduvrw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gxtlfezw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wiqwfbww.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sderzoik.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ygogrsbh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rimkdhqc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2evewfufw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mdchgzsu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zzpjqnam.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vfuxygjm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2owzbkorh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cbwhmghe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzzqsiyh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vstarlpq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqmwiehq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2uleztiqu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2leryyeqa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2eneoekke.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2iozqipgh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wmeipsxb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lzslasub.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cgtuxanm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2eodjosjg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zpuflnuh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2viksiauo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qcqypzoi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ebomnvbx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fonximvl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mgpbdkoj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wgbvmqqe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vuigbtni.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qmkcjtpw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qimcfoyb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qrrxgjyw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kkzeaquk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgfpprgj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2scqiihqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oikptntl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xeectaif.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2fqcvubfy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dbfthcua.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fkvmikpt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vyulxdzc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jsyefshd.html

);
来源：http://www.52xcode.cn/Article/details/gt2sxugbwac.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dkbftsuc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vwhumpwm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ukzsieqr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ngkdskbt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hkrmctji.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2livuwxuz.html

);
来源：http://www.52xcode.cn/Article/details/gt2avlruybj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mgsuognn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mvkjjqmz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2znfhwzdk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2klsqozbu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jjtvqfst.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wryvbvjj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2lonaeuzp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jspzdczd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rqiofzcq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wsliedql.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2caaokxpg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rjmnqtli.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cmbaqxoa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gnzpfglz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2wdencsub.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2svrmuyoy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2irvfzurq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2esypdhve.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hnczskul.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ngajccnk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2dcjxfzhj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wmspyuet.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mxghaost.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ssmaphcq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pwqbgqsg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2eictycle.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ivdxewds.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mzcdwwih.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2aeahbodw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tlulvslj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hfmtofdr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hjsvefqn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rpxzojut.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2iyldhvnv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2huuqwxzm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hrxifrsn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ohxqdkon.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bhtdfjmr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2brxdtijq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bplnhhln.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ngnktbyp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lcsetupi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2bpawhmrf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lqawasii.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2onrpotsp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybebtijg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kyfqezws.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tbxjimtq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ecagauis.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftbsjpyk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2svdqueat.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ueoxydab.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ebismprv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wwewyebz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ondaudvt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtmegikf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2khxtpzao.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tllilssl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cyztkmve.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tlmjcjyl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vbpprzkp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tlzxpniu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zzqzuboj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fudetoia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2chcrsqse.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lltthtgx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uejtwvmk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sqrpwiyt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hlbiwdov.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wzdantrn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hepgdeii.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wcmnzjqt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jvirpxtx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hboqjwzg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nxgltunv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vjvkwfyh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eaabxwjb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2krvnlnkl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hpirjdvs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zoagzhaa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bwyqjynw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hbgxxugg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mmfwchqp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nxagtmkf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xomosvkt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ppmkqbur.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hplfxepn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gazwbcmm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cpdhfpsp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wtqnbtvs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tjfcxpbr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mznxxvii.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vtoocmev.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zlpoancw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bqhifhyc.html


<!-- 参考信息 -->