代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pk.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nx.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ke.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vc.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://df.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://uu.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://fy.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://js.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sk.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://em.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ln.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://pj.chemitech.net.cn

Ruby: arr.sort
来源：http://ok.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zi.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://ip.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lz.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://rv.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cj.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ef.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ok.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iy.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://at.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xj.shxzskj.cn

[N04] 斐波那契数列
来源：http://ga.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fx.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vz.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kl.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xa.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sz.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ch.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://je.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bw.hahajie.cn

[N05] 最大公约数
来源：http://zy.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://oh.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bm.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sb.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tf.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rk.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zq.hahajie.cn

Ruby: a.gcd(b)
来源：http://mf.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zl.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://xq.jctech888.com.cn

Py:   s == s[::-1]
来源：http://wo.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://vq.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://of.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ip.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xq.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://sp.panjiajie.cn

Ruby: s == s.reverse
来源：http://xm.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lz.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://hd.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ro.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tc.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bg.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://pv.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://nb.szsharing.cn

Go:   // 手写 map[int]int
来源：http://ru.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://kp.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qq.huanxung.cn

[N08] 生成全排列
来源：http://ji.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://xz.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://yc.9csxet.cn

JS:   // 手写回溯递归
来源：http://bf.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://rz.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://qd.9csxet.cn

Go:   // 手写回溯递归
来源：http://xm.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://wq.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://xn.bjjhwx.cn

[N09] 栈与队列
来源：http://ne.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cs.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lu.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uy.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gg.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lb.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fs.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lw.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vk.lnxyls.cn

[N10] 链表节点定义
来源：http://nc.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ex.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hg.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lb.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ey.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://xm.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hf.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kc.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yx.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://rv.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ek.colortex.cn

PHP:  // 手写递归函数
来源：http://in.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eg.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yi.asd995.cn

Java: // 手写递归
来源：http://av.nicolike.cn

Go:   // 手写递归
来源：http://ec.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uc.bookmarksfly.cn

C#:   // 手写递归
来源：http://oe.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jt.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ej.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xg.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hb.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bs.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vd.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dp.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hg.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iy.asd995.cn

================================================================================
来源：http://ll.nicolike.cn

O. 并发与异步
来源：http://dn.521024.cn

================================================================================
来源：http://gz.wgjwhj.cn

[O01] 启动一个线程
来源：http://of.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ns.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ms.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qi.gzmigu.cn

TS:   // 同 JS
来源：http://wp.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://ae.bookmarksfly.cn

Go:   go f()
来源：http://vx.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://mo.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://oo.shxzskj.cn

[O02] 使用线程池
来源：http://gz.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ff.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cp.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://zb.szsharing.cn

TS:   // worker_threads 线程池
来源：http://ry.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://az.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dc.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ne.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pd.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://dt.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://bn.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://cb.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lp.shxzskj.cn

TS:   // 同 JS
来源：http://wy.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://ui.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qu.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uy.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://ra.nicolike.cn

[O04] 定义异步函数并等待
来源：http://no.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://qp.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cd.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://ub.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ja.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fp.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sb.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ys.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://qz.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://zt.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://to.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ch.asd995.cn

JS:   await Promise.all(tasks)
来源：http://sm.colortex.cn

TS:   await Promise.all(tasks)
来源：http://ym.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ww.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xr.9csxet.cn

Ruby: threads.map(&:join)
来源：http://iv.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ix.nicolike.cn

[O06] 使用进程池
来源：http://bh.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gy.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ug.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://ak.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://xl.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wm.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wm.jctech888.com.cn

Ruby: // fork 块
来源：http://ee.muxihuayi.cn

C#:   Parallel.For
来源：http://el.newstarts.cn

================================================================================
来源：http://og.gzmigu.cn

P. 常用工具函数
来源：http://fm.shtwfgs.cn

================================================================================
来源：http://br.lnxyls.cn

[P01] 生成 UUID
来源：http://wt.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ay.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lh.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://us.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://kv.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://su.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://hs.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://am.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://lb.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://ah.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bg.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gl.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dc.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ex.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fl.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rd.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vn.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://so.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://eo.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://my.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nm.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://se.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ah.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jq.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://is.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qn.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gi.colortex.cn

[P04] 求长度
来源：http://bt.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sm.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sk.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cz.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kc.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://ed.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://yj.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://qk.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kv.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://qj.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://si.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xx.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iq.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ev.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zj.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bi.huanxung.cn

Ruby: a == b
来源：http://rz.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tz.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kc.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://il.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://bc.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uv.asd995.cn

TS:   if (x == null) {}
来源：http://ik.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qj.bookmarksfly.cn

Go:   if x == nil {}
来源：http://bu.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ag.hnjuh.cn

C#:   if (x is null) {}
来源：http://tc.huixiangedu.cn

[P07] 防抖与节流
来源：http://le.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://db.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://un.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wz.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://in.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://if.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xq.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ln.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pl.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://fv.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vd.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lz.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dt.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ie.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sm.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://al.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oq.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yk.bookmarksfly.cn

================================================================================
来源：http://rz.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pu.huanxung.cn

================================================================================
来源：http://mv.lnxyls.cn

[Q01] 创建表
来源：http://ib.nicolike.cn

CREATE TABLE users (
来源：http://sm.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zr.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://qa.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://aq.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pc.hahajie.cn

);
来源：http://mv.huanxung.cn

[Q02] 创建带外键的表
来源：http://gi.szsharing.cn

CREATE TABLE orders (
来源：http://zu.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xz.wgjwhj.cn

user_id INT NOT NULL,
来源：http://gp.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://im.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zx.jianghongdianzi.cn

);
来源：http://nm.asd995.cn

[Q03] 增加列
来源：http://zf.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mi.jctech888.com.cn

[Q04] 修改列类型
来源：http://fv.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iw.huixinmuqiang.cn

[Q05] 重命名列
来源：http://sd.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mo.hnjuh.cn

[Q06] 删除列
来源：http://xq.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lv.szsharing.cn

[Q07] 删除表
来源：http://gk.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://wq.nicolike.cn

[Q08] 创建普通索引
来源：http://oq.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xq.nszjky.cn

[Q09] 创建唯一索引
来源：http://wj.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://se.panjiajie.cn

[Q10] 插入单行
来源：http://yo.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dy.jctech888.com.cn

[Q11] 一次插入多行
来源：http://uk.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mz.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://jp.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ve.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jo.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://pf.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xf.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://bl.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ht.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qm.nicolike.cn

[Q15] 查询全部
来源：http://ek.muxihuayi.cn

SELECT * FROM users;
来源：http://gx.nicolike.cn

[Q16] 查询指定列
来源：http://lk.yuexingan06.cn

SELECT id, name FROM users;
来源：http://cw.huixinmuqiang.cn

[Q17] 条件查询
来源：http://xa.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iy.shxzskj.cn

[Q18] 模糊匹配
来源：http://uq.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cv.yuexingan06.cn

[Q19] 范围查询
来源：http://dj.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sc.shxzskj.cn

[Q20] IN 列表
来源：http://bd.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://po.shxzskj.cn

[Q21] 空值判断
来源：http://xp.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ei.jianghongdianzi.cn

[Q22] 排序
来源：http://vi.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ul.huixinmuqiang.cn

[Q23] 分页
来源：http://ef.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gg.bjjhwx.cn

[Q24] 去重
来源：http://fi.521024.cn

SELECT DISTINCT city FROM users;
来源：http://zc.hnjuh.cn

[Q25] 只取前 N 条
来源：http://tq.hnjuh.cn


<!-- 参考信息 -->