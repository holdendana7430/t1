代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://qc.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ar.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ac.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vb.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://na.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zq.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://of.yuexingan06.cn

[N04] 斐波那契数列
来源：http://vg.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jl.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rz.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jn.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nm.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lb.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jy.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://up.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zf.jctech888.com.cn

[N05] 最大公约数
来源：http://qh.nicolike.cn

Py:   math.gcd(a, b)
来源：http://nm.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gy.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://up.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mu.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zv.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ee.szsharing.cn

Ruby: a.gcd(b)
来源：http://ep.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://il.newstarts.cn

[N06] 判断回文字符串
来源：http://af.szsharing.cn

Py:   s == s[::-1]
来源：http://ol.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://wv.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://wl.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://eq.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sj.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ds.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://us.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ci.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://kw.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rf.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sa.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bp.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://hv.nszjky.cn

Java: // 手写 HashMap
来源：http://go.hahajie.cn

Go:   // 手写 map[int]int
来源：http://hr.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://oc.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qz.asd995.cn

[N08] 生成全排列
来源：http://ep.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://pf.hnjuh.cn

PHP:  // 手写递归交换
来源：http://uo.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://wj.newstarts.cn

TS:   // 手写回溯递归
来源：http://tm.521024.cn

Java: // 手写回溯递归
来源：http://sw.lnxyls.cn

Go:   // 手写回溯递归
来源：http://cj.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://bc.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://da.lnxyls.cn

[N09] 栈与队列
来源：http://pt.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kz.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://or.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rh.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://su.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ux.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hs.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ij.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nc.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://og.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qz.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://up.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ws.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lz.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://su.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ev.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://se.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xy.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://cx.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uo.newstarts.cn

PHP:  // 手写递归函数
来源：http://dg.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sx.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ox.jctech888.com.cn

Java: // 手写递归
来源：http://tv.gzmigu.cn

Go:   // 手写递归
来源：http://bq.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cn.shxzukj.cn

C#:   // 手写递归
来源：http://cl.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mg.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ng.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bv.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sj.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nk.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ul.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ei.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hx.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yy.gzmigu.cn

================================================================================
来源：http://vs.asd995.cn

O. 并发与异步
来源：http://ir.wgjwhj.cn

================================================================================
来源：http://fo.gzmigu.cn

[O01] 启动一个线程
来源：http://gh.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uz.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rk.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pt.hnjuh.cn

TS:   // 同 JS
来源：http://wy.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://fq.hahajie.cn

Go:   go f()
来源：http://yl.szxytkj.cn

Ruby: Thread.new { f }
来源：http://eu.nszjky.cn

C#:   Task.Run(() => F());
来源：http://po.huanxung.cn

[O02] 使用线程池
来源：http://bx.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qu.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mi.hahajie.cn

JS:   // worker_threads 线程池
来源：http://ma.nszjky.cn

TS:   // worker_threads 线程池
来源：http://nq.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xd.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wi.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rg.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cx.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://dg.szxytkj.cn

Py:   with lock: shared += 1
来源：http://ay.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://dx.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gy.szxytkj.cn

TS:   // 同 JS
来源：http://fl.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://ol.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qw.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wc.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://an.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://fl.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://oh.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ub.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://gh.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ka.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bu.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fs.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zt.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://bg.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://aw.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://dx.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ok.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://qx.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://it.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gx.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lr.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://bj.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lj.521024.cn

[O06] 使用进程池
来源：http://mt.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ee.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hr.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://jj.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://kv.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vv.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fl.panjiajie.cn

Ruby: // fork 块
来源：http://lc.521024.cn

C#:   Parallel.For
来源：http://md.huanxung.cn

================================================================================
来源：http://ho.nszjky.cn

P. 常用工具函数
来源：http://xz.huanxung.cn

================================================================================
来源：http://ds.nszjky.cn

[P01] 生成 UUID
来源：http://oz.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://gy.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pd.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://lc.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://zd.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://er.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://js.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://ol.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://po.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://bz.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bf.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ub.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vm.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pw.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mw.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://up.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rc.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nl.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://jq.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ic.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ys.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zl.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hl.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xd.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hp.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pn.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://et.nszjky.cn

