代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://cd.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pz.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zo.newstarts.cn

Go:   slices.Sort(arr)
来源：http://hd.wgjwhj.cn

Ruby: arr.sort
来源：http://qe.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hx.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://nx.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ky.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ab.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xg.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ow.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vc.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dx.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://md.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xi.wgjwhj.cn

[N04] 斐波那契数列
来源：http://rx.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oo.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lq.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ij.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tg.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nw.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ky.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ab.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ti.jianghongdianzi.cn

[N05] 最大公约数
来源：http://of.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://jd.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wh.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gh.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eu.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mc.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qp.huanxung.cn

Ruby: a.gcd(b)
来源：http://yx.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vg.haigaiapp.cn

[N06] 判断回文字符串
来源：http://wc.shtwfgs.cn

Py:   s == s[::-1]
来源：http://vc.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://qp.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://ag.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://uk.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iu.hahajie.cn

Go:   // 双指针从两端比较
来源：http://je.colortex.cn

Ruby: s == s.reverse
来源：http://ot.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sn.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://xe.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ih.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kd.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bn.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://hr.nicolike.cn

Java: // 手写 HashMap
来源：http://ll.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://nw.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://gs.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wl.huixiangedu.cn

[N08] 生成全排列
来源：http://eu.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://ay.lnxyls.cn

PHP:  // 手写递归交换
来源：http://ji.huanxung.cn

JS:   // 手写回溯递归
来源：http://bf.shxzukj.cn

TS:   // 手写回溯递归
来源：http://qz.shtwfgs.cn

Java: // 手写回溯递归
来源：http://qr.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://zr.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://jy.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://qy.yuexingan06.cn

[N09] 栈与队列
来源：http://pk.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://va.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dk.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ad.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://io.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ct.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mk.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://og.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dx.bookmarksfly.cn

[N10] 链表节点定义
来源：http://xx.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pq.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kb.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mi.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gf.colortex.cn

Java: class Node { int v; Node next; }
来源：http://vo.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ja.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eo.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nw.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://tf.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ji.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://wk.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nj.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ws.jctech888.com.cn

Java: // 手写递归
来源：http://sx.nicolike.cn

Go:   // 手写递归
来源：http://xq.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nv.jctech888.com.cn

C#:   // 手写递归
来源：http://va.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ce.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ex.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vi.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nd.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pv.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oy.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qf.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eu.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://us.shxzukj.cn

================================================================================
来源：http://ot.jianghongdianzi.cn

O. 并发与异步
来源：http://jv.hahajie.cn

================================================================================
来源：http://io.asd995.cn

[O01] 启动一个线程
来源：http://yf.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sk.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ej.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qz.hnjuh.cn

TS:   // 同 JS
来源：http://ow.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://yq.haigaiapp.cn

Go:   go f()
来源：http://qr.lnxyls.cn

Ruby: Thread.new { f }
来源：http://qd.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://tc.wgjwhj.cn

[O02] 使用线程池
来源：http://fz.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qg.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://de.nicolike.cn

JS:   // worker_threads 线程池
来源：http://vc.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://zu.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ev.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wi.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oe.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eu.521024.cn

[O03] 加锁保护共享数据
来源：http://iq.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://qg.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://hl.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ss.bjjhwx.cn

TS:   // 同 JS
来源：http://ta.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://tm.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://od.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://al.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://ac.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://nz.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://pj.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wu.asd995.cn

JS:   async function f() { await g(); }
来源：http://zl.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lf.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://me.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lr.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nk.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://iv.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://bz.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://bp.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://le.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://ab.asd995.cn

TS:   await Promise.all(tasks)
来源：http://oe.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xk.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xt.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://ki.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qn.lnxyls.cn

[O06] 使用进程池
来源：http://pk.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ls.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://az.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://yy.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://ox.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zm.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hr.asd995.cn

Ruby: // fork 块
来源：http://qe.yuntaijiaju.cn

C#:   Parallel.For
来源：http://kk.bookmarksfly.cn

================================================================================
来源：http://ah.lnxyls.cn

P. 常用工具函数
来源：http://cn.huixinmuqiang.cn

================================================================================
来源：http://ky.huixiangedu.cn

[P01] 生成 UUID
来源：http://ll.521024.cn

