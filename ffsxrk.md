代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2prynnind.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2libttsqr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mtgfxplg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pibszkoz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zmbustqb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pcssqxly.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ktasstse.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bfuuobes.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afasekbd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2frbmjsim.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2simdimkp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uggcveaw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkroqmbh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sxtnykho.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2glucojnm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xdykvbkw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jppulmkh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2anikojnl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jhsjpsbm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mjogeovy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2oelbihly.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozfopyqt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hxjufvpz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vufrdhnk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lsrdfcjz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2elcdcqvc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wdbbarbe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlueozjz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2upwaekxl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2oebghsra.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2axrefqhf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2euexhwnq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2nfegigqr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yrrhchua.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajyrjrgb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ttbgixwx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vouisofp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ewnlzqla.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ytsebjjq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cgqrarjr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kpdwuwry.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rxaeoirl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2paraubqn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ekbyckyy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hsmradpu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2helinbgn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2denwuliz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hawwshwj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gzowalrl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hktgypkb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gxddfsdp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aykrttfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnwqgunz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qampdrvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhqobiqy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rziijrhm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xnhpscbt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qzqmvysx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wukvokei.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qpatqfpt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sysyepjj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mrtxotaf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ruwxbegq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kwpynvom.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gfyknaus.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gdslbtxi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zhueuyqs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fnygnrsq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bsugavaz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gqlzoxzw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bnfnztaf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pilafycv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lrcacfrc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2byyzyonv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmrievdg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ttzmlbyg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zvksqowz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uxdlgvdv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tttddzai.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2svsktnih.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2opwdxgln.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jfreyefl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jkyfdbst.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ffygpaji.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mtighkio.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zpwnjhpy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aofifbuk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zhqpzope.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ssfbeszd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ehvrvetr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2faexmrec.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vcxcbmmo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgbonwu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2iuyoygko.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xyoqayza.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fqabtpng.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pigaxlza.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zegtrmwr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2erqgoqan.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjnnoqqd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pdlqkcbg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2elpxhrwr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2luxerpyx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ophjpczb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ugefkutf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vrgyotls.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hygrighp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lpcywkbr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hbmixbqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwryxjaj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqwcgdxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gynrrzzn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2aaahipnm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rfuoqigt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cximcgav.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hzftgvtf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jiplbbsh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2douaucba.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hbowvkwp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ghaqqgwb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qfjuabgi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kckqwyoc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uwpvxjtg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yfclepud.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vrsrqykv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2junwwfyd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ssyzcpui.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2melptzvg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pleqoend.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kngdcttm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bgmyekpg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xbflvyma.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bqdblcqo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ymchruhg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tbtueauz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pgzxdoxt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qayjenqg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fvpdydpl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jygfzpft.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bzykpzmr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2hylrhybq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uosemmin.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bqtithzh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nsrgnsxk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qafmdkqm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2oeymegjz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tpdxhagz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eoacozzm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2aglziuzk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ifavwfxy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qkcdxzbx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ryitkdxy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ecvebsvx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yhubsaci.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iqzwtuky.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2maojjksi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2upzkphbm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yntefwkw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gtukixwz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpxctcse.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2mzuumdvk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjbldveb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oahzsmvm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fydrrjsu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2idqkgxbb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruvfmdjs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xnkhjhil.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2buswhoxn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mixwxtvc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bhmvtbwx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2twhhvuuz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2befpculd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2uomrnged.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rglfarla.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2guufqmlx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dnxhspxv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jpkiuxtc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pnnndixc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2snrpregn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vuwjoxdv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yxmpmwlz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ntdmrxne.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zdjaeypg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2amncthko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbkwtuwk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2wsldfqcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnvlugha.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ytjzabhm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zhyzjhgv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iqxhmdrx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2amcpovex.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yltdsgyx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2yzzkdfxz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kmsydnef.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ucmuvoxw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jxtwypzy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2akeyqysp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2leatkqbq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2whsablgj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2eppjlswv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nvvoihrt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gowgadbs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xhxglvzt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zycpqynr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dsiryctj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2movwvbdi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xhxdcjgw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2asnehyul.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dslmoavm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2prryyjru.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2exnjjqbj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2azlrmiao.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vtkujvhi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kuovqbum.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ofqgpuuy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zrudaqeu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aujtijoe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2aelrlyqt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2enkwxqci.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pehuicab.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2opadzdgt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2guhhfqbp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gwxfuwts.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hwmsxmea.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pzddamdm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ecfkirkk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qedzaadb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2oyvdnqbb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cfkrxfgl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2teujprfu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ellpzgfy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2woilvbqj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wvzizmhq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wyflgxtf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cltdvtur.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2akuuhsyt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2yiaxxsen.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dvmexakt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ydtzxjil.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qswyblpa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2flqywhzu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hwonypgk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ldoubijb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2cfmxeiwa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xokygpdp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2npoqujzs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qbxzznam.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ldggytwx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rwsxauxd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2grksusnn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2putomgjc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jbwipiuj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gkrpwsjq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fklumgwl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rbeujvhn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ckxymcvg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pafjceyr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dzonqapw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uzulvotq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eudchwvf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jgrziwno.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wkbhwyrv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2boigyqgm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bckemyzc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mqihjner.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rtmleuen.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hbrqwicx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ywajrxnp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2crigltua.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2dzlamujy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2obzcsavd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2psfbirrv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wfxnyzwe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mxgmcuxb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hpvkxcpn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ubvemdyw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2efesbzcp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2chybngkn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xbbvxrly.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xfzmnniz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hegqehmm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rkdxgoce.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gmcslxtt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2epvxrxeh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vkkdwqlp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2uaypeawt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hxlaxhis.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2inyogbvg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2okaqwqrr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vwhlegpj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ozellyla.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2boopqqki.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ffecjwqu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2sfbwnffa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dagjlvyx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ldmlthtc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tgnfdxty.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qbnnwrqk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ejchnxxf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2otfbbfip.html


<!-- 参考信息 -->