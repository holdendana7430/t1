代发 wailian999

Ruby: arr.sort
来源：http://zp.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bc.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://kp.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nr.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://nb.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yp.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fl.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vy.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://om.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sv.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ge.wgjwhj.cn

[N04] 斐波那契数列
来源：http://se.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uv.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ne.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xt.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zb.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mh.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gx.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gz.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gb.shtwfgs.cn

[N05] 最大公约数
来源：http://mq.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://zj.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hx.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ty.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pa.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jh.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ir.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://wj.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cn.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://gx.huanxung.cn

Py:   s == s[::-1]
来源：http://ya.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://ks.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://ae.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://rj.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sc.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://hu.gzmigu.cn

Ruby: s == s.reverse
来源：http://cd.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qk.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://fc.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zg.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fx.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ou.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://xu.shtwfgs.cn

Java: // 手写 HashMap
来源：http://wm.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://tl.newstarts.cn

Ruby: // 手写 Hash
来源：http://an.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ut.chemitech.net.cn

[N08] 生成全排列
来源：http://ju.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ht.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://il.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://zd.nszjky.cn

TS:   // 手写回溯递归
来源：http://gh.hnjuh.cn

Java: // 手写回溯递归
来源：http://mh.shxzskj.cn

Go:   // 手写回溯递归
来源：http://zl.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://kz.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://zp.huanxung.cn

[N09] 栈与队列
来源：http://kz.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kx.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ri.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lq.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wl.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sn.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jz.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://go.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zj.yuexingan06.cn

[N10] 链表节点定义
来源：http://xi.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iz.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jw.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eb.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eh.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://th.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fr.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jc.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ql.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://cu.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rs.nicolike.cn

PHP:  // 手写递归函数
来源：http://dw.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mb.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xz.bjjhwx.cn

Java: // 手写递归
来源：http://kg.jctech888.com.cn

Go:   // 手写递归
来源：http://uy.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://un.shtwfgs.cn

C#:   // 手写递归
来源：http://vp.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yx.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zr.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qb.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://no.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kp.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ze.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xi.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zb.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dk.huanxung.cn

================================================================================
来源：http://er.muxihuayi.cn

O. 并发与异步
来源：http://zu.huanxung.cn

================================================================================
来源：http://ub.huanxung.cn

[O01] 启动一个线程
来源：http://pg.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mq.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ta.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://or.shxzskj.cn

TS:   // 同 JS
来源：http://kz.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://wo.haigaiapp.cn

Go:   go f()
来源：http://ku.shxzukj.cn

Ruby: Thread.new { f }
来源：http://oq.asd995.cn

C#:   Task.Run(() => F());
来源：http://nk.szsharing.cn

[O02] 使用线程池
来源：http://vc.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rq.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lo.521024.cn

JS:   // worker_threads 线程池
来源：http://mu.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://aj.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gd.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pt.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vn.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ao.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://hb.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://bp.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://rn.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bu.muxihuayi.cn

TS:   // 同 JS
来源：http://wm.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://lu.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vx.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wu.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://rs.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://ls.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://np.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ej.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://ze.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kt.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ed.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tn.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lt.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://oj.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://bx.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://ox.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uh.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://kz.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://sg.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jc.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ih.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://pn.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iz.huanxung.cn

[O06] 使用进程池
来源：http://kd.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bq.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yt.asd995.cn

JS:   // child_process / cluster 模块
来源：http://sq.colortex.cn

TS:   // child_process / cluster 模块
来源：http://as.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wz.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qb.shxzskj.cn

Ruby: // fork 块
来源：http://mj.haigaiapp.cn

C#:   Parallel.For
来源：http://kw.hahajie.cn

================================================================================
来源：http://mb.nicolike.cn

P. 常用工具函数
来源：http://zw.521024.cn

================================================================================
来源：http://db.9csxet.cn

[P01] 生成 UUID
来源：http://de.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://xd.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xn.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://qf.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://bw.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://qg.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://ex.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://kc.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://yz.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://wp.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rv.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bx.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ut.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wq.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://li.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cb.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qd.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tx.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://zc.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xc.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ij.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vd.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cu.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bg.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gp.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lb.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://de.asd995.cn