Py:   str(uuid.uuid4())
来源：http://dx.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ud.colortex.cn

JS:   crypto.randomUUID()
来源：http://xq.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://ui.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://xz.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://jq.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://fv.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://ak.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://df.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bb.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yb.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qu.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://px.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uq.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lr.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rb.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kg.hahajie.cn

[P03] 生成短随机字符串
来源：http://xv.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jh.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lq.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ui.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ro.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ze.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hq.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rw.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chemitech.net.cn

[P04] 求长度
来源：http://jt.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ht.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uz.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lx.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yg.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://tr.9csxet.cn

Go:   len(arr);  len(m)
来源：http://ty.lnxyls.cn

Ruby: x.length;  x.size
来源：http://ee.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xi.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://qr.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://do.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://un.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://se.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fk.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wo.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pe.shxzskj.cn

Ruby: a == b
来源：http://an.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xp.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kf.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mi.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://bx.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ek.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://is.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tn.colortex.cn

Go:   if x == nil {}
来源：http://fv.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sf.hnjuh.cn

C#:   if (x is null) {}
来源：http://co.szxytkj.cn

[P07] 防抖与节流
来源：http://nr.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vf.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://ty.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ww.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yp.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uh.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hj.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://og.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://in.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://gh.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ed.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://am.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vt.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kl.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jn.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ov.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wy.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gk.9csxet.cn

================================================================================
来源：http://ue.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tm.gzmigu.cn

================================================================================
来源：http://nh.shtwfgs.cn

[Q01] 创建表
来源：http://uy.panjiajie.cn

CREATE TABLE users (
来源：http://zd.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ph.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://bw.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://qv.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mn.wgjwhj.cn

);
来源：http://vn.newstarts.cn

[Q02] 创建带外键的表
来源：http://eq.nicolike.cn

CREATE TABLE orders (
来源：http://qr.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uq.nszjky.cn

user_id INT NOT NULL,
来源：http://ir.huanxung.cn

amount DECIMAL(10, 2),
来源：http://ja.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gf.asd995.cn

);
来源：http://hw.huanxung.cn

[Q03] 增加列
来源：http://mh.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fu.yuexingan06.cn

[Q04] 修改列类型
来源：http://zt.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bp.yuntaijiaju.cn

[Q05] 重命名列
来源：http://lf.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bu.jctech888.com.cn

[Q06] 删除列
来源：http://bz.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jv.nicolike.cn

[Q07] 删除表
来源：http://ca.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://ky.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://xx.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ob.9csxet.cn

[Q09] 创建唯一索引
来源：http://kg.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gd.huanxung.cn

[Q10] 插入单行
来源：http://by.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://am.muxihuayi.cn

[Q11] 一次插入多行
来源：http://pr.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://td.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://on.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cl.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hg.szxytkj.cn

[Q13] 忽略重复插入
来源：http://fl.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ce.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://hk.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sh.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ap.jianghongdianzi.cn

[Q15] 查询全部
来源：http://jd.newstarts.cn

SELECT * FROM users;
来源：http://lk.nicolike.cn

[Q16] 查询指定列
来源：http://ky.9csxet.cn

SELECT id, name FROM users;
来源：http://pm.huixinmuqiang.cn

[Q17] 条件查询
来源：http://uv.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aq.wgjwhj.cn

[Q18] 模糊匹配
来源：http://ko.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qk.szxytkj.cn

[Q19] 范围查询
来源：http://no.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uq.hahajie.cn

[Q20] IN 列表
来源：http://dn.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://je.gzmigu.cn

[Q21] 空值判断
来源：http://wa.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tl.huanxung.cn

[Q22] 排序
来源：http://ux.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ou.huanxung.cn

[Q23] 分页
来源：http://sb.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rz.9csxet.cn

[Q24] 去重
来源：http://po.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://yn.newstarts.cn

[Q25] 只取前 N 条
来源：http://xw.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zc.yuntaijiaju.cn

[Q26] 计数
来源：http://kq.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://gk.hnjuh.cn

[Q27] 条件计数
来源：http://qt.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ol.haigaiapp.cn

[Q28] 求和与平均
来源：http://ln.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nk.huixiangedu.cn

[Q29] 最大最小值
来源：http://tj.hahajie.cn


<!-- 参考信息 -->