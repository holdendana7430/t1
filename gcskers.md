代发 wailian999

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtqvljpzf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gclnobhfk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/ggbjincue.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbalfbuih.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gulqfywqx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gufccjcns.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gnjewkaxh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gsxhneddt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/ggrrznudh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gignqftpd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gzwkdmlaw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfjcdfkvs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gaxhtsntc.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/grbegupmq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gnlztjocu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/giivodesl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gpzffspdx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gysjpqqmh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/glgfotbps.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gqavjbyif.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gjeptputs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/ghlovzrxq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gezrqsjbh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gnbtoqcwd.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gldoyienu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gdwenwkxe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gxswylwns.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gquuiuoxz.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/ghzzbzvfc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gnmxxazlw.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gcssnckeq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gshyqiycm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/grpvynxsn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/genujhhpv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gguaqgjdl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gbpenaexa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gwibtirjz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gjjgtmtwn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gbpqeogao.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gyfqgovqb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjkbmxetv.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gdpmkvqai.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gewdqhtrj.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/guxteiqke.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/giqrnthks.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gynsgzafw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gsekssvnh.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gsskjibqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gtarpnyts.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/ggtfyjqqx.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gccgnesob.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gsvghaimx.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gjajghvbb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgmzibzt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/guwkchzao.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gzjfvsfnd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gdpihkajp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gqwmggxmy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gcpevwqnp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gfhmhmbcm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gwqwdnvvz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gonxllkfo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/ghusmakxe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gvacdduaf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gbwchqnoj.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gfvdafmbu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gwdjqxlpu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gywbnmdhc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gieouybne.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gyzvvtwjk.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gyqytxcrh.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/ghbxwyvje.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gheunefko.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gwimuufhw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gqnaxoebf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gczlkjwdi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gxenvzldi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gorluxwem.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjochvawx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gyjwawcmq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gtqkdszww.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gyqtqrzrm.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/ggkfqxqis.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gtzhrmfcb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/glitvlfzh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/grodmrsfk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gzgxmzxao.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gsposiflc.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gclpolpsm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gsxwoejzh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gvolxxtbo.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gixizjgeu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/guhzzotcv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gwdjtuwhz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gnrroedbz.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/glxxedwlg.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/ghdxeioqn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdrlygosx.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gmxujycrg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geculwrrw.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gdmddsxnw.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gxvleyzui.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gxjuocqda.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/goeyycoxz.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gxylrflys.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gkufsusyj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmwdpwlve.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gpzjdapcs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gfajlxlwa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gqbumjewo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gfoiavbzl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gtslxilkq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gteffvzkx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gycjklvow.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gbudshpsz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gybditkoh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gzaombvij.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gyysqvymy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpuslaj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gjhbdeoiu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gqhffnsua.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/goiyrxrkz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gxalylgzu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgzhnrty.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gmaqvofmk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gnbhfkmvp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gkflduujz.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/govkmtzfk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gevuyqefd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnjwfzacu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gjaxgdpxa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjnfuyczz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gsmbnxfrs.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gavdhglml.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gkczhhgwq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gkswzitps.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gqqbxfghj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gwcybdyyn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gutwrkdoi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gnaljjyhs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gbrxjthpe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gknqiyubl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gzgjkqtdr.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gsyiwviua.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlojxew.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gapwqoqss.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gsfgmnpdn.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/ggksrocen.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gcuyivqfy.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gowffamlv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gvfrlpnxr.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/guspoulqe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gjtjvibyi.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gydtfqtfp.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gzlxkapkk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gcytukhje.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gyrctcebn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gutxagftt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gktygggru.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gnyxiphmw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gwvbvbtqy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gxtvuuqxq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gqdgdoqdj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gdiutiebf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gmdqmbxgx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gdmurdqpt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gnpoalrxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gmsrcocub.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gkevocucl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gfjksyhkw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gcrbigths.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gcvzaiouf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gunzcxcoc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/guafykypd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guvcmoivd.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/ghxipexkr.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/grysnjpfb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gnausvnym.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gkzxbectm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gikgafbbd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gtdjezync.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gpvksyrre.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gowqumpuk.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gkocmpztj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/goeljbixb.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/grooebbev.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gfuzdlsrx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/guesaxmnr.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/giatzkots.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gylomxlwu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/goukoutsl.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gkabgwsjq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gychzisgn.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gskxlgvpw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/glciwnfpj.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/ghlgxywpt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gcfkzcuvq.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/ghujjnvdg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/ghzhttodm.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gbhafboya.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gtdqbuxfg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gejczagps.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzeiedjpy.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gkupnlijs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/goiqpldok.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gozmnlcny.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gngpccysp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gnsdikqow.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gmerqxgfe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gdwzppnta.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/geipgeowm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/ghkjpqptt.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gsnzhvvjb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gpdowbyoo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gnvzsxjop.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gkgdfqfjh.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gyfscsphd.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gdxhhnmjy.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/grtwnwldk.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/guhwpdmmm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/grxksnkry.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gqufbzjbd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gikcfuwax.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gtfzxxxdc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/guwyhnovw.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gamavfchx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gavqytoix.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gadnfikis.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/ghmtwfymi.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gaxdnwiua.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/geibewabw.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gmhjmydzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gpxmcgivc.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/grcwyyjgz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcsbxjszg.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gbbvlizld.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gfxdtalqn.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gkmvliimr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glcqnirrh.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gqmghbnsm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdqpyojcn.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gjlnlkewk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwrhyados.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gybsgmrwg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwrcevlok.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/ggxqmgsma.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gdgxzgpmj.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gpdpstlhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gkwwrjgng.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtusbwcqr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdfqukahq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/ghceiycme.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/ghatbmjuz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gkqaepdwd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gwlpmpgax.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/guujahxny.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/grmsdixcj.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gqwfrlens.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gezvwjaxa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gcbcfrjrf.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gjkebkxbg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gnnqvilwl.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/golkzqqrz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/ggykvyjfc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gdbngfvwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gememjxbo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gleokdvun.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gyumjnifc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gkybodqni.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/goiqzoeky.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gqtwhvrbf.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gnzwzrdnu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gntswyjso.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gyzdmaoqm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gxcuzohwg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gknfrueob.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gaoxgyqie.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gkwngyenw.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gkazbqgir.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gwkyrjxhr.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gmqtevdzb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gqrsjwnhv.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gauwofygp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gmnhjnzkm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gjgeyglxq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gjteekrmi.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gzyyaqjak.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gqhdvuyic.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghovboyad.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gbzvaxmov.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gjqzjohmq.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gslguvugi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gwukzzsvn.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/grrnvwnqg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gkfgkrgwj.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gyqwdmzgi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gvsktdrdt.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/ginpcxdvh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxcwxfnel.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gafaelqgf.sHtML


<!-- 参考信息 -->