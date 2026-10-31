代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://zs.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zp.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ho.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://op.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nb.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zy.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bi.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://sa.szsharing.cn

Ruby: arr.sort
来源：http://iq.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rx.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://pe.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pc.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://hv.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yo.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hb.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wk.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kl.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ap.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rw.yuexingan06.cn

[N04] 斐波那契数列
来源：http://wz.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lz.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mh.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mf.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sb.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://du.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tt.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rz.nicolike.cn

[N05] 最大公约数
来源：http://ar.asd995.cn

Py:   math.gcd(a, b)
来源：http://nq.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mz.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kb.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xm.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qg.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wm.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://ku.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jm.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://rp.hahajie.cn

Py:   s == s[::-1]
来源：http://ix.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://oe.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://xf.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://rr.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://je.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://hl.szxytkj.cn

Ruby: s == s.reverse
来源：http://dq.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ld.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://xx.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zy.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vt.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ii.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://yp.shxzukj.cn

Java: // 手写 HashMap
来源：http://id.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://in.gzmigu.cn

Ruby: // 手写 Hash
来源：http://bm.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pt.colortex.cn

[N08] 生成全排列
来源：http://kx.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://wv.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://eu.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://jd.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://lx.hnjuh.cn

Java: // 手写回溯递归
来源：http://nm.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://gj.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://zb.gzmigu.cn

C#:   // 手写回溯递归
来源：http://ft.huixiangedu.cn

[N09] 栈与队列
来源：http://ep.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://li.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ag.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://og.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hy.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wp.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hm.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://na.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bp.huixiangedu.cn

[N10] 链表节点定义
来源：http://ac.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bw.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pe.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ab.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fb.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://mf.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ay.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rx.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ym.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://en.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eo.szxytkj.cn

PHP:  // 手写递归函数
来源：http://go.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fw.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://up.yuexingan06.cn

Java: // 手写递归
来源：http://zn.shxzukj.cn

Go:   // 手写递归
来源：http://dv.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nb.wgjwhj.cn

C#:   // 手写递归
来源：http://wx.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ii.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rp.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ff.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nu.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mr.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yd.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lt.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ic.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iq.wgjwhj.cn

================================================================================
来源：http://ek.jianghongdianzi.cn

O. 并发与异步
来源：http://hp.shxzskj.cn

================================================================================
来源：http://dm.lnxyls.cn

[O01] 启动一个线程
来源：http://tn.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zg.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kd.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://os.szsharing.cn

TS:   // 同 JS
来源：http://go.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://pw.huixinmuqiang.cn

Go:   go f()
来源：http://vr.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://lb.huanxung.cn

C#:   Task.Run(() => F());
来源：http://yz.huixinmuqiang.cn

[O02] 使用线程池
来源：http://bb.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ws.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://js.newstarts.cn

JS:   // worker_threads 线程池
来源：http://is.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://rm.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ot.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xq.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kk.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sw.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://za.shxzukj.cn

Py:   with lock: shared += 1
来源：http://qq.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://vf.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jp.huixiangedu.cn

TS:   // 同 JS
来源：http://dc.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://bt.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ku.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sf.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://cu.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://ii.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://os.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sm.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://lj.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://am.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://si.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://se.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://az.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://rr.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://bg.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://lq.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oo.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://lt.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://ol.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ao.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xm.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://qc.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rm.newstarts.cn

[O06] 使用进程池
来源：http://bf.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uz.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xa.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://qg.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://wm.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hr.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sp.hnjuh.cn

Ruby: // fork 块
来源：http://qf.wgjwhj.cn

C#:   Parallel.For
来源：http://sl.yuexingan06.cn

================================================================================
来源：http://vn.bjjhwx.cn

P. 常用工具函数
来源：http://zq.nicolike.cn

================================================================================
来源：http://qg.shtwfgs.cn

[P01] 生成 UUID
来源：http://yn.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://ax.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://my.521024.cn

