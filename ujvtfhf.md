代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://uc.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://yg.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://fl.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://os.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vi.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mw.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xy.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://mq.bjjhwx.cn

Ruby: arr.sort
来源：http://ih.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jb.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://of.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uy.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://eq.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dd.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ym.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kc.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bh.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://se.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fu.lnxyls.cn

[N04] 斐波那契数列
来源：http://ek.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ox.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ea.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ps.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lm.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mh.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zj.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uv.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ga.shxzskj.cn

[N05] 最大公约数
来源：http://kb.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://oh.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eu.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uh.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ag.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://je.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nr.szxytkj.cn

Ruby: a.gcd(b)
来源：http://bo.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nj.shxzskj.cn

[N06] 判断回文字符串
来源：http://fb.shxzskj.cn

Py:   s == s[::-1]
来源：http://fm.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://uc.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://op.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://rj.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wp.nicolike.cn

Go:   // 双指针从两端比较
来源：http://fh.chemitech.net.cn

Ruby: s == s.reverse
来源：http://hz.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jp.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://oq.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fq.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tf.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zq.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://cr.newstarts.cn

Java: // 手写 HashMap
来源：http://xd.nszjky.cn

Go:   // 手写 map[int]int
来源：http://ko.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://vg.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rs.hnjuh.cn

[N08] 生成全排列
来源：http://qt.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://fy.hnjuh.cn

PHP:  // 手写递归交换
来源：http://qh.asd995.cn

JS:   // 手写回溯递归
来源：http://vq.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://cr.muxihuayi.cn

Java: // 手写回溯递归
来源：http://un.hahajie.cn

Go:   // 手写回溯递归
来源：http://wv.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://wu.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://wm.9csxet.cn

[N09] 栈与队列
来源：http://cm.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zm.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wl.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fg.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ih.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rb.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ay.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vo.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gd.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://ql.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lt.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mm.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qx.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://if.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://jt.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://da.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ci.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://er.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://hn.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ha.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://ij.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hf.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wp.shxzskj.cn

Java: // 手写递归
来源：http://ez.newstarts.cn

Go:   // 手写递归
来源：http://xx.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rw.jianghongdianzi.cn

C#:   // 手写递归
来源：http://fq.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cj.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ns.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ow.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ca.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pc.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://is.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://so.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lf.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dj.haigaiapp.cn

================================================================================
来源：http://tu.haigaiapp.cn

O. 并发与异步
来源：http://tk.szxytkj.cn

================================================================================
来源：http://mf.asd995.cn

[O01] 启动一个线程
来源：http://ba.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fr.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yy.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ny.asd995.cn

TS:   // 同 JS
来源：http://ut.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://qk.nszjky.cn

Go:   go f()
来源：http://jd.szsharing.cn

Ruby: Thread.new { f }
来源：http://ca.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://bj.muxihuayi.cn

[O02] 使用线程池
来源：http://di.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kg.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uv.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://te.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://up.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sw.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vi.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ya.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mm.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://io.9csxet.cn

Py:   with lock: shared += 1
来源：http://mz.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://cn.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ss.yuexingan06.cn

TS:   // 同 JS
来源：http://nw.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://cj.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hh.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gq.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://ey.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://df.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://xe.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ij.9csxet.cn

JS:   async function f() { await g(); }
来源：http://zg.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hh.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pf.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://im.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hd.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://na.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://xq.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://rl.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iy.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://mc.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://gq.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yn.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sj.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ft.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iy.muxihuayi.cn

[O06] 使用进程池
来源：http://zm.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://on.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ek.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://wa.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ul.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bq.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uw.hnjuh.cn

Ruby: // fork 块
来源：http://eh.yuntaijiaju.cn

C#:   Parallel.For
来源：http://hk.bjjhwx.cn

================================================================================
来源：http://gh.9csxet.cn

P. 常用工具函数
来源：http://ej.shxzskj.cn

================================================================================
来源：http://ev.9csxet.cn

