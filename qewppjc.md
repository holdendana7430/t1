代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://up.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://md.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oi.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://rw.muxihuayi.cn

Ruby: arr.sort
来源：http://da.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eg.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://lr.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ih.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://jl.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://md.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qd.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pe.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ys.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uc.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ki.9csxet.cn

[N04] 斐波那契数列
来源：http://jv.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ff.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://px.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://or.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vt.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lv.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zk.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xh.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://un.haigaiapp.cn

[N05] 最大公约数
来源：http://nn.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://lx.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ea.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lh.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jn.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oi.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ew.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://ps.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qd.szsharing.cn

[N06] 判断回文字符串
来源：http://uv.szxytkj.cn

Py:   s == s[::-1]
来源：http://el.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://nr.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://zv.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://ca.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fv.colortex.cn

Go:   // 双指针从两端比较
来源：http://xv.haigaiapp.cn

Ruby: s == s.reverse
来源：http://kp.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nm.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://in.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ds.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uj.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mw.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://ee.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://xq.9csxet.cn

Go:   // 手写 map[int]int
来源：http://od.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://kj.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mu.hahajie.cn

[N08] 生成全排列
来源：http://ud.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://jr.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://iu.colortex.cn

JS:   // 手写回溯递归
来源：http://sv.lnxyls.cn

TS:   // 手写回溯递归
来源：http://oy.nicolike.cn

Java: // 手写回溯递归
来源：http://pd.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://he.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://dv.asd995.cn

C#:   // 手写回溯递归
来源：http://qk.jctech888.com.cn

[N09] 栈与队列
来源：http://qg.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fk.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yy.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ts.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zv.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pu.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rk.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zv.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eq.lnxyls.cn

[N10] 链表节点定义
来源：http://li.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qk.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ey.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ys.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gg.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://ho.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://um.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ea.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jg.asd995.cn

[N11] 二叉树中序遍历
来源：http://ec.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hq.asd995.cn

PHP:  // 手写递归函数
来源：http://pg.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ji.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wr.9csxet.cn

Java: // 手写递归
来源：http://wo.shxzukj.cn

Go:   // 手写递归
来源：http://yf.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sz.huanxung.cn

C#:   // 手写递归
来源：http://ty.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cr.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ni.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://li.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wx.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qk.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eh.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zm.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jb.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tc.yuntaijiaju.cn

================================================================================
来源：http://xk.muxihuayi.cn

O. 并发与异步
来源：http://sh.newstarts.cn

================================================================================
来源：http://kk.chemitech.net.cn

[O01] 启动一个线程
来源：http://jr.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dh.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nx.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sd.shxzskj.cn

TS:   // 同 JS
来源：http://ei.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://tp.lnxyls.cn

Go:   go f()
来源：http://cw.asd995.cn

Ruby: Thread.new { f }
来源：http://su.huanxung.cn

C#:   Task.Run(() => F());
来源：http://qa.nicolike.cn

[O02] 使用线程池
来源：http://zf.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tv.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fb.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://qg.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://cs.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bk.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jg.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kl.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xu.colortex.cn

[O03] 加锁保护共享数据
来源：http://rx.hnjuh.cn

Py:   with lock: shared += 1
来源：http://fz.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://yy.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qz.bjjhwx.cn

TS:   // 同 JS
来源：http://mm.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://rw.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wm.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cy.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://ip.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://wp.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://wp.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xj.nszjky.cn

JS:   async function f() { await g(); }
来源：http://yh.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qu.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gn.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qp.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ef.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://rm.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://zx.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://jn.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fg.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://cn.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://ox.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vn.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pq.9csxet.cn

Ruby: threads.map(&:join)
来源：http://ox.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gs.bookmarksfly.cn

[O06] 使用进程池
来源：http://tm.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lk.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zf.521024.cn

JS:   // child_process / cluster 模块
来源：http://he.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://rj.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ea.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bg.huixinmuqiang.cn

Ruby: // fork 块
来源：http://ly.muxihuayi.cn

C#:   Parallel.For
来源：http://bn.huanxung.cn

================================================================================
来源：http://ue.jianghongdianzi.cn

P. 常用工具函数
来源：http://df.hahajie.cn

================================================================================
来源：http://pf.gzmigu.cn

