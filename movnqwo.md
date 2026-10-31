代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://of.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://be.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jj.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tk.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iv.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://by.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xq.lnxyls.cn

[N04] 斐波那契数列
来源：http://mp.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://td.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sl.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uh.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://on.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oi.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yw.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pu.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sv.asd995.cn

[N05] 最大公约数
来源：http://gu.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://bu.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zw.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://co.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jz.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ac.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ml.hnjuh.cn

Ruby: a.gcd(b)
来源：http://dr.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dl.gzmigu.cn

[N06] 判断回文字符串
来源：http://ti.bjjhwx.cn

Py:   s == s[::-1]
来源：http://mf.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://km.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ke.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ug.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qb.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://cr.jctech888.com.cn

Ruby: s == s.reverse
来源：http://dr.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qv.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://mx.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bq.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pd.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dc.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://be.lnxyls.cn

Java: // 手写 HashMap
来源：http://co.huanxung.cn

Go:   // 手写 map[int]int
来源：http://kj.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://pa.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pm.nszjky.cn

[N08] 生成全排列
来源：http://vn.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://ct.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ph.szxytkj.cn

JS:   // 手写回溯递归
来源：http://ed.9csxet.cn

TS:   // 手写回溯递归
来源：http://ll.lnxyls.cn

Java: // 手写回溯递归
来源：http://ux.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://lu.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://gs.lnxyls.cn

C#:   // 手写回溯递归
来源：http://pg.panjiajie.cn

[N09] 栈与队列
来源：http://kd.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tq.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wb.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vf.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gd.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sc.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lb.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pt.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pc.bookmarksfly.cn

[N10] 链表节点定义
来源：http://mj.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ng.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vj.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cf.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fr.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://mt.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://te.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cd.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ml.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://or.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://um.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://rs.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oe.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ii.wgjwhj.cn

Java: // 手写递归
来源：http://bf.lnxyls.cn

Go:   // 手写递归
来源：http://tl.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://er.asd995.cn

C#:   // 手写递归
来源：http://mf.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ii.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bp.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bh.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cq.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ie.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://do.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hw.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vm.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sz.asd995.cn

================================================================================
来源：http://gb.yuntaijiaju.cn

O. 并发与异步
来源：http://qf.jctech888.com.cn

================================================================================
来源：http://sk.9csxet.cn

[O01] 启动一个线程
来源：http://ux.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://df.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oe.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uo.shtwfgs.cn

TS:   // 同 JS
来源：http://nx.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://vd.yuexingan06.cn

Go:   go f()
来源：http://ab.521024.cn

Ruby: Thread.new { f }
来源：http://ov.asd995.cn

C#:   Task.Run(() => F());
来源：http://qk.szxytkj.cn

[O02] 使用线程池
来源：http://oi.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qd.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ze.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://ai.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://st.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kb.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kq.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bd.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kc.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://ha.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://jt.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://wt.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hp.yuexingan06.cn

TS:   // 同 JS
来源：http://el.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://wl.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dh.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xj.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://hh.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://xz.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://ti.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lk.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://ak.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hq.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://go.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nm.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://he.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://qd.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://wf.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://pw.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ch.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://dj.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://cy.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xg.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jt.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://uf.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ml.nszjky.cn

[O06] 使用进程池
来源：http://gr.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hf.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qb.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://wt.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://hk.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qr.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uu.nszjky.cn

Ruby: // fork 块
来源：http://xb.panjiajie.cn

C#:   Parallel.For
来源：http://sq.nszjky.cn

================================================================================
来源：http://ot.9csxet.cn

P. 常用工具函数
来源：http://kc.lnxyls.cn

================================================================================
来源：http://ja.shxzskj.cn

[P01] 生成 UUID
来源：http://vb.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://wk.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uv.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://jz.nszjky.cn

TS:   crypto.randomUUID()
来源：http://mn.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://gd.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://ho.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://si.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://qy.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://oy.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ru.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jm.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://by.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cr.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dd.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fy.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bd.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qo.lnxyls.cn

