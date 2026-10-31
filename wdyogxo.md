代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ja.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vd.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://hq.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hl.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://er.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://vd.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://jp.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jk.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fy.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gk.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bo.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://qi.jctech888.com.cn

Ruby: arr.sort
来源：http://sb.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gj.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://yg.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cm.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://xs.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uq.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ty.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ll.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mr.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mj.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oj.szxytkj.cn

[N04] 斐波那契数列
来源：http://dl.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sq.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eu.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ht.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://im.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mk.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dp.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eb.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rh.shxzskj.cn

[N05] 最大公约数
来源：http://fb.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://wd.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mu.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vu.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://la.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vv.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ot.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://bi.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ct.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://qv.asd995.cn

Py:   s == s[::-1]
来源：http://nt.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://cu.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://nr.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://sl.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vy.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://xh.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://ew.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://om.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://kl.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sf.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zi.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fp.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://ts.haigaiapp.cn

Java: // 手写 HashMap
来源：http://sj.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://ft.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://ed.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://de.panjiajie.cn

[N08] 生成全排列
来源：http://yk.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://mm.szxytkj.cn

PHP:  // 手写递归交换
来源：http://jm.colortex.cn

JS:   // 手写回溯递归
来源：http://vo.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://vm.wgjwhj.cn

Java: // 手写回溯递归
来源：http://vg.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://mw.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://zu.szxytkj.cn

C#:   // 手写回溯递归
来源：http://sv.bookmarksfly.cn

[N09] 栈与队列
来源：http://eq.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ay.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vc.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xt.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wf.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ox.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tc.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mr.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://us.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://dh.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ka.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nl.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uk.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ye.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://ma.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yv.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fr.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://no.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://iu.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wk.szsharing.cn

PHP:  // 手写递归函数
来源：http://yj.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bp.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jk.shxzukj.cn

Java: // 手写递归
来源：http://by.lnxyls.cn

Go:   // 手写递归
来源：http://ni.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cm.asd995.cn

C#:   // 手写递归
来源：http://mz.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fp.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ti.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lu.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dj.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zl.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dn.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ch.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ed.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hb.huanxung.cn

================================================================================
来源：http://jj.gzmigu.cn

O. 并发与异步
来源：http://zi.yuntaijiaju.cn

================================================================================
来源：http://bi.bookmarksfly.cn

[O01] 启动一个线程
来源：http://ot.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://le.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zq.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mc.jctech888.com.cn

TS:   // 同 JS
来源：http://gv.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://jh.panjiajie.cn

Go:   go f()
来源：http://hp.lnxyls.cn

Ruby: Thread.new { f }
来源：http://nf.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://hj.lnxyls.cn

[O02] 使用线程池
来源：http://gr.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sb.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hc.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://we.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://be.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fu.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cc.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://er.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ur.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://ak.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://gt.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://dc.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ao.huixiangedu.cn

TS:   // 同 JS
来源：http://wf.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://ud.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rq.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hf.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://yd.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://ny.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://co.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nb.nicolike.cn

JS:   async function f() { await g(); }
来源：http://if.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://el.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kw.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wp.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mo.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://xe.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://zs.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://ua.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fh.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://gn.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://qs.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gl.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ab.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ju.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zn.nszjky.cn

[O06] 使用进程池
来源：http://xo.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ll.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tu.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://wz.colortex.cn

TS:   // child_process / cluster 模块
来源：http://ia.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://om.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pq.bjjhwx.cn

Ruby: // fork 块
来源：http://yd.panjiajie.cn

C#:   Parallel.For
来源：http://vo.yuexingan06.cn

================================================================================
来源：http://wu.lnxyls.cn

P. 常用工具函数
来源：http://jv.jctech888.com.cn

================================================================================
来源：http://ak.lnxyls.cn

[P01] 生成 UUID
来源：http://vk.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://ir.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ss.nszjky.cn

JS:   crypto.randomUUID()
来源：http://xl.9csxet.cn

TS:   crypto.randomUUID()
来源：http://fp.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://ha.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://vi.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://wa.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://bl.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://np.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ja.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zv.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pv.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ca.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dd.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pd.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xd.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zk.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://eq.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rl.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hj.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rt.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rf.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://na.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ql.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mz.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wz.bookmarksfly.cn

[P04] 求长度
来源：http://xn.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qt.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://do.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nj.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ih.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://cd.szsharing.cn

Go:   len(arr);  len(m)
来源：http://pq.hnjuh.cn

Ruby: x.length;  x.size
来源：http://pp.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hk.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://qs.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ed.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://el.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://si.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vw.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yw.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wx.huixinmuqiang.cn

Ruby: a == b
来源：http://bs.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nt.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jj.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ii.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://oe.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pm.gzmigu.cn

TS:   if (x == null) {}
来源：http://ka.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://up.asd995.cn

Go:   if x == nil {}
来源：http://gz.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sq.asd995.cn

C#:   if (x is null) {}
来源：http://pj.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://jy.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ew.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://es.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oj.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yf.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xw.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iu.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tx.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oo.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://wr.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://un.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kb.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dr.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ye.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wd.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bu.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wf.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iw.gzmigu.cn

================================================================================
来源：http://rf.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cz.wgjwhj.cn

================================================================================
来源：http://uq.panjiajie.cn

[Q01] 创建表
来源：http://cr.shxzskj.cn

CREATE TABLE users (
来源：http://sw.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ue.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://bg.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://jy.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qn.shtwfgs.cn

);
来源：http://le.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://me.colortex.cn

CREATE TABLE orders (
来源：http://fn.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hy.hnjuh.cn

user_id INT NOT NULL,
来源：http://ph.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://oz.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pv.hnjuh.cn

);
来源：http://zz.haigaiapp.cn

[Q03] 增加列
来源：http://wc.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://af.9csxet.cn

[Q04] 修改列类型
来源：http://pb.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qq.panjiajie.cn

[Q05] 重命名列
来源：http://fr.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dj.bjjhwx.cn

[Q06] 删除列
来源：http://iq.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sr.jianghongdianzi.cn

[Q07] 删除表
来源：http://gm.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://ez.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://kg.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uo.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://pk.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ui.521024.cn

[Q10] 插入单行
来源：http://og.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zi.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://kz.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yh.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://uo.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bp.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://em.hnjuh.cn

[Q13] 忽略重复插入
来源：http://zk.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vg.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://xi.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sl.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ir.szsharing.cn

[Q15] 查询全部
来源：http://vz.shtwfgs.cn

SELECT * FROM users;
来源：http://jp.bookmarksfly.cn

[Q16] 查询指定列
来源：http://ej.yuexingan06.cn

SELECT id, name FROM users;
来源：http://pm.bookmarksfly.cn

[Q17] 条件查询
来源：http://qq.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cl.nicolike.cn

[Q18] 模糊匹配
来源：http://ne.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ll.jianghongdianzi.cn

[Q19] 范围查询
来源：http://ox.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ta.asd995.cn

[Q20] IN 列表
来源：http://ow.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://on.shxzskj.cn

[Q21] 空值判断
来源：http://pp.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mo.wgjwhj.cn

[Q22] 排序
来源：http://ot.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cs.bjjhwx.cn

[Q23] 分页
来源：http://yb.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://va.gzmigu.cn

[Q24] 去重
来源：http://qa.521024.cn

SELECT DISTINCT city FROM users;
来源：http://eo.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://sr.hnjuh.cn


<!-- 参考信息 -->