[P01] 生成 UUID
来源：http://ld.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://hp.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qg.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://oa.521024.cn

TS:   crypto.randomUUID()
来源：http://hp.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://ke.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://vk.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://ze.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://vw.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://em.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qz.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pe.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gg.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uk.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qd.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ig.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fj.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yy.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://sx.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ts.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dl.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mg.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xt.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zr.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ot.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ol.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uq.521024.cn

[P04] 求长度
来源：http://lp.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jc.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dn.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ir.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fq.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://gs.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://vw.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://ix.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vm.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://iv.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cx.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nu.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zr.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xa.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rc.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jk.asd995.cn

Ruby: a == b
来源：http://fm.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ck.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yh.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hc.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://sf.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zo.huixiangedu.cn

TS:   if (x == null) {}
来源：http://tx.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://es.colortex.cn

Go:   if x == nil {}
来源：http://ic.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nb.colortex.cn

C#:   if (x is null) {}
来源：http://rb.hahajie.cn

[P07] 防抖与节流
来源：http://ha.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rc.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://bq.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ny.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://du.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wb.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://av.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lj.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ab.colortex.cn

[P08] 处理浮点精度问题
来源：http://tf.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hf.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mo.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fl.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rx.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fh.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pg.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fh.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jd.shtwfgs.cn

================================================================================
来源：http://sb.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jl.hahajie.cn

================================================================================
来源：http://gy.jianghongdianzi.cn

[Q01] 创建表
来源：http://wt.asd995.cn

CREATE TABLE users (
来源：http://et.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tn.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://rv.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://np.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ln.bjjhwx.cn

);
来源：http://nr.huanxung.cn

[Q02] 创建带外键的表
来源：http://qc.lnxyls.cn

CREATE TABLE orders (
来源：http://hk.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mi.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://eg.huanxung.cn

amount DECIMAL(10, 2),
来源：http://nn.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cs.shtwfgs.cn

);
来源：http://kh.newstarts.cn

[Q03] 增加列
来源：http://es.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vq.wgjwhj.cn

[Q04] 修改列类型
来源：http://lx.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rn.yuexingan06.cn

[Q05] 重命名列
来源：http://ol.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wt.huixinmuqiang.cn

[Q06] 删除列
来源：http://hs.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://je.wgjwhj.cn

[Q07] 删除表
来源：http://he.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://on.bjjhwx.cn

[Q08] 创建普通索引
来源：http://pd.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hq.lnxyls.cn

[Q09] 创建唯一索引
来源：http://ek.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qi.colortex.cn

[Q10] 插入单行
来源：http://kz.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tq.newstarts.cn

[Q11] 一次插入多行
来源：http://we.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bw.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://ih.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eo.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ol.colortex.cn

[Q13] 忽略重复插入
来源：http://dt.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ii.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://jo.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jf.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bx.panjiajie.cn

[Q15] 查询全部
来源：http://sm.muxihuayi.cn

SELECT * FROM users;
来源：http://ro.colortex.cn

[Q16] 查询指定列
来源：http://af.szsharing.cn

SELECT id, name FROM users;
来源：http://eg.shxzukj.cn

[Q17] 条件查询
来源：http://ge.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://td.jctech888.com.cn

[Q18] 模糊匹配
来源：http://kd.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://er.hnjuh.cn

[Q19] 范围查询
来源：http://ft.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qe.jctech888.com.cn

[Q20] IN 列表
来源：http://cc.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qn.hnjuh.cn

[Q21] 空值判断
来源：http://qi.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ph.chemitech.net.cn

[Q22] 排序
来源：http://nt.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tq.newstarts.cn

[Q23] 分页
来源：http://eb.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hh.jctech888.com.cn

[Q24] 去重
来源：http://lp.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://eb.asd995.cn

[Q25] 只取前 N 条
来源：http://af.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://do.wgjwhj.cn

[Q26] 计数
来源：http://up.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://gs.jianghongdianzi.cn

[Q27] 条件计数
来源：http://tm.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qb.nszjky.cn

[Q28] 求和与平均
来源：http://sg.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lg.shxzskj.cn

[Q29] 最大最小值
来源：http://dc.chemitech.net.cn


<!-- 参考信息 -->