代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://qe.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nb.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hf.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sl.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dy.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hu.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://to.hahajie.cn

[N04] 斐波那契数列
来源：http://mj.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dz.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jn.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xd.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qc.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dc.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pn.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xq.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lw.hnjuh.cn

[N05] 最大公约数
来源：http://nq.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://xb.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dp.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fm.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uw.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kr.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cs.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://le.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rb.nszjky.cn

[N06] 判断回文字符串
来源：http://jd.hnjuh.cn

Py:   s == s[::-1]
来源：http://al.521024.cn

PHP:  $s === strrev($s);
来源：http://uf.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://it.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://wf.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mp.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://fc.szsharing.cn

Ruby: s == s.reverse
来源：http://lx.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ab.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://hs.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://po.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jj.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ry.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://is.gzmigu.cn

Java: // 手写 HashMap
来源：http://xf.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://cl.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://gx.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fn.shxzskj.cn

[N08] 生成全排列
来源：http://ur.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://lf.9csxet.cn

PHP:  // 手写递归交换
来源：http://rr.shxzskj.cn

JS:   // 手写回溯递归
来源：http://rj.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://xl.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://ms.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://no.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://cd.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://dg.521024.cn

[N09] 栈与队列
来源：http://ef.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kp.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qf.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ub.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lt.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uv.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zw.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ku.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hq.szxytkj.cn

[N10] 链表节点定义
来源：http://qx.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oc.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qp.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fs.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cd.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ef.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uj.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rx.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lq.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://fo.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://km.nszjky.cn

PHP:  // 手写递归函数
来源：http://ga.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://br.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fq.lnxyls.cn

Java: // 手写递归
来源：http://fs.chemitech.net.cn

Go:   // 手写递归
来源：http://ge.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ru.newstarts.cn

C#:   // 手写递归
来源：http://ho.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cd.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pa.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ch.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hj.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ff.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ve.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xm.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zq.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pk.bookmarksfly.cn

================================================================================
来源：http://fk.nicolike.cn

O. 并发与异步
来源：http://rc.521024.cn

================================================================================
来源：http://iu.jctech888.com.cn

[O01] 启动一个线程
来源：http://pf.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://de.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fh.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nc.bjjhwx.cn

TS:   // 同 JS
来源：http://fr.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://tz.haigaiapp.cn

Go:   go f()
来源：http://lw.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://iu.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://ei.shtwfgs.cn

[O02] 使用线程池
来源：http://px.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rm.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://by.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://dl.hahajie.cn

TS:   // worker_threads 线程池
来源：http://xt.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zu.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://am.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jw.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tg.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://pv.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://ki.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://cf.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yi.gzmigu.cn

TS:   // 同 JS
来源：http://da.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://qs.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jn.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rv.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://oj.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://mr.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://bc.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uq.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://ri.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jw.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yc.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vt.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ui.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://sx.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://fs.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://gm.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://py.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://oc.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://xf.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hq.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kk.hahajie.cn

Ruby: threads.map(&:join)
来源：http://of.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hn.jctech888.com.cn

[O06] 使用进程池
来源：http://mi.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hb.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tu.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://rq.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://pj.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wt.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nk.yuexingan06.cn

Ruby: // fork 块
来源：http://qi.521024.cn

C#:   Parallel.For
来源：http://ts.huixinmuqiang.cn

================================================================================
来源：http://ru.muxihuayi.cn

P. 常用工具函数
来源：http://ui.huanxung.cn

================================================================================
来源：http://iz.szxytkj.cn

[P01] 生成 UUID
来源：http://ht.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://lh.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hu.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://lh.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://we.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://no.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://ge.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://vj.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://cy.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://tb.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nn.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://by.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pz.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qp.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jd.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qk.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rx.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sn.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://yr.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ex.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oc.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sm.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mi.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rg.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kr.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ze.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ma.colortex.cn

[P04] 求长度
来源：http://cm.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ww.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ds.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xv.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cq.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://bs.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://jd.szsharing.cn

Ruby: x.length;  x.size
来源：http://hg.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cd.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://dv.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hb.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nk.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hu.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hr.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mo.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vj.huixiangedu.cn

Ruby: a == b
来源：http://uv.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://un.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wp.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vz.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://fw.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fe.szxytkj.cn

TS:   if (x == null) {}
来源：http://cl.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rn.panjiajie.cn

Go:   if x == nil {}
来源：http://tt.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yu.nicolike.cn

C#:   if (x is null) {}
来源：http://gm.nicolike.cn

[P07] 防抖与节流
来源：http://ko.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://py.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://yi.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lg.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qu.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://se.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://od.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ix.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dd.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://ja.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rv.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pb.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uh.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aq.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pb.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://og.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ex.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vx.huixinmuqiang.cn

================================================================================
来源：http://kx.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uw.jctech888.com.cn

================================================================================
来源：http://pq.panjiajie.cn

[Q01] 创建表
来源：http://xh.colortex.cn

CREATE TABLE users (
来源：http://ou.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zq.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://wk.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ao.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ua.shxzukj.cn

);
来源：http://so.panjiajie.cn

[Q02] 创建带外键的表
来源：http://lm.muxihuayi.cn

CREATE TABLE orders (
来源：http://gt.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://em.hnjuh.cn

user_id INT NOT NULL,
来源：http://iq.huanxung.cn

amount DECIMAL(10, 2),
来源：http://yo.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://or.shtwfgs.cn

);
来源：http://ys.hnjuh.cn

[Q03] 增加列
来源：http://lu.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://us.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://vz.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://of.jctech888.com.cn

[Q05] 重命名列
来源：http://lt.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nl.muxihuayi.cn

[Q06] 删除列
来源：http://qp.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hq.wgjwhj.cn

[Q07] 删除表
来源：http://ie.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://kq.haigaiapp.cn

[Q08] 创建普通索引
来源：http://xk.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fo.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://tc.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ed.muxihuayi.cn

[Q10] 插入单行
来源：http://rj.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ph.chemitech.net.cn

[Q11] 一次插入多行
来源：http://cz.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nm.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://vh.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pj.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lu.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://ut.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://go.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://vn.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nk.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pm.haigaiapp.cn

[Q15] 查询全部
来源：http://sg.huixiangedu.cn

SELECT * FROM users;
来源：http://du.bookmarksfly.cn

[Q16] 查询指定列
来源：http://ij.newstarts.cn

SELECT id, name FROM users;
来源：http://zk.wgjwhj.cn

[Q17] 条件查询
来源：http://kt.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wf.hahajie.cn

[Q18] 模糊匹配
来源：http://om.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qu.huixinmuqiang.cn

[Q19] 范围查询
来源：http://kg.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://di.jianghongdianzi.cn

[Q20] IN 列表
来源：http://pe.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mr.panjiajie.cn

[Q21] 空值判断
来源：http://pw.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hy.521024.cn

[Q22] 排序
来源：http://rx.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rc.nszjky.cn

[Q23] 分页
来源：http://qm.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gv.lnxyls.cn

[Q24] 去重
来源：http://yo.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://aa.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://ce.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rt.huixiangedu.cn

[Q26] 计数
来源：http://le.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://jr.wgjwhj.cn

[Q27] 条件计数
来源：http://cr.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oe.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://zu.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kv.wgjwhj.cn

[Q29] 最大最小值
来源：http://gl.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cb.szxytkj.cn

[Q30] 分组统计
来源：http://dg.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ei.haigaiapp.cn

[Q31] 分组后过滤
来源：http://hg.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://op.newstarts.cn

[Q32] 分组拼接字符串
来源：http://dy.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fj.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fq.hahajie.cn


<!-- 参考信息 -->