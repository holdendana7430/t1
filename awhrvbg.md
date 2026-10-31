代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pd.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://an.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://rf.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ki.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ih.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://fn.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ux.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jr.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tw.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://to.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ig.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://ox.newstarts.cn

Ruby: arr.sort
来源：http://mw.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ov.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://ii.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ad.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://oy.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xq.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hl.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fq.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mg.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uu.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://df.szxytkj.cn

[N04] 斐波那契数列
来源：http://mz.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kt.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ht.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gu.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wm.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ij.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gj.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rz.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mv.shxzskj.cn

[N05] 最大公约数
来源：http://qu.huanxung.cn

Py:   math.gcd(a, b)
来源：http://mk.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://da.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fj.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wk.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wn.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://er.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://hm.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oi.9csxet.cn

[N06] 判断回文字符串
来源：http://rr.muxihuayi.cn

Py:   s == s[::-1]
来源：http://da.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://xq.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://di.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://jl.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://di.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://vv.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ub.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wb.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://gx.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pr.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jc.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://os.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://fq.nicolike.cn

Java: // 手写 HashMap
来源：http://kx.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://zb.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://st.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://us.shxzskj.cn

[N08] 生成全排列
来源：http://fe.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://ri.asd995.cn

PHP:  // 手写递归交换
来源：http://wl.521024.cn

JS:   // 手写回溯递归
来源：http://ze.huanxung.cn

TS:   // 手写回溯递归
来源：http://ih.jctech888.com.cn

Java: // 手写回溯递归
来源：http://pg.nicolike.cn

Go:   // 手写回溯递归
来源：http://la.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ng.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://rn.hnjuh.cn

[N09] 栈与队列
来源：http://qd.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qm.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://px.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://la.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fm.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ln.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://he.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ij.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ct.shtwfgs.cn

[N10] 链表节点定义
来源：http://fo.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://da.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://we.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rw.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bg.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://go.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lg.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://it.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wx.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://zd.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xn.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://ty.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yt.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gx.lnxyls.cn

Java: // 手写递归
来源：http://sm.521024.cn

Go:   // 手写递归
来源：http://gb.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hj.bookmarksfly.cn

C#:   // 手写递归
来源：http://ej.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gh.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gx.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bl.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sw.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dz.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ol.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ja.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pd.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sq.hnjuh.cn

================================================================================
来源：http://bj.chemitech.net.cn

O. 并发与异步
来源：http://mg.muxihuayi.cn

================================================================================
来源：http://xz.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://ze.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ij.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ew.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eo.haigaiapp.cn

TS:   // 同 JS
来源：http://dh.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://zp.nszjky.cn

Go:   go f()
来源：http://ws.nszjky.cn

Ruby: Thread.new { f }
来源：http://ef.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://uv.colortex.cn

[O02] 使用线程池
来源：http://kp.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ox.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rf.newstarts.cn

JS:   // worker_threads 线程池
来源：http://iu.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://sb.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xf.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hv.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zo.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sr.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://kk.shxzskj.cn

Py:   with lock: shared += 1
来源：http://ku.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://uq.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zx.bjjhwx.cn

TS:   // 同 JS
来源：http://jl.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://kl.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pm.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cd.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://rd.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://sr.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://vl.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kn.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://xm.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uv.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hc.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gu.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ds.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://oi.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://cj.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://bf.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oo.colortex.cn

JS:   await Promise.all(tasks)
来源：http://le.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://mz.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gv.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jq.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://yt.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yc.huanxung.cn

[O06] 使用进程池
来源：http://ng.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xj.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bb.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://da.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://ic.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ps.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pr.bjjhwx.cn

Ruby: // fork 块
来源：http://uw.huixinmuqiang.cn

C#:   Parallel.For
来源：http://di.shxzukj.cn

================================================================================
来源：http://xv.asd995.cn

P. 常用工具函数
来源：http://ag.shtwfgs.cn

