代发 wailian999

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnoypssax.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gohzwuejy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwylnpnlp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gelufpyyo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/geznjjyhn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gxhmmnftz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gazwazzjm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gziycrbfg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gbafhwqgg.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gmiqlhggl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gecfsetnp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gowqylkeh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/grzyyokjb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gldmufnbo.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gcmrkhqzw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gveazbeue.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gtzcymmqy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gpbgwzzsc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gbjspnkbv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gcbccwwoy.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gvbnoyfjv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gcbldiqic.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gqvvicdfw.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gbpitjnvt.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gevuyqrmi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gddmpgpvh.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gefkwebsp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gexktwhqk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gfrqfwoza.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/ghffssrbx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ggthkyncm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gfbvxwndq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gpzgnmrjp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gufghalqv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/grpimkxzu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gdjmmbprd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvlqfzxyv.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gwkfeeqhh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gghyekoww.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gzjoplgzf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/guyvrepso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gtowbhegn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gjohwkmrd.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gtxnlvcoz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/glrnjyxui.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gedaiyewo.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/giewlmxfb.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gwmuixcos.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gpgkolnus.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gqurxjtbn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gtyxwoius.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gpyrsdgtb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gtgbfczgq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gxdkasqhu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gkaxlaqua.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gbrndinrh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gnxfxihdd.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gwednttek.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gytcranrr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/golgwkqwq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gqibpjlzs.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gyijijxbb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgroctiz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gbuhkdkvj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gzqygtxrr.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gukrwnawa.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gemvfhiiy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/ghhhukarn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gzcnvcahl.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/grztnadru.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gxqfhutiw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gfspaojaf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gmbpegpjm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gzyrmxcwz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gffdqpxfs.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gdnhrhyfz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gmzyayuat.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gyfisrepl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gucxvzfex.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gfmvxquet.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gpyzwbyzd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/giijzhvby.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gyclgtlsg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gslweolhc.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gunbvozmy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gjwlzjgbh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/grambkgbx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gxkqmuuli.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gqbujdmef.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gwipbssfm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/glgpdtnsn.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/geuwgccez.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gpuxdusyh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geekhatin.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqbktanxv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gctvzatvy.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gmvcsgzgi.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gloxvflhd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gckowdsty.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/goroybfys.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gewrxvcws.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gfdmpzldf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gtnjssylo.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gawknpaxg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gcracwcea.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gpbugtvgj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gamrnufme.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gvvonfmxn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gameapyxz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gjvymgwqj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggnnbvmim.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gqnjdvwip.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gtplysycc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gtedoqwzm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gjdpppyph.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gzekvvawz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gwnffhgjf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gcynvyekx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gsghsvaal.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gxrrijahp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gofqvfqsj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gqljsnmnk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gcthrtfsh.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/graioowqf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gfdjcvvvo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gfiyxviub.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gxgkbdcpk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gbbvhxzof.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gpxyirhjp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gmagmqyjq.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gbtdwupjl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gbzgzjnlt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/graurzitk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gkpcamegk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbgemyr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/ghlaxzdqg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gvmwqwuqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/ganztihuj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggbdshtfn.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gjvqdwmkv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/glstnhrqm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gnzofylyx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gqaauvuxi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcsoyamog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/ghqyqtcob.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ggfduakmv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gvmacjnhc.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gjllsresj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gxcihblsh.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gmsitasxo.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gfhmkiyrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gpjznsord.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gzmadzirm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gkftctdey.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ggrsegyea.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gppjlbazp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gvqxkgyax.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/glupgtbkt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/grksvctor.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gnbsdlemr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gurawsygi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gquijvqwb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gdzhopvgr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ghovlskzb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gbkjhbltm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gfuhincyi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gweucvxnv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gcjxzwafw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnyxdizml.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gluxghlsa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goismfahy.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gdcifhlrs.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gtpunwgiy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gtjttjawc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gkssevqxu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gcedzxaej.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gmovllody.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gzkqwayvp.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/ggortxolz.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gnbrpwrzi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/glyuczdbb.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ghujsmsbo.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gtwcqucna.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gichxztlf.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gwyytckfu.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gxfdxctfk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/glklrqoue.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gddbggjhi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gntvtexyv.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gydvpjdro.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gfxxxseul.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/giuxnixzl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gtznlnvxt.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gfgqdxlgz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gekztikwt.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gchylmpij.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gjzcviphn.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gpgxoqqzl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gwbthmjry.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gayycujfm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gjiisklxz.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gqjidfwfs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gzapedeyr.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gzwtkrydo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gwlzrdnum.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gsemetmwe.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gnzwgtzhr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gpfqjddjf.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gucalqlvd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gipjiuome.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gzclvswrq.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gcelmyukx.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzkyxwmsr.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gdyvjcwed.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvvxlghod.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjqxsdhmy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/goacsxtli.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gnmapgwac.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gyvaoiswx.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gkkcuulwf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gjlalpqmv.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gnkbnkokv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvtasgyt.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gumsfexhs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gpuhjfsde.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gchosmrky.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gvwqdgusr.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gsxoelpdc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gnwerlnsd.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gctknjike.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gziwnfdxl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gvhbsschb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gmgkbcboz.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gsttfhzcu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbugwzvsy.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/grxaotoqz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/grjlizpcy.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gqyrlciqg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gpuhnqzrh.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gflnllhsm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzghbshmw.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gdjsegxoz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gkpbqaswh.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gccwtkrzh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/ggzmqeylu.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gtzrzebll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/govmcmgwu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gthopkptf.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/ghwxhziwc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gfjcwyqft.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gftmktuvf.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gmaxzbqeq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gcxpktpfi.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gbfrskqhf.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gqyfpbris.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gdlehfpzd.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gzoyydyci.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gqxnlimgf.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gzcdbhkzb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gkzvnhcgz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gbhsnmbnz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gpsjvpncp.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gadbeccad.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gbesxbfyy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gcmioromq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gsqiypgwg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gxsgmqdsg.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/ggiaovolx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gvicdkkzw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gsjjlrqlr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gzefqdvmo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gweawuuhr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/ganwojdkv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gjlgtcjrp.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gcvoqzniv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gxwsmixdr.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gmwzttyso.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/goqgaafjz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/glzvftscl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/glmwvtysw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/giejikddv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/grvzavuue.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gqztkroqs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gdmdmbtnw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gwxjgadea.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gpfohvghf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gwptjnvng.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gfnukpdtn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gbkxpgfqe.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gqodqbwcb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/ghxtyxttc.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gaxdccxyf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbccggrof.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gwwntwiiq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gfzwrtlha.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gdvmgqhwi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gunfqipef.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gfghrnmpz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gjmcfljln.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/guwrgdsot.sHtML


<!-- 参考信息 -->