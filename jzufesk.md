代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://xl.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://wk.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://xg.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://se.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ap.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lm.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://df.521024.cn

Go:   slices.Sort(arr)
来源：http://wp.shtwfgs.cn

Ruby: arr.sort
来源：http://kj.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://re.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://dc.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vf.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://yc.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eg.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vy.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tr.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yc.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hx.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://by.jctech888.com.cn

[N04] 斐波那契数列
来源：http://uv.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://id.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kd.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nf.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sn.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vq.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eb.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pb.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://df.nicolike.cn

[N05] 最大公约数
来源：http://xh.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://fn.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hh.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gb.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nd.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lt.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://br.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://oo.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ac.nszjky.cn

[N06] 判断回文字符串
来源：http://ax.szsharing.cn

Py:   s == s[::-1]
来源：http://wl.9csxet.cn

PHP:  $s === strrev($s);
来源：http://tl.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://nh.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://fk.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vq.521024.cn

Go:   // 双指针从两端比较
来源：http://wi.newstarts.cn

Ruby: s == s.reverse
来源：http://ps.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://la.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://nm.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yy.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ar.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gt.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://gf.lnxyls.cn

Java: // 手写 HashMap
来源：http://vh.9csxet.cn

Go:   // 手写 map[int]int
来源：http://ts.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://ib.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kp.gzmigu.cn

[N08] 生成全排列
来源：http://vu.521024.cn

Py:   itertools.permutations(arr)
来源：http://se.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://eb.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://dw.newstarts.cn

TS:   // 手写回溯递归
来源：http://gy.chemitech.net.cn

Java: // 手写回溯递归
来源：http://hg.panjiajie.cn

Go:   // 手写回溯递归
来源：http://uz.asd995.cn

Ruby: arr.permutation.to_a
来源：http://up.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://hm.huixiangedu.cn

[N09] 栈与队列
来源：http://ca.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cs.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hb.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ad.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yz.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zg.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wj.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mx.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fk.jctech888.com.cn

[N10] 链表节点定义
来源：http://wt.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gj.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uk.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ri.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ln.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://ua.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ze.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zw.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iw.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://xz.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hh.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://od.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uk.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sd.lnxyls.cn

Java: // 手写递归
来源：http://nl.wgjwhj.cn

Go:   // 手写递归
来源：http://ak.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://or.huanxung.cn

C#:   // 手写递归
来源：http://es.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fu.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://he.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wf.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yv.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zq.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xv.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iz.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wt.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qa.muxihuayi.cn

================================================================================
来源：http://mj.muxihuayi.cn

O. 并发与异步
来源：http://qs.shxzukj.cn

================================================================================
来源：http://zv.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://ob.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qk.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vq.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mu.bjjhwx.cn

TS:   // 同 JS
来源：http://dl.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://pj.bookmarksfly.cn

Go:   go f()
来源：http://ne.hnjuh.cn

Ruby: Thread.new { f }
来源：http://if.colortex.cn

C#:   Task.Run(() => F());
来源：http://ta.nszjky.cn

[O02] 使用线程池
来源：http://hm.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gc.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ez.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://xu.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://uc.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fr.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ho.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oe.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vl.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://hu.nszjky.cn

Py:   with lock: shared += 1
来源：http://xr.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ey.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nu.shxzskj.cn

TS:   // 同 JS
来源：http://mc.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://fe.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ip.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ws.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://cx.nszjky.cn

[O04] 定义异步函数并等待
来源：http://pz.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://fh.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lh.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://kz.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yf.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zh.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ob.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://an.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://xy.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://ko.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://xd.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ne.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://mb.colortex.cn

TS:   await Promise.all(tasks)
来源：http://wi.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://on.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qn.asd995.cn

Ruby: threads.map(&:join)
来源：http://pt.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wl.shxzskj.cn

[O06] 使用进程池
来源：http://cx.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jl.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jb.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://wz.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://df.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vi.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sw.haigaiapp.cn

Ruby: // fork 块
来源：http://zk.chemitech.net.cn

C#:   Parallel.For
来源：http://nv.bookmarksfly.cn

================================================================================
来源：http://na.lnxyls.cn

