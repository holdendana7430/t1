代发 wailian999

Ruby: arr.sort
来源：http://nx.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zq.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://ye.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bf.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://fv.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pf.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bo.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://me.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ql.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nr.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hz.haigaiapp.cn

[N04] 斐波那契数列
来源：http://fm.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rb.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ib.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fz.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://im.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dz.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rs.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rt.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bk.huanxung.cn

[N05] 最大公约数
来源：http://ct.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://jq.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mt.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mx.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nn.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yg.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dy.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://ui.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://my.shtwfgs.cn

[N06] 判断回文字符串
来源：http://im.huanxung.cn

Py:   s == s[::-1]
来源：http://bn.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://bv.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://sv.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://dc.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sk.nszjky.cn

Go:   // 双指针从两端比较
来源：http://cf.yuexingan06.cn

Ruby: s == s.reverse
来源：http://cw.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gx.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://gc.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hv.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tm.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eo.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://am.nszjky.cn

Java: // 手写 HashMap
来源：http://vx.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://la.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://sd.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jt.lnxyls.cn

[N08] 生成全排列
来源：http://eh.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://wt.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://sg.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ot.asd995.cn

TS:   // 手写回溯递归
来源：http://yi.newstarts.cn

Java: // 手写回溯递归
来源：http://gt.colortex.cn

Go:   // 手写回溯递归
来源：http://tg.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://ri.hnjuh.cn

C#:   // 手写回溯递归
来源：http://ck.chemitech.net.cn

[N09] 栈与队列
来源：http://py.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ks.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vb.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eh.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zf.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gf.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bc.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://io.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wf.jctech888.com.cn

[N10] 链表节点定义
来源：http://eo.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vy.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fw.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qh.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zq.colortex.cn

Java: class Node { int v; Node next; }
来源：http://pg.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://an.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eq.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uj.hahajie.cn

[N11] 二叉树中序遍历
来源：http://uz.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vd.nszjky.cn

PHP:  // 手写递归函数
来源：http://cm.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zi.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tn.hahajie.cn

Java: // 手写递归
来源：http://ai.newstarts.cn

Go:   // 手写递归
来源：http://bj.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fx.huanxung.cn

C#:   // 手写递归
来源：http://od.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mr.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://el.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ba.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mq.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tp.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wv.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bl.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hc.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sg.muxihuayi.cn

================================================================================
来源：http://ig.panjiajie.cn

O. 并发与异步
来源：http://nf.shtwfgs.cn

================================================================================
来源：http://gl.asd995.cn

[O01] 启动一个线程
来源：http://au.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yw.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dp.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kx.panjiajie.cn

TS:   // 同 JS
来源：http://sh.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://ik.huanxung.cn

Go:   go f()
来源：http://qj.521024.cn

Ruby: Thread.new { f }
来源：http://tt.nszjky.cn

C#:   Task.Run(() => F());
来源：http://tr.huixinmuqiang.cn

[O02] 使用线程池
来源：http://lt.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cx.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vh.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://pv.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://nj.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ui.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rg.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pr.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mz.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://mg.hahajie.cn

Py:   with lock: shared += 1
来源：http://ys.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://ql.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gj.shxzukj.cn

TS:   // 同 JS
来源：http://jr.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://pc.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oy.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://he.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://cf.521024.cn

[O04] 定义异步函数并等待
来源：http://lg.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://jw.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wd.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://us.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dw.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vx.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xr.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ek.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://ev.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://cc.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://vq.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://za.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://uq.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://ry.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://td.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mn.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://pt.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ac.muxihuayi.cn

[O06] 使用进程池
来源：http://td.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://et.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jj.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://uu.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://gg.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aa.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dx.szxytkj.cn

Ruby: // fork 块
来源：http://uh.hnjuh.cn

C#:   Parallel.For
来源：http://sa.szsharing.cn

================================================================================
来源：http://hb.jctech888.com.cn

P. 常用工具函数
来源：http://hd.bjjhwx.cn

================================================================================
来源：http://xb.jctech888.com.cn

[P01] 生成 UUID
来源：http://dx.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://fi.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wx.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://cf.colortex.cn