JS:   crypto.randomUUID()
来源：http://tu.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://ff.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://zq.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://qu.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://ri.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://kw.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://yp.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tg.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sm.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tn.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cv.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nw.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ev.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gn.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kn.521024.cn

[P03] 生成短随机字符串
来源：http://aq.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fv.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://io.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://va.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uq.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tf.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bc.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cr.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ch.lnxyls.cn

[P04] 求长度
来源：http://ye.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ox.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wa.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dl.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vp.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://hn.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://fz.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://ky.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xq.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://fj.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sh.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ts.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://un.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://de.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sf.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://on.colortex.cn

Ruby: a == b
来源：http://ty.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xv.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nj.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ij.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://to.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dc.hnjuh.cn

TS:   if (x == null) {}
来源：http://uk.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gu.asd995.cn

Go:   if x == nil {}
来源：http://rn.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wn.huixiangedu.cn

C#:   if (x is null) {}
来源：http://sa.szsharing.cn

[P07] 防抖与节流
来源：http://jk.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yx.colortex.cn

PHP:  // 手写时间戳比较
来源：http://zt.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hj.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wi.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://os.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ov.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gw.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tg.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://zp.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yn.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://il.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ju.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://op.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://md.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://od.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qa.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oi.yuntaijiaju.cn

================================================================================
来源：http://ke.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://be.asd995.cn

================================================================================
来源：http://jt.huixinmuqiang.cn

[Q01] 创建表
来源：http://sz.szsharing.cn

CREATE TABLE users (
来源：http://fi.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gm.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://be.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://es.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zt.chemitech.net.cn

);
来源：http://ff.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://mt.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://tn.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kd.shxzukj.cn

user_id INT NOT NULL,
来源：http://vn.9csxet.cn

amount DECIMAL(10, 2),
来源：http://da.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ym.szxytkj.cn

);
来源：http://hu.hahajie.cn

[Q03] 增加列
来源：http://lc.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xm.jctech888.com.cn

[Q04] 修改列类型
来源：http://uv.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gw.shxzskj.cn

[Q05] 重命名列
来源：http://ur.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kp.hahajie.cn

[Q06] 删除列
来源：http://vd.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nz.newstarts.cn

[Q07] 删除表
来源：http://nz.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://tg.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://wu.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fi.nszjky.cn

[Q09] 创建唯一索引
来源：http://iq.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ni.huanxung.cn

[Q10] 插入单行
来源：http://ru.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bi.nicolike.cn

[Q11] 一次插入多行
来源：http://ld.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nl.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://cf.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ke.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ed.shxzskj.cn

[Q13] 忽略重复插入
来源：http://tb.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ln.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://bm.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xi.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wi.shtwfgs.cn

[Q15] 查询全部
来源：http://aq.huixiangedu.cn

SELECT * FROM users;
来源：http://uu.muxihuayi.cn

[Q16] 查询指定列
来源：http://rq.lnxyls.cn

SELECT id, name FROM users;
来源：http://wt.hahajie.cn

[Q17] 条件查询
来源：http://hw.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wj.yuexingan06.cn

[Q18] 模糊匹配
来源：http://mj.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rg.szsharing.cn

[Q19] 范围查询
来源：http://gi.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dp.asd995.cn

[Q20] IN 列表
来源：http://vr.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ex.colortex.cn

[Q21] 空值判断
来源：http://oh.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://me.wgjwhj.cn

[Q22] 排序
来源：http://pu.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ci.haigaiapp.cn

[Q23] 分页
来源：http://wu.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oc.shxzskj.cn

[Q24] 去重
来源：http://ng.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://wg.szxytkj.cn

[Q25] 只取前 N 条
来源：http://iu.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://az.shxzukj.cn

[Q26] 计数
来源：http://av.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://pm.szsharing.cn

[Q27] 条件计数
来源：http://ou.chemitech.net.cn


<!-- 参考信息 -->