P. 常用工具函数
来源：http://ow.chemitech.net.cn

================================================================================
来源：http://vy.shxzukj.cn

[P01] 生成 UUID
来源：http://iy.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://oq.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tm.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://wl.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://ii.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://kp.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://hh.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://ga.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://wk.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://gv.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jw.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gf.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rc.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oc.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vw.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ut.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vn.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ol.colortex.cn

[P03] 生成短随机字符串
来源：http://va.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pd.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hp.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zi.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ju.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jw.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://az.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ec.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xy.huixinmuqiang.cn

[P04] 求长度
来源：http://fz.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yq.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ml.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wb.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fv.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://ub.521024.cn

Go:   len(arr);  len(m)
来源：http://bo.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://va.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rc.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://xo.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://op.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fe.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eq.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vz.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gu.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yr.colortex.cn

Ruby: a == b
来源：http://jy.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oq.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xm.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ep.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://ky.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jy.colortex.cn

TS:   if (x == null) {}
来源：http://at.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nt.shtwfgs.cn

Go:   if x == nil {}
来源：http://ey.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ph.haigaiapp.cn

C#:   if (x is null) {}
来源：http://wu.huanxung.cn

[P07] 防抖与节流
来源：http://yv.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pu.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://uh.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nw.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kw.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ir.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dv.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pz.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fv.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://tu.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wd.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oq.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hm.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yb.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ot.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://te.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ql.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://br.nszjky.cn

================================================================================
来源：http://dm.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fm.jianghongdianzi.cn

================================================================================
来源：http://tm.nszjky.cn

[Q01] 创建表
来源：http://nk.9csxet.cn

CREATE TABLE users (
来源：http://le.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tq.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://dy.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://wq.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mj.hahajie.cn

);
来源：http://zw.huanxung.cn

[Q02] 创建带外键的表
来源：http://nc.9csxet.cn

CREATE TABLE orders (
来源：http://ba.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ad.szxytkj.cn

user_id INT NOT NULL,
来源：http://mg.nszjky.cn

amount DECIMAL(10, 2),
来源：http://zw.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nw.szxytkj.cn

);
来源：http://pn.panjiajie.cn

[Q03] 增加列
来源：http://ok.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gw.bjjhwx.cn

[Q04] 修改列类型
来源：http://fk.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pb.gzmigu.cn

[Q05] 重命名列
来源：http://we.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ui.chemitech.net.cn

[Q06] 删除列
来源：http://fo.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ha.521024.cn

[Q07] 删除表
来源：http://st.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://oc.521024.cn

[Q08] 创建普通索引
来源：http://lb.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dy.nicolike.cn

[Q09] 创建唯一索引
来源：http://fj.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ut.huixiangedu.cn

[Q10] 插入单行
来源：http://cu.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jt.huanxung.cn

[Q11] 一次插入多行
来源：http://pn.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ij.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://fv.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ez.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zu.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://sg.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://be.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://ev.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hj.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ag.haigaiapp.cn

[Q15] 查询全部
来源：http://tx.asd995.cn

SELECT * FROM users;
来源：http://tl.yuexingan06.cn

[Q16] 查询指定列
来源：http://gv.shxzskj.cn

SELECT id, name FROM users;
来源：http://wc.hnjuh.cn

[Q17] 条件查询
来源：http://zv.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jv.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://fh.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gq.bjjhwx.cn

[Q19] 范围查询
来源：http://vd.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ku.jianghongdianzi.cn

[Q20] IN 列表
来源：http://jl.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ap.huanxung.cn

[Q21] 空值判断
来源：http://oj.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yp.haigaiapp.cn

[Q22] 排序
来源：http://ek.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wn.szsharing.cn

[Q23] 分页
来源：http://wp.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rs.muxihuayi.cn

[Q24] 去重
来源：http://td.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://qv.hahajie.cn

[Q25] 只取前 N 条
来源：http://eh.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vx.huixiangedu.cn

[Q26] 计数
来源：http://ie.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://rr.szxytkj.cn

[Q27] 条件计数
来源：http://tl.huanxung.cn


<!-- 参考信息 -->