[P01] 生成 UUID
来源：http://gc.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://zz.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uo.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://ox.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://wn.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://we.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://he.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://qk.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://pz.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://mb.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oe.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jj.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ig.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qm.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ju.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fq.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dr.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ye.newstarts.cn

[P03] 生成短随机字符串
来源：http://ll.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ml.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ft.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://by.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jq.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://um.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bw.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kj.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yt.haigaiapp.cn

[P04] 求长度
来源：http://ys.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vm.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lq.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dh.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gs.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://ck.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://ht.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://ik.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yj.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://yz.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rk.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://le.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ag.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ja.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lj.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kn.bookmarksfly.cn

Ruby: a == b
来源：http://dq.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xd.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://me.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dl.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://dc.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nf.lnxyls.cn

TS:   if (x == null) {}
来源：http://la.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xk.muxihuayi.cn

Go:   if x == nil {}
来源：http://jn.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oj.wgjwhj.cn

C#:   if (x is null) {}
来源：http://gs.colortex.cn

[P07] 防抖与节流
来源：http://wb.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xs.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://oe.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rh.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wa.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yi.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pz.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qc.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pf.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://ry.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://je.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zz.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ij.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://om.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hu.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mn.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sz.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kr.chemitech.net.cn

================================================================================
来源：http://np.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ur.huixiangedu.cn

================================================================================
来源：http://mi.muxihuayi.cn

[Q01] 创建表
来源：http://uh.gzmigu.cn

CREATE TABLE users (
来源：http://ou.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xa.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://nk.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://eb.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jf.chemitech.net.cn

);
来源：http://ag.szsharing.cn

[Q02] 创建带外键的表
来源：http://wr.szxytkj.cn

CREATE TABLE orders (
来源：http://ee.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dc.chemitech.net.cn

user_id INT NOT NULL,
来源：http://ob.nszjky.cn

amount DECIMAL(10, 2),
来源：http://ce.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ig.yuntaijiaju.cn

);
来源：http://wf.haigaiapp.cn

[Q03] 增加列
来源：http://ih.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bs.szxytkj.cn

[Q04] 修改列类型
来源：http://ao.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gs.bookmarksfly.cn

[Q05] 重命名列
来源：http://fv.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fw.yuexingan06.cn

[Q06] 删除列
来源：http://nu.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jy.shxzukj.cn

[Q07] 删除表
来源：http://ns.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://wt.lnxyls.cn

[Q08] 创建普通索引
来源：http://dt.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ly.szxytkj.cn

[Q09] 创建唯一索引
来源：http://au.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pl.shtwfgs.cn

[Q10] 插入单行
来源：http://lz.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ts.shxzukj.cn

[Q11] 一次插入多行
来源：http://va.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gz.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://ns.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ab.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vg.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://fd.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ei.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://js.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gh.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zb.muxihuayi.cn

[Q15] 查询全部
来源：http://fd.huanxung.cn

SELECT * FROM users;
来源：http://sl.bookmarksfly.cn

[Q16] 查询指定列
来源：http://yy.bjjhwx.cn

SELECT id, name FROM users;
来源：http://ri.huixiangedu.cn

[Q17] 条件查询
来源：http://jb.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yd.panjiajie.cn

[Q18] 模糊匹配
来源：http://co.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://os.muxihuayi.cn

[Q19] 范围查询
来源：http://sy.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://de.colortex.cn

[Q20] IN 列表
来源：http://wl.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://om.shtwfgs.cn

[Q21] 空值判断
来源：http://hi.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ya.chemitech.net.cn

[Q22] 排序
来源：http://jb.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ms.hahajie.cn

[Q23] 分页
来源：http://hg.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aq.chemitech.net.cn

[Q24] 去重
来源：http://cm.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://zz.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://wj.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ow.521024.cn

[Q26] 计数
来源：http://zu.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://kn.huixiangedu.cn

[Q27] 条件计数
来源：http://qx.asd995.cn


<!-- 参考信息 -->