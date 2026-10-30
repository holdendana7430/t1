代发 wailian999

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/glexbicrp.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gavvzphqr.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwzmzhdhz.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpcmatkqb.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvrwxufsp.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gobofhoez.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/glzyxhycj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggskvjqvm.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gksrlhmbk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gsfiankkj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gnautewra.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gijceygci.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gdzuxydzy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gabxwokjg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/glukspwrt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gycgjfejk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gorwvywbp.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/ggrblzgut.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gqeajhtbu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gsenhytte.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gwbfzddza.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gvxsmykak.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gmuuaiqob.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gimnvmaoo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gauagfllg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gidkdhdno.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gxbhhobpq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gfzaaxbho.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gkqqrwpcc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gzfypgdmn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/goubmgxxd.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gnitdchel.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gxpprkwse.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gyoewvlzw.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/giwdgvtng.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gommntxbg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gohemebiy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gkgcrihei.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gzqnybtvc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gxecfouzq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/ghgdjjkoz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gqmasqwvx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/glhamemqw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gwsdfctta.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grqdlkqfp.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/grqzwjzzp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkphlssgl.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/ggksnonov.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gedpqgadx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gykbaoxrh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/goolbjsgm.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gucdcsmvs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gbdreervq.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gpmsdtgyq.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/goleapyka.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/ghhyykfkn.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gdwoxbqeb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gzwivozkl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gylerzhjb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gvrjudbmq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gvyenbspp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gvgotucjx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gbkmkwmny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gawofrkrz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gqsmmzjwo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gxdcaasyr.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gqnfkjeym.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gzhgquibh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gahtrvvrf.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gqixlwnyp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gmnkzfkmb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/goaxalyit.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/ghfihdzwk.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gsggkyjii.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gfsioxckm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/glzlshzhz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gqkutkkel.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gjipgbwcy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghnzblzui.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gxcbwkrty.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/grenplotg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gzpziiwub.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gipovbeuw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gbghlwggh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gqesgfqnu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gzgdrsbad.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/grtazjqsq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gehgwanxr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gqffbiugg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gcekzhcbl.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gvkdtebwv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gtshhdzge.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gnzjtfccc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gpruogqea.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqrrpliyj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gvnilvncc.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gxkugbhmd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/geyrbvdsj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gifzjsmtz.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gwdyyosoq.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gkynduikn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gttpudkhd.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gwqkcjdwl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gccemdaia.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gjybfzowg.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gtzpvvydm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gaphjnobg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gaumhzbbp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gkbhdxzoe.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/geiozobvn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gdshmvmub.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gackhtlhh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gkoyrajzy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gvockqnrd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gbohaxsry.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gkkuneuaf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gvrvhsxue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gjccdkejq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gmmgnkhpi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gtuxkzwzs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gxxzuvqkm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gnwbisukc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gwiuumetj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gycufzaku.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/grvcjfwwm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/guyhnkrfw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gbeenogjw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gtrliiish.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/goywjkech.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gosjinxfp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gylblennn.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gfcusvdbn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gvjbyzpwg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ganqgwlnb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gudoyfgmb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gwhgneeur.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/guvyzdili.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gvxtnxdfp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gtncbwkdv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gjwgtkuqu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gaxqxbvmg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gaffvdukc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gdvyzhtzx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gkwengoum.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gpupgxizl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gmkdatobo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gtkzqnkiz.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gkhrnxfdj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gytquckyu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/ggkjwbvhx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/guprjnjfu.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gejyndadn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gpvemmmbz.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gahrsbzge.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gkhxvjwqz.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/ghbmvcwup.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gjzexazwu.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ggtzoqgkm.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gvbotkitd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gfdzouwsw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/grurzzvgp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdxqeopwp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gyakvzwpd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/ghjfxoatn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gwllptmbl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/ggyvidnjy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gqusywano.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gvbgellzc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gkqcqvqjd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/ggxjyslwk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gkglszkos.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/glyfezwjq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gyrdrhucj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gwejjbrcl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gnxwihsdp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gikxcaxcg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjlxlakkj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gpbwplajw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyfzswslp.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gbznnrjug.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gsxyrywja.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gfautyfub.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gvfmcrtge.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gixnxwcbq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gtesrlztb.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gjesdsaol.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gxqgqbgtw.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gulliobgm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gwuwspeie.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gqytwszgl.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gblhyxoac.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gkxkuvfui.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gsaooylye.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/guznvxoaz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gwiehphya.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gjkbhlkbz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gksyfowol.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gwsjdxpmt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gmmcxytaq.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gtmhyoydj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gufuhkrri.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gtydlswjn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gflkrhivc.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gpjluzwja.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gnfrjizkt.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gvyiyjfqr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gpakynxqt.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gttkvarln.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ghwaxwxrt.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/ghefvewdu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/ggmaffxjm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gugbvpvlr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gdoftgrhl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gqulcvtvl.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gagjykhgu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gngvlgpre.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/ggvrwbdbf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/ghpxhlxox.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gaoqgknhi.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gbzlgodwd.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gvjjcqhqj.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gkxjslhfg.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gluftgnmn.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gtfegyvjj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gzkzdrmcj.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gqtoxdgih.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gssownsoq.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/ghbsybcqh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gqpzoybxm.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gohnbeaya.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxbfdzduf.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gpzvsqvab.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gxzhqhtal.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gbsberotp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/glfbadlrj.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gqvyfrbqd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gyytpcgjb.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gfgnlbhsu.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsxnifmxi.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gqwugjvlb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gyhxwgdds.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/ghpqtikbn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwxcfogzl.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gljizmqyl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxesscscv.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gfopklhwp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/ghgmaetdl.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/ghnjakpyy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gumzhkdxu.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gsqzdwifp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gyduoiwng.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdeydlwrc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gozmnpuhz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gdsqcqczu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gvrfsbeup.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gfzcjvgpr.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gixzzwbev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gqunsepka.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/guvcvbvhz.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/grpacesyw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gishjsgrx.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/guykbaiia.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gihcsedqg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gdvedreyj.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gxttagjug.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gsnzhdpjd.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gojfhrukd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gbetwblup.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gybzjxogn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gklyplgmp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/giicfwzom.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gqmhntjip.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gokpmuhpl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/glgtoefwu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gxogvdhnu.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gbvicyrvh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gpsjqikha.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gnythxkdl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/ghpjapxag.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gepcevhag.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/grsvteprt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gmymgzqsv.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gxkahpvba.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/grxjwrgst.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gaamjkuwf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gahttgcwk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gqlulcwkj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gpaijdifa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gupzubpwe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gocsmqllb.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gyhafbayk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gyjsbebid.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gmjeqqmvh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gijtfccrj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gdflcpzue.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gahjjrtlv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gyqjhwbnn.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gdyvrpidw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gzijlbrnn.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gqyoxtbzg.sHtML


<!-- 参考信息 -->