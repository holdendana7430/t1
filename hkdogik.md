代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zs.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ha.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xb.lnxyls.cn

[N04] 斐波那契数列
来源：http://xh.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hj.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kt.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jj.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tb.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dv.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qb.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yp.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lz.panjiajie.cn

[N05] 最大公约数
来源：http://mo.asd995.cn

Py:   math.gcd(a, b)
来源：http://sc.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://la.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qi.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pg.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ti.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vy.shxzukj.cn

Ruby: a.gcd(b)
来源：http://nw.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gm.shxzukj.cn

[N06] 判断回文字符串
来源：http://bv.szxytkj.cn

Py:   s == s[::-1]
来源：http://kv.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://bo.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://qr.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://en.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hv.hahajie.cn

Go:   // 双指针从两端比较
来源：http://gt.szsharing.cn

Ruby: s == s.reverse
来源：http://fa.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gi.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://sw.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cg.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mb.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zm.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://bk.huanxung.cn

Java: // 手写 HashMap
来源：http://we.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://wa.lnxyls.cn

Ruby: // 手写 Hash
来源：http://zc.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ee.lnxyls.cn

[N08] 生成全排列
来源：http://aa.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://eu.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://wp.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://mx.newstarts.cn

TS:   // 手写回溯递归
来源：http://uy.huixiangedu.cn

Java: // 手写回溯递归
来源：http://go.shxzukj.cn

Go:   // 手写回溯递归
来源：http://xj.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://oc.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://ce.521024.cn

[N09] 栈与队列
来源：http://sd.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iv.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yo.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qa.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lp.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dp.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jd.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ek.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hahajie.cn

[N10] 链表节点定义
来源：http://vo.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ez.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vd.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wn.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dr.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://cm.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dz.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://en.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ih.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://ci.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mh.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://of.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xo.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yh.yuexingan06.cn

Java: // 手写递归
来源：http://bm.szxytkj.cn

Go:   // 手写递归
来源：http://qz.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tz.newstarts.cn

C#:   // 手写递归
来源：http://ln.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://af.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mz.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sv.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gc.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qm.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gf.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xj.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://io.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://on.yuexingan06.cn

================================================================================
来源：http://bv.colortex.cn

O. 并发与异步
来源：http://or.hnjuh.cn

================================================================================
来源：http://hr.huanxung.cn

[O01] 启动一个线程
来源：http://ac.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ys.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ei.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ej.lnxyls.cn

TS:   // 同 JS
来源：http://vq.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://tr.shtwfgs.cn

Go:   go f()
来源：http://ls.huanxung.cn

Ruby: Thread.new { f }
来源：http://rn.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://zw.yuexingan06.cn

[O02] 使用线程池
来源：http://bh.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://le.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wr.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://et.nszjky.cn

TS:   // worker_threads 线程池
来源：http://cf.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jv.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yy.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xw.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ab.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://sy.newstarts.cn

Py:   with lock: shared += 1
来源：http://ym.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://se.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://je.bjjhwx.cn

TS:   // 同 JS
来源：http://dl.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://us.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kk.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bn.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://bj.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://ga.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://jy.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kq.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://ai.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fz.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hm.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qu.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fl.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://xv.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://am.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://oi.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ha.colortex.cn

JS:   await Promise.all(tasks)
来源：http://ed.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://ai.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cg.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rz.9csxet.cn

Ruby: threads.map(&:join)
来源：http://si.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rk.asd995.cn

[O06] 使用进程池
来源：http://cv.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vr.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lz.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://lm.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://wo.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sz.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dn.gzmigu.cn

Ruby: // fork 块
来源：http://kg.shxzukj.cn

C#:   Parallel.For
来源：http://tt.shtwfgs.cn

================================================================================
来源：http://qo.huanxung.cn

P. 常用工具函数
来源：http://sq.jctech888.com.cn

================================================================================
来源：http://il.shtwfgs.cn

[P01] 生成 UUID
来源：http://by.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://te.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ol.nicolike.cn

JS:   crypto.randomUUID()
来源：http://ep.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://sc.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://hu.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://xd.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://wy.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://rw.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://oh.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jl.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mt.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ag.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ih.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ks.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hh.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ng.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aj.szxytkj.cn

