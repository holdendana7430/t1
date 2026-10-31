代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://ug.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nd.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pi.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pg.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wf.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qv.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jq.jctech888.com.cn

[N04] 斐波那契数列
来源：http://tg.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://js.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wv.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xb.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://do.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ny.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://as.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yv.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://da.muxihuayi.cn

[N05] 最大公约数
来源：http://yh.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://wb.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jf.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://du.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ur.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zh.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dg.huanxung.cn

Ruby: a.gcd(b)
来源：http://ue.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sj.9csxet.cn

[N06] 判断回文字符串
来源：http://mn.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://wq.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://mk.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://sp.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://om.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gd.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://en.huanxung.cn

Ruby: s == s.reverse
来源：http://wp.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rj.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://tn.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://df.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ok.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nw.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://vm.wgjwhj.cn

Java: // 手写 HashMap
来源：http://cy.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://zb.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ty.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ir.huanxung.cn

[N08] 生成全排列
来源：http://se.521024.cn

Py:   itertools.permutations(arr)
来源：http://du.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://fh.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://bd.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://vo.huixiangedu.cn

Java: // 手写回溯递归
来源：http://iq.newstarts.cn

Go:   // 手写回溯递归
来源：http://vb.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://zd.lnxyls.cn

C#:   // 手写回溯递归
来源：http://uj.asd995.cn

[N09] 栈与队列
来源：http://my.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ng.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hd.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tq.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zq.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ee.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ie.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yd.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ur.newstarts.cn

[N10] 链表节点定义
来源：http://pg.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://it.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bw.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ff.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hk.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://ap.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zt.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dt.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wd.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://hc.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gj.szxytkj.cn

PHP:  // 手写递归函数
来源：http://ky.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ll.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ga.colortex.cn

Java: // 手写递归
来源：http://lg.lnxyls.cn

Go:   // 手写递归
来源：http://el.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zu.szxytkj.cn

C#:   // 手写递归
来源：http://ar.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ka.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zv.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tx.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lm.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sv.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yu.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://em.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gf.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://if.nszjky.cn

================================================================================
来源：http://xj.9csxet.cn

O. 并发与异步
来源：http://iu.huixinmuqiang.cn

================================================================================
来源：http://pk.nicolike.cn

[O01] 启动一个线程
来源：http://nm.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nq.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ot.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://he.colortex.cn

TS:   // 同 JS
来源：http://tl.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://xo.wgjwhj.cn

Go:   go f()
来源：http://iq.nszjky.cn

Ruby: Thread.new { f }
来源：http://jy.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://on.huixinmuqiang.cn

[O02] 使用线程池
来源：http://ed.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sk.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://hw.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://aq.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cd.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hg.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dc.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cs.hahajie.cn

[O03] 加锁保护共享数据
来源：http://cp.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://ag.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://vy.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kp.szsharing.cn

TS:   // 同 JS
来源：http://mx.521024.cn

Java: synchronized (this) { shared++; }
来源：http://ro.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hq.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gf.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://kk.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://gi.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://lr.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://we.szsharing.cn

JS:   async function f() { await g(); }
来源：http://bk.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://du.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xn.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jl.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kb.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://st.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://uy.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://bm.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ej.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://ie.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://ri.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mf.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uc.9csxet.cn

Ruby: threads.map(&:join)
来源：http://vg.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://su.yuntaijiaju.cn

[O06] 使用进程池
来源：http://zb.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zf.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zx.521024.cn

JS:   // child_process / cluster 模块
来源：http://eu.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://un.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lz.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pm.colortex.cn

Ruby: // fork 块
来源：http://tp.huixiangedu.cn

C#:   Parallel.For
来源：http://vp.gzmigu.cn

================================================================================
来源：http://qj.wgjwhj.cn

P. 常用工具函数
来源：http://cu.gzmigu.cn

================================================================================
来源：http://gi.szsharing.cn

[P01] 生成 UUID
来源：http://jf.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://kv.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lh.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://mu.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://pp.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://rt.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://sq.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://xw.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://pe.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://dr.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cz.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ma.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pv.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xe.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hd.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pm.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zc.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://in.521024.cn