[P04] 求长度
来源：http://ci.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mg.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jr.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rc.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qn.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://yz.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://uh.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://kc.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jb.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://bc.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ey.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sf.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vt.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bo.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mj.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ks.shxzukj.cn

Ruby: a == b
来源：http://ks.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jd.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xt.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lf.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://ih.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aj.bjjhwx.cn

TS:   if (x == null) {}
来源：http://pg.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://br.yuexingan06.cn

Go:   if x == nil {}
来源：http://jg.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ba.bjjhwx.cn

C#:   if (x is null) {}
来源：http://ud.yuexingan06.cn

[P07] 防抖与节流
来源：http://zf.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pk.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://mc.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ir.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pu.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lc.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xn.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://va.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wc.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://gx.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://st.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sa.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hf.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ac.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dz.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ey.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vu.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aa.huixiangedu.cn

================================================================================
来源：http://uq.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ik.gzmigu.cn

================================================================================
来源：http://gk.bookmarksfly.cn

[Q01] 创建表
来源：http://ee.huanxung.cn

CREATE TABLE users (
来源：http://am.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://db.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://zl.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://jp.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rm.nszjky.cn

);
来源：http://wh.lnxyls.cn

[Q02] 创建带外键的表
来源：http://uc.521024.cn

CREATE TABLE orders (
来源：http://cv.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ba.haigaiapp.cn

user_id INT NOT NULL,
来源：http://vu.nszjky.cn

amount DECIMAL(10, 2),
来源：http://ay.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wy.bjjhwx.cn

);
来源：http://rd.hahajie.cn

[Q03] 增加列
来源：http://ig.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fr.huanxung.cn

[Q04] 修改列类型
来源：http://iv.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rd.9csxet.cn

[Q05] 重命名列
来源：http://od.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fc.huanxung.cn

[Q06] 删除列
来源：http://cs.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ac.jianghongdianzi.cn

[Q07] 删除表
来源：http://zh.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://kd.wgjwhj.cn

[Q08] 创建普通索引
来源：http://ct.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aw.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://bl.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gy.chemitech.net.cn

[Q10] 插入单行
来源：http://qw.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ek.asd995.cn

[Q11] 一次插入多行
来源：http://mi.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wb.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://zv.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sf.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zq.shxzskj.cn

[Q13] 忽略重复插入
来源：http://uv.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aj.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://mr.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vu.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://no.colortex.cn

[Q15] 查询全部
来源：http://ss.521024.cn

SELECT * FROM users;
来源：http://sr.shxzskj.cn

[Q16] 查询指定列
来源：http://xi.szxytkj.cn

SELECT id, name FROM users;
来源：http://ez.shxzukj.cn

[Q17] 条件查询
来源：http://fg.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rq.newstarts.cn

[Q18] 模糊匹配
来源：http://wa.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oe.haigaiapp.cn

[Q19] 范围查询
来源：http://pu.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ef.haigaiapp.cn

[Q20] IN 列表
来源：http://ol.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://od.haigaiapp.cn

[Q21] 空值判断
来源：http://fa.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lo.9csxet.cn

[Q22] 排序
来源：http://bm.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lr.gzmigu.cn

[Q23] 分页
来源：http://pr.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pf.panjiajie.cn

[Q24] 去重
来源：http://kq.521024.cn

SELECT DISTINCT city FROM users;
来源：http://kv.hahajie.cn

[Q25] 只取前 N 条
来源：http://ul.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://im.shxzskj.cn

[Q26] 计数
来源：http://db.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://gd.haigaiapp.cn

[Q27] 条件计数
来源：http://of.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zu.hahajie.cn

[Q28] 求和与平均
来源：http://bc.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iq.newstarts.cn

[Q29] 最大最小值
来源：http://iy.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fd.haigaiapp.cn

[Q30] 分组统计
来源：http://zm.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://na.shtwfgs.cn

[Q31] 分组后过滤
来源：http://ts.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ci.nicolike.cn

[Q32] 分组拼接字符串
来源：http://xy.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ww.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dm.yuexingan06.cn


<!-- 参考信息 -->