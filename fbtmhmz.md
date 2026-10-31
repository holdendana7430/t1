代发 wailian999

Ruby: arr.sort
来源：http://cd.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wp.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://yr.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ii.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://dj.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ot.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jh.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jn.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wg.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qd.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kq.newstarts.cn

[N04] 斐波那契数列
来源：http://kd.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iu.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qz.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mr.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qj.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gz.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fr.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yu.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fp.lnxyls.cn

[N05] 最大公约数
来源：http://qg.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://cw.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uq.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qd.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cq.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dh.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lo.nszjky.cn

Ruby: a.gcd(b)
来源：http://mp.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lt.lnxyls.cn

[N06] 判断回文字符串
来源：http://ao.asd995.cn

Py:   s == s[::-1]
来源：http://cb.newstarts.cn

PHP:  $s === strrev($s);
来源：http://mh.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://nv.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://qt.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ux.nszjky.cn

Go:   // 双指针从两端比较
来源：http://ty.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://ev.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rh.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://mu.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qe.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pf.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gt.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://tz.gzmigu.cn

Java: // 手写 HashMap
来源：http://py.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://ta.szsharing.cn

Ruby: // 手写 Hash
来源：http://sp.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dj.521024.cn

[N08] 生成全排列
来源：http://rg.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ng.colortex.cn

PHP:  // 手写递归交换
来源：http://sj.gzmigu.cn

JS:   // 手写回溯递归
来源：http://va.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://er.asd995.cn

Java: // 手写回溯递归
来源：http://qc.hnjuh.cn

Go:   // 手写回溯递归
来源：http://nh.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://ru.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://uf.huixinmuqiang.cn

[N09] 栈与队列
来源：http://uq.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tv.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xm.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://se.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ei.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bx.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://et.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://es.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zm.9csxet.cn

[N10] 链表节点定义
来源：http://oh.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dc.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://im.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kg.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bj.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://fa.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://or.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ki.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ro.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://xz.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ys.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://dc.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gp.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://th.hahajie.cn

Java: // 手写递归
来源：http://tj.huixinmuqiang.cn

Go:   // 手写递归
来源：http://jq.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ce.shxzukj.cn

C#:   // 手写递归
来源：http://qv.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qb.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mz.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://al.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ac.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oa.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yz.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nt.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pu.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bg.wgjwhj.cn

================================================================================
来源：http://kv.szsharing.cn

O. 并发与异步
来源：http://hf.panjiajie.cn

================================================================================
来源：http://gx.nicolike.cn

[O01] 启动一个线程
来源：http://ib.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wq.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jx.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bw.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ea.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://sy.haigaiapp.cn

Go:   go f()
来源：http://eh.szsharing.cn

Ruby: Thread.new { f }
来源：http://qd.hahajie.cn

C#:   Task.Run(() => F());
来源：http://sc.hahajie.cn

[O02] 使用线程池
来源：http://xm.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ft.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ak.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://vl.huanxung.cn

TS:   // worker_threads 线程池
来源：http://rf.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xv.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ue.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qx.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cp.nszjky.cn

[O03] 加锁保护共享数据
来源：http://ut.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://ht.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://xz.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ja.bookmarksfly.cn

TS:   // 同 JS
来源：http://wg.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://nj.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dp.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lv.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://cy.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://ia.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://ns.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wr.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://mo.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oh.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cm.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://de.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wq.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://bq.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://rx.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://uo.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fu.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://tv.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://uj.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wf.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yg.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://lb.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bm.newstarts.cn

[O06] 使用进程池
来源：http://zj.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://db.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lw.521024.cn

JS:   // child_process / cluster 模块
来源：http://zb.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://no.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ux.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://la.shtwfgs.cn

Ruby: // fork 块
来源：http://wi.bookmarksfly.cn

C#:   Parallel.For
来源：http://iw.asd995.cn

================================================================================
来源：http://wn.yuexingan06.cn

P. 常用工具函数
来源：http://cn.shtwfgs.cn

================================================================================
来源：http://vf.asd995.cn

[P01] 生成 UUID
来源：http://vv.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://ie.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mi.nicolike.cn

