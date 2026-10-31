代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://wn.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ty.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://th.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://op.huixinmuqiang.cn

Ruby: arr.sort
来源：http://kx.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ti.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://ts.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zj.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://sh.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wo.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pq.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://an.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ro.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ov.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ww.lnxyls.cn

[N04] 斐波那契数列
来源：http://un.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://is.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nr.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oo.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://an.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qo.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lx.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wa.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ej.jctech888.com.cn

[N05] 最大公约数
来源：http://is.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://qx.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ld.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vh.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mi.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ab.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fx.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://mz.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cy.521024.cn

[N06] 判断回文字符串
来源：http://tx.muxihuayi.cn

Py:   s == s[::-1]
来源：http://gj.nicolike.cn

PHP:  $s === strrev($s);
来源：http://hg.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://nb.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://rr.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lp.hahajie.cn

Go:   // 双指针从两端比较
来源：http://ys.szxytkj.cn

Ruby: s == s.reverse
来源：http://zu.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tq.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://rx.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ip.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xe.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vn.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://jk.bjjhwx.cn

Java: // 手写 HashMap
来源：http://up.asd995.cn

Go:   // 手写 map[int]int
来源：http://kr.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://mv.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://of.bookmarksfly.cn

[N08] 生成全排列
来源：http://sa.asd995.cn

Py:   itertools.permutations(arr)
来源：http://ca.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://kr.hnjuh.cn

JS:   // 手写回溯递归
来源：http://iw.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://ev.9csxet.cn

Java: // 手写回溯递归
来源：http://tm.panjiajie.cn

Go:   // 手写回溯递归
来源：http://cm.colortex.cn

Ruby: arr.permutation.to_a
来源：http://uu.521024.cn

C#:   // 手写回溯递归
来源：http://ee.huixinmuqiang.cn

[N09] 栈与队列
来源：http://zc.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bj.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aa.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://li.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://po.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ho.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yy.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vd.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wk.newstarts.cn

[N10] 链表节点定义
来源：http://wd.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qd.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wa.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gm.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kw.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://tx.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zp.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ga.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qu.521024.cn

[N11] 二叉树中序遍历
来源：http://ks.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ap.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://xf.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://it.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://il.nicolike.cn

Java: // 手写递归
来源：http://zg.huixinmuqiang.cn

Go:   // 手写递归
来源：http://de.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uy.hahajie.cn

C#:   // 手写递归
来源：http://ws.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qo.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wu.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://np.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fg.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zw.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zu.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wv.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://re.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zh.bjjhwx.cn

================================================================================
来源：http://dy.muxihuayi.cn

O. 并发与异步
来源：http://wa.newstarts.cn

================================================================================
来源：http://iz.521024.cn

[O01] 启动一个线程
来源：http://lp.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yp.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nb.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ez.yuexingan06.cn

TS:   // 同 JS
来源：http://uj.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://fa.yuexingan06.cn

Go:   go f()
来源：http://ed.nicolike.cn

Ruby: Thread.new { f }
来源：http://cs.asd995.cn

C#:   Task.Run(() => F());
来源：http://zo.521024.cn

[O02] 使用线程池
来源：http://qj.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lo.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dh.newstarts.cn

JS:   // worker_threads 线程池
来源：http://oy.nszjky.cn

TS:   // worker_threads 线程池
来源：http://zk.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vf.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sr.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fe.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eh.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://sx.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://it.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://yp.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://co.lnxyls.cn

TS:   // 同 JS
来源：http://rz.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://eg.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gu.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yr.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://rm.nszjky.cn

[O04] 定义异步函数并等待
来源：http://yf.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://rh.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fe.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://ii.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fi.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cv.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kt.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cq.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://go.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://sb.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://az.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://db.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://ny.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://di.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fy.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yf.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://vw.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ff.lnxyls.cn

[O06] 使用进程池
来源：http://ot.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://et.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bg.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://vq.colortex.cn

TS:   // child_process / cluster 模块
来源：http://tw.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ed.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uj.jianghongdianzi.cn

Ruby: // fork 块
来源：http://vp.huixiangedu.cn

C#:   Parallel.For
来源：http://ak.newstarts.cn

================================================================================
来源：http://vy.bookmarksfly.cn