[P03] 生成短随机字符串
来源：http://jc.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tb.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dq.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hg.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mp.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zn.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zf.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mw.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ee.shxzskj.cn

[P04] 求长度
来源：http://yk.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sr.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jf.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ge.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oc.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://cp.colortex.cn

Go:   len(arr);  len(m)
来源：http://ds.9csxet.cn

Ruby: x.length;  x.size
来源：http://tl.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zl.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://yv.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ih.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://du.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bn.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sk.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ae.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zm.hahajie.cn

Ruby: a == b
来源：http://xh.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lu.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bv.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ny.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://ux.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://in.9csxet.cn

TS:   if (x == null) {}
来源：http://pv.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zu.nszjky.cn

Go:   if x == nil {}
来源：http://tp.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zq.521024.cn

C#:   if (x is null) {}
来源：http://cb.asd995.cn

[P07] 防抖与节流
来源：http://wq.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nc.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ms.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://er.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mx.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ly.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fr.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nj.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lq.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://bm.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mx.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://am.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gk.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ln.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uo.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ej.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xh.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ca.nszjky.cn

================================================================================
来源：http://oy.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fu.hahajie.cn

================================================================================
来源：http://dr.shtwfgs.cn

[Q01] 创建表
来源：http://hc.bookmarksfly.cn

CREATE TABLE users (
来源：http://nk.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lb.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://bu.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://go.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yg.521024.cn

);
来源：http://rr.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://gn.asd995.cn

CREATE TABLE orders (
来源：http://yo.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fe.huanxung.cn

user_id INT NOT NULL,
来源：http://vg.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://qt.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ry.szsharing.cn

);
来源：http://jt.huanxung.cn

[Q03] 增加列
来源：http://ca.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jl.huanxung.cn

[Q04] 修改列类型
来源：http://xd.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pf.shxzskj.cn

[Q05] 重命名列
来源：http://ib.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yg.muxihuayi.cn

[Q06] 删除列
来源：http://oc.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://za.huixinmuqiang.cn

[Q07] 删除表
来源：http://bj.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://ev.521024.cn

[Q08] 创建普通索引
来源：http://oc.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pk.nicolike.cn

[Q09] 创建唯一索引
来源：http://ip.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sr.haigaiapp.cn

[Q10] 插入单行
来源：http://km.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dh.chemitech.net.cn

[Q11] 一次插入多行
来源：http://cb.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ii.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://rp.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wf.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vp.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://qp.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ia.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://wx.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yx.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qz.chemitech.net.cn

[Q15] 查询全部
来源：http://cg.haigaiapp.cn

SELECT * FROM users;
来源：http://cu.shxzukj.cn

[Q16] 查询指定列
来源：http://bg.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://vf.newstarts.cn

[Q17] 条件查询
来源：http://xd.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ir.shtwfgs.cn

[Q18] 模糊匹配
来源：http://qv.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xn.colortex.cn

[Q19] 范围查询
来源：http://nu.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nw.lnxyls.cn

[Q20] IN 列表
来源：http://ea.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gh.hnjuh.cn

[Q21] 空值判断
来源：http://kt.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lc.yuntaijiaju.cn

[Q22] 排序
来源：http://qy.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fa.yuntaijiaju.cn

[Q23] 分页
来源：http://fn.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qb.lnxyls.cn

[Q24] 去重
来源：http://ew.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://mo.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://ta.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vf.yuntaijiaju.cn

[Q26] 计数
来源：http://nz.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://sz.shxzukj.cn

[Q27] 条件计数
来源：http://qu.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yj.nicolike.cn

[Q28] 求和与平均
来源：http://nm.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yi.shtwfgs.cn

[Q29] 最大最小值
来源：http://ha.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pu.bookmarksfly.cn

[Q30] 分组统计
来源：http://kw.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uo.muxihuayi.cn

[Q31] 分组后过滤
来源：http://hu.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tm.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://ld.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://am.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eb.521024.cn

[Q33] 多列分组
来源：http://cq.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shxzukj.cn

[Q34] 每组取第一条
来源：http://ig.bjjhwx.cn

SELECT * FROM (
来源：http://om.hahajie.cn


<!-- 参考信息 -->