JS:   crypto.randomUUID()
来源：http://nh.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://xu.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://pe.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://yn.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://bs.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://px.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://lq.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rm.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cp.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hv.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://na.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yk.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://km.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sa.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ce.szsharing.cn

[P03] 生成短随机字符串
来源：http://vp.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iw.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wn.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://te.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ds.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bf.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ku.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rd.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yq.hnjuh.cn

[P04] 求长度
来源：http://ie.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nc.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://im.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hd.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yl.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://or.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://gg.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://xi.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ir.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://dm.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ge.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pa.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mn.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ul.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tl.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qm.asd995.cn

Ruby: a == b
来源：http://dp.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nn.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ao.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vj.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://sh.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rk.bjjhwx.cn

TS:   if (x == null) {}
来源：http://dt.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cl.newstarts.cn

Go:   if x == nil {}
来源：http://pi.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vp.shxzukj.cn

C#:   if (x is null) {}
来源：http://wf.jctech888.com.cn

[P07] 防抖与节流
来源：http://py.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ec.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://zy.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://an.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kj.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bt.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hf.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oe.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xd.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://ga.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pc.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yf.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zk.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xp.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xk.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ln.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qv.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kg.haigaiapp.cn

================================================================================
来源：http://yy.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ga.shtwfgs.cn

================================================================================
来源：http://sc.colortex.cn

[Q01] 创建表
来源：http://xi.muxihuayi.cn

CREATE TABLE users (
来源：http://ob.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lw.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://nr.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://yz.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dx.jctech888.com.cn

);
来源：http://jq.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://dv.jctech888.com.cn

CREATE TABLE orders (
来源：http://zs.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mv.haigaiapp.cn

user_id INT NOT NULL,
来源：http://by.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://pt.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rq.chemitech.net.cn

);
来源：http://ui.szsharing.cn

[Q03] 增加列
来源：http://tq.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pv.lnxyls.cn

[Q04] 修改列类型
来源：http://ki.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cq.panjiajie.cn

[Q05] 重命名列
来源：http://by.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ni.shxzukj.cn

[Q06] 删除列
来源：http://xv.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pf.huixiangedu.cn

[Q07] 删除表
来源：http://tw.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://vw.shtwfgs.cn

[Q08] 创建普通索引
来源：http://vh.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ga.nicolike.cn

[Q09] 创建唯一索引
来源：http://kh.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fx.huixiangedu.cn

[Q10] 插入单行
来源：http://cq.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://za.521024.cn

[Q11] 一次插入多行
来源：http://ru.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eu.colortex.cn

[Q12] 插入后取自增 ID
来源：http://nt.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pr.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ck.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://bg.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ut.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://bi.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gh.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cq.muxihuayi.cn

[Q15] 查询全部
来源：http://fo.gzmigu.cn

SELECT * FROM users;
来源：http://fg.szxytkj.cn

[Q16] 查询指定列
来源：http://jt.newstarts.cn

SELECT id, name FROM users;
来源：http://ac.bjjhwx.cn

[Q17] 条件查询
来源：http://qj.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cp.szxytkj.cn

[Q18] 模糊匹配
来源：http://lz.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lr.yuntaijiaju.cn

[Q19] 范围查询
来源：http://ug.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hh.asd995.cn

[Q20] IN 列表
来源：http://mh.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tl.szsharing.cn

[Q21] 空值判断
来源：http://su.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yi.shxzskj.cn

[Q22] 排序
来源：http://ib.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bm.chemitech.net.cn

[Q23] 分页
来源：http://dr.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cg.bjjhwx.cn

[Q24] 去重
来源：http://og.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://lb.nszjky.cn

[Q25] 只取前 N 条
来源：http://kz.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zr.gzmigu.cn

[Q26] 计数
来源：http://ko.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://nk.chemitech.net.cn

[Q27] 条件计数
来源：http://oc.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://md.yuexingan06.cn

[Q28] 求和与平均
来源：http://ys.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tr.szxytkj.cn

[Q29] 最大最小值
来源：http://gy.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yx.newstarts.cn

[Q30] 分组统计
来源：http://pf.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gd.szsharing.cn

[Q31] 分组后过滤
来源：http://vl.nicolike.cn


<!-- 参考信息 -->