代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://on.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ws.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://aa.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mx.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wl.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://pg.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://kl.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zd.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wg.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hm.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uk.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://xd.haigaiapp.cn

Ruby: arr.sort
来源：http://io.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://op.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://iz.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xm.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://pc.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jj.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://us.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ds.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pu.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jt.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://el.chemitech.net.cn

[N04] 斐波那契数列
来源：http://jq.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pg.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cg.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wu.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nc.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fd.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fa.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fs.haigaiapp.cn

[N05] 最大公约数
来源：http://av.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://jn.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iq.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xa.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zc.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hi.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vp.nszjky.cn

Ruby: a.gcd(b)
来源：http://pp.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mq.bjjhwx.cn

[N06] 判断回文字符串
来源：http://bd.nicolike.cn

Py:   s == s[::-1]
来源：http://to.colortex.cn

PHP:  $s === strrev($s);
来源：http://fl.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://bf.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://qi.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ti.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://ke.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://gk.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qn.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://wv.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rm.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://un.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wi.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://qn.huanxung.cn

Java: // 手写 HashMap
来源：http://rc.nszjky.cn

Go:   // 手写 map[int]int
来源：http://ao.9csxet.cn

Ruby: // 手写 Hash
来源：http://tu.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fa.newstarts.cn

[N08] 生成全排列
来源：http://qr.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://yf.9csxet.cn

PHP:  // 手写递归交换
来源：http://kx.szxytkj.cn

JS:   // 手写回溯递归
来源：http://uv.szxytkj.cn

TS:   // 手写回溯递归
来源：http://bi.shtwfgs.cn

Java: // 手写回溯递归
来源：http://vb.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://hh.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://ee.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://yz.panjiajie.cn

[N09] 栈与队列
来源：http://he.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fj.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ob.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ap.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hx.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lo.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gu.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lh.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ua.wgjwhj.cn

[N10] 链表节点定义
来源：http://lb.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://be.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://au.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bs.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qp.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://uw.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rt.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qu.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://er.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://tq.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ra.newstarts.cn

PHP:  // 手写递归函数
来源：http://km.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://or.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xq.chemitech.net.cn

Java: // 手写递归
来源：http://os.asd995.cn

Go:   // 手写递归
来源：http://oh.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://os.hnjuh.cn

C#:   // 手写递归
来源：http://xk.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://im.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ac.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rw.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rd.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sr.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://py.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qq.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gh.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uh.szsharing.cn

================================================================================
来源：http://jl.shtwfgs.cn

O. 并发与异步
来源：http://dv.newstarts.cn

================================================================================
来源：http://al.colortex.cn

[O01] 启动一个线程
来源：http://yh.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bb.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bp.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ft.hahajie.cn

TS:   // 同 JS
来源：http://zv.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://wa.bookmarksfly.cn

Go:   go f()
来源：http://je.hnjuh.cn

Ruby: Thread.new { f }
来源：http://cg.nicolike.cn

C#:   Task.Run(() => F());
来源：http://bg.haigaiapp.cn

[O02] 使用线程池
来源：http://mz.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vp.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kw.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://id.huanxung.cn

TS:   // worker_threads 线程池
来源：http://ox.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://js.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tp.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ai.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ot.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://bo.szxytkj.cn

Py:   with lock: shared += 1
来源：http://oh.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://xh.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://es.szsharing.cn

TS:   // 同 JS
来源：http://zl.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://wu.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jm.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hd.521024.cn

C#:   lock (gate) { shared++; }
来源：http://lp.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://ev.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://hd.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kb.asd995.cn

JS:   async function f() { await g(); }
来源：http://me.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bx.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://al.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kp.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jx.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://wz.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://qk.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://pm.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rj.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://ge.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://yk.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://op.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hk.hahajie.cn

Ruby: threads.map(&:join)
来源：http://fu.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tq.521024.cn

[O06] 使用进程池
来源：http://jj.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://es.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bk.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://hy.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://fl.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nx.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cz.gzmigu.cn

Ruby: // fork 块
来源：http://jc.huanxung.cn