[P03] 生成短随机字符串
来源：http://vo.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gb.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wp.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vj.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jg.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://db.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oo.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ms.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ig.shtwfgs.cn

[P04] 求长度
来源：http://cg.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ai.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yt.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yi.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gg.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://ss.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://bo.panjiajie.cn

Ruby: x.length;  x.size
来源：http://dt.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kf.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://xs.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://io.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zd.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dw.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hq.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rt.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://se.lnxyls.cn

Ruby: a == b
来源：http://oh.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xc.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qn.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tl.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://ru.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rd.newstarts.cn

TS:   if (x == null) {}
来源：http://zl.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ne.newstarts.cn

Go:   if x == nil {}
来源：http://bi.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ny.wgjwhj.cn

C#:   if (x is null) {}
来源：http://vl.chemitech.net.cn

[P07] 防抖与节流
来源：http://kx.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ua.asd995.cn

PHP:  // 手写时间戳比较
来源：http://fr.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://en.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zp.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ja.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://at.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hv.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sv.521024.cn

[P08] 处理浮点精度问题
来源：http://kv.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rx.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uo.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aj.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tt.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kc.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mz.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fl.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iw.521024.cn

================================================================================
来源：http://hb.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ni.jctech888.com.cn

================================================================================
来源：http://ld.shxzskj.cn

[Q01] 创建表
来源：http://yz.lnxyls.cn

CREATE TABLE users (
来源：http://mq.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cz.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://wr.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://ba.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ye.szxytkj.cn

);
来源：http://dj.newstarts.cn

[Q02] 创建带外键的表
来源：http://bi.bookmarksfly.cn

CREATE TABLE orders (
来源：http://wl.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ke.hnjuh.cn

user_id INT NOT NULL,
来源：http://hj.nszjky.cn

amount DECIMAL(10, 2),
来源：http://mq.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ma.bookmarksfly.cn

);
来源：http://ex.muxihuayi.cn

[Q03] 增加列
来源：http://gf.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lw.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://zt.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://il.521024.cn

[Q05] 重命名列
来源：http://zj.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yh.muxihuayi.cn

[Q06] 删除列
来源：http://nk.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jv.jctech888.com.cn

[Q07] 删除表
来源：http://mm.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://nb.bjjhwx.cn

[Q08] 创建普通索引
来源：http://ul.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hl.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://vd.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ig.huixinmuqiang.cn

[Q10] 插入单行
来源：http://ja.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pz.hnjuh.cn

[Q11] 一次插入多行
来源：http://pv.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ao.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://wk.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lq.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hs.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://wa.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xc.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://vm.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iv.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zk.chemitech.net.cn

[Q15] 查询全部
来源：http://on.yuexingan06.cn

SELECT * FROM users;
来源：http://sm.gzmigu.cn

[Q16] 查询指定列
来源：http://cy.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://ph.szxytkj.cn

[Q17] 条件查询
来源：http://pc.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mu.szsharing.cn

[Q18] 模糊匹配
来源：http://ec.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ld.haigaiapp.cn

[Q19] 范围查询
来源：http://hq.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://re.huixinmuqiang.cn

[Q20] IN 列表
来源：http://eu.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lz.bookmarksfly.cn

[Q21] 空值判断
来源：http://jm.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nb.haigaiapp.cn

[Q22] 排序
来源：http://ci.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ko.9csxet.cn

[Q23] 分页
来源：http://eb.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rn.jctech888.com.cn

[Q24] 去重
来源：http://hm.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://pl.nicolike.cn

[Q25] 只取前 N 条
来源：http://zr.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yv.shtwfgs.cn

[Q26] 计数
来源：http://jc.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://nd.szxytkj.cn

[Q27] 条件计数
来源：http://qg.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bc.shxzskj.cn

[Q28] 求和与平均
来源：http://sp.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nw.muxihuayi.cn

[Q29] 最大最小值
来源：http://nm.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xj.hnjuh.cn

[Q30] 分组统计
来源：http://kw.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gx.wgjwhj.cn

[Q31] 分组后过滤
来源：http://xo.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ox.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://qi.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eo.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bm.wgjwhj.cn


<!-- 参考信息 -->