================================================================================
来源：http://ix.huanxung.cn

[P01] 生成 UUID
来源：http://sc.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://hd.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ct.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://iq.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://bi.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://uw.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://zf.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://nv.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://fw.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://eb.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ml.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pj.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pa.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xu.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bb.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kw.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fc.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eh.lnxyls.cn

[P03] 生成短随机字符串
来源：http://go.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qi.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xv.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oo.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://md.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nl.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rq.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ur.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bl.newstarts.cn

[P04] 求长度
来源：http://qs.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ij.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://co.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qr.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ey.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://sb.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://aa.newstarts.cn

Ruby: x.length;  x.size
来源：http://he.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wt.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://bk.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ks.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nh.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yy.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qp.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rz.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eu.shtwfgs.cn

Ruby: a == b
来源：http://el.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bu.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yh.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sd.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://zq.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://py.chemitech.net.cn

TS:   if (x == null) {}
来源：http://er.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ll.gzmigu.cn

Go:   if x == nil {}
来源：http://dq.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yq.nszjky.cn

C#:   if (x is null) {}
来源：http://xk.yuexingan06.cn

[P07] 防抖与节流
来源：http://ca.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hb.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://bx.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://la.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xx.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dz.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jq.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qg.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ca.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://qv.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ob.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ul.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aa.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tw.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qe.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ii.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xf.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wr.nicolike.cn

================================================================================
来源：http://gm.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kk.jctech888.com.cn

================================================================================
来源：http://cs.szxytkj.cn

[Q01] 创建表
来源：http://su.wgjwhj.cn

CREATE TABLE users (
来源：http://ua.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bi.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://db.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://xu.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lp.huixiangedu.cn

);
来源：http://wj.asd995.cn

[Q02] 创建带外键的表
来源：http://tz.9csxet.cn

CREATE TABLE orders (
来源：http://bm.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yw.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://wg.nicolike.cn

amount DECIMAL(10, 2),
来源：http://cc.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wf.bookmarksfly.cn

);
来源：http://vu.nicolike.cn

[Q03] 增加列
来源：http://cf.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fr.shxzskj.cn

[Q04] 修改列类型
来源：http://sx.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rf.asd995.cn

[Q05] 重命名列
来源：http://gh.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jf.wgjwhj.cn

[Q06] 删除列
来源：http://ax.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cx.lnxyls.cn

[Q07] 删除表
来源：http://xq.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://dt.muxihuayi.cn

[Q08] 创建普通索引
来源：http://hd.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fg.lnxyls.cn

[Q09] 创建唯一索引
来源：http://bo.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lm.9csxet.cn

[Q10] 插入单行
来源：http://fp.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lh.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://vf.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vy.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://nj.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://je.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ol.asd995.cn

[Q13] 忽略重复插入
来源：http://br.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mj.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://ks.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ig.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mm.shxzukj.cn

[Q15] 查询全部
来源：http://kx.521024.cn

SELECT * FROM users;
来源：http://jw.521024.cn

[Q16] 查询指定列
来源：http://wl.colortex.cn

SELECT id, name FROM users;
来源：http://xi.lnxyls.cn

[Q17] 条件查询
来源：http://fp.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ki.shxzukj.cn

[Q18] 模糊匹配
来源：http://yt.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lz.nszjky.cn

[Q19] 范围查询
来源：http://fw.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xj.lnxyls.cn

[Q20] IN 列表
来源：http://qv.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://en.shxzukj.cn

[Q21] 空值判断
来源：http://sl.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://me.yuexingan06.cn

[Q22] 排序
来源：http://ns.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ce.shxzukj.cn

[Q23] 分页
来源：http://cb.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wt.yuntaijiaju.cn

[Q24] 去重
来源：http://ve.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ka.521024.cn

[Q25] 只取前 N 条
来源：http://jn.nicolike.cn


<!-- 参考信息 -->