[P03] 生成短随机字符串
来源：http://ou.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tz.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bl.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mi.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dq.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eh.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vp.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ww.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ir.huixinmuqiang.cn

[P04] 求长度
来源：http://iz.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ca.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pd.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lq.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://he.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://zd.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://ut.521024.cn

Ruby: x.length;  x.size
来源：http://rx.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hl.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://tx.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uy.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tw.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zi.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mf.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zd.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zc.huixinmuqiang.cn

Ruby: a == b
来源：http://gr.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gm.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sd.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tf.colortex.cn

PHP:  if (empty($x)) {}
来源：http://qw.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qg.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://xq.muxihuayi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://en.huanxung.cn

Go:   if x == nil {}
来源：http://uh.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bx.jctech888.com.cn

C#:   if (x is null) {}
来源：http://un.asd995.cn

[P07] 防抖与节流
来源：http://rj.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://be.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://uo.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bp.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gw.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bv.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wk.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bq.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ny.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://bb.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ub.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kb.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ey.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://db.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mb.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xa.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xc.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pa.huanxung.cn

================================================================================
来源：http://qe.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jt.newstarts.cn

================================================================================
来源：http://hf.huixinmuqiang.cn

[Q01] 创建表
来源：http://fq.szsharing.cn

CREATE TABLE users (
来源：http://ux.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ty.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://wj.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://lb.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xo.hahajie.cn

);
来源：http://sw.shxzukj.cn

[Q02] 创建带外键的表
来源：http://va.nszjky.cn

CREATE TABLE orders (
来源：http://fh.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vp.huixiangedu.cn

user_id INT NOT NULL,
来源：http://fd.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://fj.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fu.hahajie.cn

);
来源：http://dp.jctech888.com.cn

[Q03] 增加列
来源：http://qf.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wc.9csxet.cn

[Q04] 修改列类型
来源：http://iv.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hv.huanxung.cn

[Q05] 重命名列
来源：http://pz.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lv.gzmigu.cn

[Q06] 删除列
来源：http://nz.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dy.asd995.cn

[Q07] 删除表
来源：http://xp.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://kt.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://uo.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bp.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://pr.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vf.huixiangedu.cn

[Q10] 插入单行
来源：http://zy.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ek.9csxet.cn

[Q11] 一次插入多行
来源：http://bq.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sy.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://th.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yg.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xu.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://sw.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jd.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://lh.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zo.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://er.hnjuh.cn

[Q15] 查询全部
来源：http://az.521024.cn

SELECT * FROM users;
来源：http://vn.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://ax.wgjwhj.cn

SELECT id, name FROM users;
来源：http://jc.yuntaijiaju.cn

[Q17] 条件查询
来源：http://yx.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iw.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://ff.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hm.colortex.cn

[Q19] 范围查询
来源：http://mr.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://da.hahajie.cn

[Q20] IN 列表
来源：http://uy.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jn.bookmarksfly.cn

[Q21] 空值判断
来源：http://ly.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://os.haigaiapp.cn

[Q22] 排序
来源：http://gc.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fj.yuexingan06.cn

[Q23] 分页
来源：http://nq.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tg.jianghongdianzi.cn

[Q24] 去重
来源：http://mh.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://kx.nicolike.cn

[Q25] 只取前 N 条
来源：http://cv.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sj.wgjwhj.cn

[Q26] 计数
来源：http://xa.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://lz.newstarts.cn

[Q27] 条件计数
来源：http://vz.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yy.521024.cn

[Q28] 求和与平均
来源：http://rs.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vv.9csxet.cn

[Q29] 最大最小值
来源：http://cx.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bj.shtwfgs.cn

[Q30] 分组统计
来源：http://ix.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zu.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://vk.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ci.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://cu.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mx.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ek.muxihuayi.cn


<!-- 参考信息 -->