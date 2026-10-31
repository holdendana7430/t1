代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://bo.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gn.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aa.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://np.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cj.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tv.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vp.521024.cn

[N04] 斐波那契数列
来源：http://ni.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vn.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zw.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cf.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ot.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iu.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vc.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://do.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tz.asd995.cn

[N05] 最大公约数
来源：http://rt.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://na.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qf.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ab.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rn.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fi.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gd.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://rf.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sx.panjiajie.cn

[N06] 判断回文字符串
来源：http://ff.newstarts.cn

Py:   s == s[::-1]
来源：http://qk.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://vw.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://vj.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://yv.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wl.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://bw.huanxung.cn

Ruby: s == s.reverse
来源：http://xj.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jz.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://mo.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qm.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dz.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ys.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://il.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://ux.asd995.cn

Go:   // 手写 map[int]int
来源：http://hf.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ms.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zn.hahajie.cn

[N08] 生成全排列
来源：http://ab.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://su.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://hw.szsharing.cn

JS:   // 手写回溯递归
来源：http://ct.9csxet.cn

TS:   // 手写回溯递归
来源：http://fi.huanxung.cn

Java: // 手写回溯递归
来源：http://aj.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://rw.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://br.9csxet.cn

C#:   // 手写回溯递归
来源：http://is.shtwfgs.cn

[N09] 栈与队列
来源：http://dx.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fp.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jw.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://de.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wl.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ae.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ad.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xk.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.szxytkj.cn

[N10] 链表节点定义
来源：http://ya.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cv.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jc.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gb.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hr.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://pn.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rq.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gw.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fz.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://fu.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dq.newstarts.cn

PHP:  // 手写递归函数
来源：http://ta.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://as.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gz.nicolike.cn

Java: // 手写递归
来源：http://je.shtwfgs.cn

Go:   // 手写递归
来源：http://yc.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dv.szsharing.cn

C#:   // 手写递归
来源：http://xb.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bn.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gb.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fz.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eh.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rm.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fj.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lv.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://co.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fz.asd995.cn

================================================================================
来源：http://ps.jctech888.com.cn

O. 并发与异步
来源：http://zk.colortex.cn

================================================================================
来源：http://lc.huanxung.cn

[O01] 启动一个线程
来源：http://zy.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ie.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://da.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yv.huanxung.cn

TS:   // 同 JS
来源：http://xe.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://kl.szxytkj.cn

Go:   go f()
来源：http://pa.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://ei.9csxet.cn

C#:   Task.Run(() => F());
来源：http://bn.newstarts.cn

[O02] 使用线程池
来源：http://iu.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zt.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pr.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://go.asd995.cn

TS:   // worker_threads 线程池
来源：http://oj.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fj.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kw.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://de.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xl.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://mi.nicolike.cn

Py:   with lock: shared += 1
来源：http://hw.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://nk.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rx.yuexingan06.cn

TS:   // 同 JS
来源：http://su.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://ui.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jb.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jp.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://si.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://xq.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://rb.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sj.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://ey.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bn.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://op.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bl.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fb.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://is.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://bs.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://yy.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://je.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://pg.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://xl.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oe.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zz.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://nq.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hx.asd995.cn

[O06] 使用进程池
来源：http://lr.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qq.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lq.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://hv.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://hg.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ct.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qi.lnxyls.cn

Ruby: // fork 块
来源：http://we.huixinmuqiang.cn

C#:   Parallel.For
来源：http://bk.szxytkj.cn

================================================================================
来源：http://qa.shxzskj.cn

P. 常用工具函数
来源：http://vl.jctech888.com.cn

================================================================================
来源：http://qx.newstarts.cn

[P01] 生成 UUID
来源：http://yf.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://hd.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zc.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://er.colortex.cn

TS:   crypto.randomUUID()
来源：http://fr.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://qg.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://uy.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://jo.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://dq.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://np.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://es.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oi.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yk.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hu.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bs.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rz.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hr.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dy.lnxyls.cn