TS:   crypto.randomUUID()
来源：http://aw.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://rj.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://mx.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://ka.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://rd.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://uw.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bp.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tx.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rg.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vs.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bj.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lj.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gh.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vg.szxytkj.cn

[P03] 生成短随机字符串
来源：http://hm.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vw.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://so.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ja.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ss.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cs.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pa.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vl.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tv.bookmarksfly.cn

[P04] 求长度
来源：http://ei.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://it.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://we.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bs.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ra.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://xr.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://xq.gzmigu.cn

Ruby: x.length;  x.size
来源：http://yb.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sw.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://jc.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zo.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zb.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bd.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://px.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ik.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fl.shxzskj.cn

Ruby: a == b
来源：http://xo.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fq.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gw.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://no.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://dz.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oa.shxzskj.cn

TS:   if (x == null) {}
来源：http://la.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ug.szsharing.cn

Go:   if x == nil {}
来源：http://wd.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gq.shtwfgs.cn

C#:   if (x is null) {}
来源：http://ly.hnjuh.cn

[P07] 防抖与节流
来源：http://re.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gd.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://jp.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gv.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xm.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://am.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bc.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lk.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ci.colortex.cn

[P08] 处理浮点精度问题
来源：http://vy.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mf.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ma.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jz.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pr.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yu.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://og.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://da.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kq.jctech888.com.cn

================================================================================
来源：http://bg.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tf.newstarts.cn

================================================================================
来源：http://em.newstarts.cn

[Q01] 创建表
来源：http://vu.jctech888.com.cn

CREATE TABLE users (
来源：http://ab.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ht.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://zj.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://us.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tu.shxzukj.cn

);
来源：http://bd.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://aa.bjjhwx.cn

CREATE TABLE orders (
来源：http://sn.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lp.jctech888.com.cn

user_id INT NOT NULL,
来源：http://ww.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://hw.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mw.gzmigu.cn

);
来源：http://ly.huanxung.cn

[Q03] 增加列
来源：http://wu.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wm.jctech888.com.cn

[Q04] 修改列类型
来源：http://vl.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qh.9csxet.cn

[Q05] 重命名列
来源：http://ux.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rw.shxzukj.cn

[Q06] 删除列
来源：http://al.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fg.newstarts.cn

[Q07] 删除表
来源：http://ye.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://fo.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://sm.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ec.nszjky.cn

[Q09] 创建唯一索引
来源：http://yd.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tq.haigaiapp.cn

[Q10] 插入单行
来源：http://oh.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vo.huixiangedu.cn

[Q11] 一次插入多行
来源：http://wm.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qb.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://xo.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hi.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ym.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://ua.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rk.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://hf.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://or.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mp.hahajie.cn

[Q15] 查询全部
来源：http://dm.521024.cn

SELECT * FROM users;
来源：http://kc.521024.cn

[Q16] 查询指定列
来源：http://ky.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://ri.szxytkj.cn

[Q17] 条件查询
来源：http://df.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yh.shxzukj.cn

[Q18] 模糊匹配
来源：http://px.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pf.panjiajie.cn

[Q19] 范围查询
来源：http://dq.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ir.chemitech.net.cn

[Q20] IN 列表
来源：http://wo.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wi.yuexingan06.cn

[Q21] 空值判断
来源：http://nd.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gg.huixinmuqiang.cn

[Q22] 排序
来源：http://oh.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jk.shtwfgs.cn

[Q23] 分页
来源：http://ny.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xl.nicolike.cn

[Q24] 去重
来源：http://if.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://tl.szxytkj.cn

[Q25] 只取前 N 条
来源：http://zd.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yp.hnjuh.cn

[Q26] 计数
来源：http://ry.521024.cn

SELECT COUNT(*) FROM users;
来源：http://zy.shxzukj.cn

[Q27] 条件计数
来源：http://gn.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://to.521024.cn

[Q28] 求和与平均
来源：http://tk.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ba.colortex.cn

[Q29] 最大最小值
来源：http://es.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ye.jianghongdianzi.cn

[Q30] 分组统计
来源：http://lz.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qr.jctech888.com.cn

[Q31] 分组后过滤
来源：http://zt.panjiajie.cn


<!-- 参考信息 -->