P. 常用工具函数
来源：http://iv.nicolike.cn

================================================================================
来源：http://ua.haigaiapp.cn

[P01] 生成 UUID
来源：http://lw.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://xf.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ep.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://hg.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://mp.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://jk.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://ea.521024.cn

Ruby: SecureRandom.uuid
来源：http://nu.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://tx.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://ty.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hr.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tt.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yx.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bg.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ju.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dw.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lu.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ql.521024.cn

[P03] 生成短随机字符串
来源：http://bo.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yl.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xr.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rm.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oq.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yi.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://at.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://em.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dx.bookmarksfly.cn

[P04] 求长度
来源：http://vx.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ps.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fx.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kb.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yw.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://hd.9csxet.cn

Go:   len(arr);  len(m)
来源：http://zq.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://qn.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://st.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://ev.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zx.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bt.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bi.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ga.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ja.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kk.szxytkj.cn

Ruby: a == b
来源：http://tp.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pw.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gw.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jr.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://jn.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kl.asd995.cn

TS:   if (x == null) {}
来源：http://xx.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://oq.wgjwhj.cn

Go:   if x == nil {}
来源：http://tm.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kt.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://zn.jctech888.com.cn

[P07] 防抖与节流
来源：http://uu.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qi.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://xm.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://if.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ol.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hw.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ya.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ht.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nd.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://iq.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ou.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hk.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bq.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ad.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xo.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vj.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mi.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://se.huanxung.cn

================================================================================
来源：http://by.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lu.hahajie.cn

================================================================================
来源：http://kf.521024.cn

[Q01] 创建表
来源：http://gz.newstarts.cn

CREATE TABLE users (
来源：http://zi.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://go.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ea.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://ev.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lj.haigaiapp.cn

);
来源：http://ic.9csxet.cn

[Q02] 创建带外键的表
来源：http://mh.haigaiapp.cn

CREATE TABLE orders (
来源：http://id.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bq.szxytkj.cn

user_id INT NOT NULL,
来源：http://hz.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://ul.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lz.newstarts.cn

);
来源：http://af.muxihuayi.cn

[Q03] 增加列
来源：http://pm.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cp.lnxyls.cn

[Q04] 修改列类型
来源：http://st.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zu.haigaiapp.cn

[Q05] 重命名列
来源：http://hs.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qa.gzmigu.cn

[Q06] 删除列
来源：http://id.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wt.huanxung.cn

[Q07] 删除表
来源：http://as.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://ax.newstarts.cn

[Q08] 创建普通索引
来源：http://kg.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sm.colortex.cn

[Q09] 创建唯一索引
来源：http://ln.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yt.huixiangedu.cn

[Q10] 插入单行
来源：http://bt.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://un.szsharing.cn

[Q11] 一次插入多行
来源：http://yt.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vw.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://ht.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zv.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://th.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://el.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xq.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://jn.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vs.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://is.huanxung.cn

[Q15] 查询全部
来源：http://tj.hnjuh.cn

SELECT * FROM users;
来源：http://cq.bjjhwx.cn

[Q16] 查询指定列
来源：http://pb.bjjhwx.cn

SELECT id, name FROM users;
来源：http://si.shtwfgs.cn

[Q17] 条件查询
来源：http://nk.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bi.bjjhwx.cn

[Q18] 模糊匹配
来源：http://sj.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bf.shtwfgs.cn

[Q19] 范围查询
来源：http://jn.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fu.yuexingan06.cn

[Q20] IN 列表
来源：http://oi.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ot.shxzskj.cn

[Q21] 空值判断
来源：http://hg.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://an.panjiajie.cn

[Q22] 排序
来源：http://oz.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vw.hnjuh.cn

[Q23] 分页
来源：http://tu.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://al.newstarts.cn

[Q24] 去重
来源：http://kr.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://xu.szsharing.cn

[Q25] 只取前 N 条
来源：http://ka.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://or.wgjwhj.cn

[Q26] 计数
来源：http://dc.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://vk.lnxyls.cn

[Q27] 条件计数
来源：http://nn.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vz.yuexingan06.cn

[Q28] 求和与平均
来源：http://et.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rd.asd995.cn

[Q29] 最大最小值
来源：http://qd.szsharing.cn


<!-- 参考信息 -->