[P04] 求长度
来源：http://em.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://du.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zm.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xw.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fv.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://fd.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://ah.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://pn.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ks.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://tq.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ra.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jb.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jg.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sp.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tq.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bo.haigaiapp.cn

Ruby: a == b
来源：http://li.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ax.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jy.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wg.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://xi.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ht.521024.cn

TS:   if (x == null) {}
来源：http://ww.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vp.asd995.cn

Go:   if x == nil {}
来源：http://iy.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pz.wgjwhj.cn

C#:   if (x is null) {}
来源：http://ep.muxihuayi.cn

[P07] 防抖与节流
来源：http://do.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xd.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://dn.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://au.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ij.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tx.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xd.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ib.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ed.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://kd.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nk.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dx.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nh.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://az.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ka.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qz.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wt.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vu.chemitech.net.cn

================================================================================
来源：http://rb.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://id.panjiajie.cn

================================================================================
来源：http://ap.gzmigu.cn

[Q01] 创建表
来源：http://cn.jianghongdianzi.cn

CREATE TABLE users (
来源：http://eu.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xq.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://dp.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://ar.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ky.szxytkj.cn

);
来源：http://jz.panjiajie.cn

[Q02] 创建带外键的表
来源：http://mt.nszjky.cn

CREATE TABLE orders (
来源：http://nx.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wy.jctech888.com.cn

user_id INT NOT NULL,
来源：http://bq.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://et.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jv.szxytkj.cn

);
来源：http://uf.colortex.cn

[Q03] 增加列
来源：http://vn.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hy.huanxung.cn

[Q04] 修改列类型
来源：http://uf.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gg.hnjuh.cn

[Q05] 重命名列
来源：http://pb.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rt.chemitech.net.cn

[Q06] 删除列
来源：http://ae.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pp.jctech888.com.cn

[Q07] 删除表
来源：http://le.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://id.muxihuayi.cn

[Q08] 创建普通索引
来源：http://td.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tm.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://pd.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://or.wgjwhj.cn

[Q10] 插入单行
来源：http://ui.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mj.shtwfgs.cn

[Q11] 一次插入多行
来源：http://wa.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iq.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://gt.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pd.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cg.shxzskj.cn

[Q13] 忽略重复插入
来源：http://uq.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xr.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://ni.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rk.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ku.jctech888.com.cn

[Q15] 查询全部
来源：http://nu.asd995.cn

SELECT * FROM users;
来源：http://jv.9csxet.cn

[Q16] 查询指定列
来源：http://zj.haigaiapp.cn

SELECT id, name FROM users;
来源：http://iy.shxzskj.cn

[Q17] 条件查询
来源：http://zl.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ue.wgjwhj.cn

[Q18] 模糊匹配
来源：http://ar.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uu.huixinmuqiang.cn

[Q19] 范围查询
来源：http://vt.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mt.bjjhwx.cn

[Q20] IN 列表
来源：http://qc.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cd.shxzskj.cn

[Q21] 空值判断
来源：http://fk.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ln.hahajie.cn

[Q22] 排序
来源：http://qb.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yq.yuntaijiaju.cn

[Q23] 分页
来源：http://qc.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jn.nicolike.cn

[Q24] 去重
来源：http://kx.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://vl.521024.cn

[Q25] 只取前 N 条
来源：http://ao.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oi.huixinmuqiang.cn

[Q26] 计数
来源：http://oj.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://on.newstarts.cn

[Q27] 条件计数
来源：http://oi.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qz.wgjwhj.cn

[Q28] 求和与平均
来源：http://zh.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fo.hahajie.cn

[Q29] 最大最小值
来源：http://gz.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mu.nicolike.cn

[Q30] 分组统计
来源：http://nm.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xp.shxzskj.cn

[Q31] 分组后过滤
来源：http://dw.huixiangedu.cn


<!-- 参考信息 -->