C#:   Parallel.For
来源：http://jt.panjiajie.cn

================================================================================
来源：http://fw.shtwfgs.cn

P. 常用工具函数
来源：http://vz.521024.cn

================================================================================
来源：http://yi.hnjuh.cn

[P01] 生成 UUID
来源：http://ei.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://wl.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ua.nicolike.cn

JS:   crypto.randomUUID()
来源：http://ec.asd995.cn

TS:   crypto.randomUUID()
来源：http://ms.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://jq.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://kh.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://jz.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://lm.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://ht.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yh.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nn.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gk.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aa.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qa.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dn.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ms.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ur.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://gn.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gg.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fw.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://io.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://az.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nu.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zq.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qw.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yu.bjjhwx.cn

[P04] 求长度
来源：http://jc.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bu.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xa.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gf.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ww.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://jf.newstarts.cn

Go:   len(arr);  len(m)
来源：http://ow.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://sk.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://og.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://tx.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wf.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sa.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jl.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ms.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vc.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ju.bookmarksfly.cn

Ruby: a == b
来源：http://uf.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://je.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zw.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ae.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://gc.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lg.9csxet.cn

TS:   if (x == null) {}
来源：http://gk.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cd.nszjky.cn

Go:   if x == nil {}
来源：http://em.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wu.lnxyls.cn

C#:   if (x is null) {}
来源：http://jg.gzmigu.cn

[P07] 防抖与节流
来源：http://mc.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ra.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://ga.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pc.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oj.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kd.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pq.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ig.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ws.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://id.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xf.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ko.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rf.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mi.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gy.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gh.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fj.szsharing.cn

================================================================================
来源：http://fa.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://no.9csxet.cn

================================================================================
来源：http://xb.shxzskj.cn

[Q01] 创建表
来源：http://ha.hahajie.cn

CREATE TABLE users (
来源：http://sv.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ny.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://qd.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://kw.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mb.newstarts.cn

);
来源：http://lc.lnxyls.cn

[Q02] 创建带外键的表
来源：http://kz.huanxung.cn

CREATE TABLE orders (
来源：http://ha.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mh.hnjuh.cn

user_id INT NOT NULL,
来源：http://ct.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://np.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dh.chemitech.net.cn

);
来源：http://be.hnjuh.cn

[Q03] 增加列
来源：http://kc.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wl.9csxet.cn

[Q04] 修改列类型
来源：http://xd.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://il.huixiangedu.cn

[Q05] 重命名列
来源：http://fa.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cp.wgjwhj.cn

[Q06] 删除列
来源：http://lu.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yo.9csxet.cn

[Q07] 删除表
来源：http://yc.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://me.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://ai.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fr.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://qs.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yj.nicolike.cn

[Q10] 插入单行
来源：http://do.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qk.shtwfgs.cn

[Q11] 一次插入多行
来源：http://zj.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://de.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://ej.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ob.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ud.lnxyls.cn

[Q13] 忽略重复插入
来源：http://qo.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qh.521024.cn

[Q14] 存在则更新（upsert）
来源：http://me.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qn.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rr.nicolike.cn

[Q15] 查询全部
来源：http://zo.hahajie.cn

SELECT * FROM users;
来源：http://lo.wgjwhj.cn

[Q16] 查询指定列
来源：http://cs.shtwfgs.cn

SELECT id, name FROM users;
来源：http://su.nicolike.cn

[Q17] 条件查询
来源：http://oe.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yu.huixiangedu.cn

[Q18] 模糊匹配
来源：http://it.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hp.jianghongdianzi.cn

[Q19] 范围查询
来源：http://dl.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qz.lnxyls.cn

[Q20] IN 列表
来源：http://mr.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eq.nicolike.cn

[Q21] 空值判断
来源：http://oc.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ax.huanxung.cn

[Q22] 排序
来源：http://so.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hi.nszjky.cn

[Q23] 分页
来源：http://cp.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wj.szsharing.cn

[Q24] 去重
来源：http://fj.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://dc.huanxung.cn

[Q25] 只取前 N 条
来源：http://kc.9csxet.cn


<!-- 参考信息 -->