[P03] 生成短随机字符串
来源：http://zk.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://su.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nn.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uu.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eq.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qn.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bg.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nd.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jv.shxzukj.cn

[P04] 求长度
来源：http://ph.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ie.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://md.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rl.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fh.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://qz.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ur.panjiajie.cn

Ruby: x.length;  x.size
来源：http://xw.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dp.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://hd.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ru.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fl.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uy.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xc.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kz.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://km.jctech888.com.cn

Ruby: a == b
来源：http://ay.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ua.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vt.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lw.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://ls.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fu.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://re.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nm.huixiangedu.cn

Go:   if x == nil {}
来源：http://sv.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pw.szxytkj.cn

C#:   if (x is null) {}
来源：http://hz.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://ww.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qm.colortex.cn

PHP:  // 手写时间戳比较
来源：http://oq.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fy.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ro.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vo.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vl.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hd.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ji.asd995.cn

[P08] 处理浮点精度问题
来源：http://zi.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oh.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uo.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ej.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://td.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nk.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vr.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fn.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://af.wgjwhj.cn

================================================================================
来源：http://eo.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ei.muxihuayi.cn

================================================================================
来源：http://vg.521024.cn

[Q01] 创建表
来源：http://cr.wgjwhj.cn

CREATE TABLE users (
来源：http://tb.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://il.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://vb.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://ho.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://se.panjiajie.cn

);
来源：http://hu.asd995.cn

[Q02] 创建带外键的表
来源：http://jp.panjiajie.cn

CREATE TABLE orders (
来源：http://yh.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wx.huanxung.cn

user_id INT NOT NULL,
来源：http://ub.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://wk.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ui.wgjwhj.cn

);
来源：http://ju.szxytkj.cn

[Q03] 增加列
来源：http://sl.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wb.nicolike.cn

[Q04] 修改列类型
来源：http://wi.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nv.haigaiapp.cn

[Q05] 重命名列
来源：http://ag.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ih.jianghongdianzi.cn

[Q06] 删除列
来源：http://zv.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yr.bookmarksfly.cn

[Q07] 删除表
来源：http://gj.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://qo.yuexingan06.cn

[Q08] 创建普通索引
来源：http://dm.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ks.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://zs.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vs.shxzskj.cn

[Q10] 插入单行
来源：http://au.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cl.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://ut.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tl.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://od.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lw.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://km.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://jw.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lh.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://gu.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lv.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vg.shxzukj.cn

[Q15] 查询全部
来源：http://zm.panjiajie.cn

SELECT * FROM users;
来源：http://mg.newstarts.cn

[Q16] 查询指定列
来源：http://iu.shxzukj.cn

SELECT id, name FROM users;
来源：http://ku.haigaiapp.cn

[Q17] 条件查询
来源：http://qu.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jj.hnjuh.cn

[Q18] 模糊匹配
来源：http://tf.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jx.shxzskj.cn

[Q19] 范围查询
来源：http://tm.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nc.9csxet.cn

[Q20] IN 列表
来源：http://yu.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sm.hnjuh.cn

[Q21] 空值判断
来源：http://px.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bf.jctech888.com.cn

[Q22] 排序
来源：http://xp.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rr.panjiajie.cn

[Q23] 分页
来源：http://or.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xa.yuntaijiaju.cn

[Q24] 去重
来源：http://kj.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://pb.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://on.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cg.jctech888.com.cn

[Q26] 计数
来源：http://uz.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://ug.chemitech.net.cn

[Q27] 条件计数
来源：http://ie.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dn.9csxet.cn

[Q28] 求和与平均
来源：http://qt.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gq.szsharing.cn

[Q29] 最大最小值
来源：http://gh.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oh.szsharing.cn

[Q30] 分组统计
来源：http://jc.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://af.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://me.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yk.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://us.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uw.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gz.shxzukj.cn


<!-- 参考信息 -->