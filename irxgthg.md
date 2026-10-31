代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nw.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gq.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://om.yuexingan06.cn

[N04] 斐波那契数列
来源：http://dh.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ml.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cw.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jy.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kk.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ga.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://il.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://im.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pd.gzmigu.cn

[N05] 最大公约数
来源：http://ew.nicolike.cn

Py:   math.gcd(a, b)
来源：http://nw.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oa.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uo.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mk.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rx.hnjuh.cn

Ruby: a.gcd(b)
来源：http://yn.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://am.muxihuayi.cn

[N06] 判断回文字符串
来源：http://tf.nszjky.cn

Py:   s == s[::-1]
来源：http://wh.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://ig.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://af.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://rd.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xm.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://nm.haigaiapp.cn

Ruby: s == s.reverse
来源：http://rc.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xe.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://zm.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ht.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oz.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://an.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://cd.panjiajie.cn

Java: // 手写 HashMap
来源：http://of.nszjky.cn

Go:   // 手写 map[int]int
来源：http://qb.gzmigu.cn

Ruby: // 手写 Hash
来源：http://cn.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://in.haigaiapp.cn

[N08] 生成全排列
来源：http://vs.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://uy.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://qm.szsharing.cn

JS:   // 手写回溯递归
来源：http://xx.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://cv.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://no.9csxet.cn

Go:   // 手写回溯递归
来源：http://xc.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://ha.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://qj.huixinmuqiang.cn

[N09] 栈与队列
来源：http://io.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rw.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://st.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cj.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xp.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xc.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zm.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bw.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rv.panjiajie.cn

[N10] 链表节点定义
来源：http://xx.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pw.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dj.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jk.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bt.521024.cn

Java: class Node { int v; Node next; }
来源：http://cg.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mo.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vj.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hu.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://yk.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://un.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://hy.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pu.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kv.hnjuh.cn

Java: // 手写递归
来源：http://zw.newstarts.cn

Go:   // 手写递归
来源：http://xd.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mg.nicolike.cn

C#:   // 手写递归
来源：http://mh.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zc.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kl.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tc.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yw.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ac.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sr.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ap.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ln.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ls.huixiangedu.cn

================================================================================
来源：http://bg.shxzukj.cn

O. 并发与异步
来源：http://le.521024.cn

================================================================================
来源：http://gr.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://vu.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oi.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qi.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jl.haigaiapp.cn

TS:   // 同 JS
来源：http://us.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://qm.haigaiapp.cn

Go:   go f()
来源：http://mu.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://fu.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://cj.panjiajie.cn

[O02] 使用线程池
来源：http://wk.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rh.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uw.colortex.cn

JS:   // worker_threads 线程池
来源：http://yf.asd995.cn

TS:   // worker_threads 线程池
来源：http://ea.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jq.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qd.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uu.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rz.nicolike.cn

[O03] 加锁保护共享数据
来源：http://fj.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://jy.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://fh.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ku.wgjwhj.cn

TS:   // 同 JS
来源：http://yk.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://nb.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uy.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ue.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://xc.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://mv.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://js.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kk.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://ep.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jm.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dx.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ok.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lm.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://vt.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://xw.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://xi.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://br.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://sl.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://lk.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yx.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oq.9csxet.cn

Ruby: threads.map(&:join)
来源：http://iy.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ni.muxihuayi.cn

[O06] 使用进程池
来源：http://aj.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kp.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qo.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://pg.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://oe.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yo.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ro.asd995.cn

Ruby: // fork 块
来源：http://ji.9csxet.cn

C#:   Parallel.For
来源：http://iv.shxzukj.cn

================================================================================
来源：http://ah.szxytkj.cn

P. 常用工具函数
来源：http://pe.hahajie.cn

================================================================================
来源：http://kk.shxzukj.cn

[P01] 生成 UUID
来源：http://br.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://fh.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ur.nszjky.cn

JS:   crypto.randomUUID()
来源：http://br.huanxung.cn

TS:   crypto.randomUUID()
来源：http://fe.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://bb.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://aj.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://hx.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://kk.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://px.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qu.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://an.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ic.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ax.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://go.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hb.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bh.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://no.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://ch.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://by.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yw.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sp.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lp.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jd.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zk.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ic.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ug.huanxung.cn

[P04] 求长度
来源：http://vx.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eh.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oi.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pn.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ln.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://qt.521024.cn

Go:   len(arr);  len(m)
来源：http://mx.9csxet.cn

Ruby: x.length;  x.size
来源：http://uu.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pr.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://jt.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ce.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://en.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sl.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://so.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mj.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hr.huixiangedu.cn

Ruby: a == b
来源：http://pr.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ww.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qa.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oi.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://nf.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rt.bjjhwx.cn

TS:   if (x == null) {}
来源：http://hy.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vj.haigaiapp.cn

Go:   if x == nil {}
来源：http://co.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gy.panjiajie.cn

C#:   if (x is null) {}
来源：http://mq.gzmigu.cn

[P07] 防抖与节流
来源：http://fb.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mm.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://kd.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oc.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://om.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hg.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mw.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cv.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://om.nszjky.cn

[P08] 处理浮点精度问题
来源：http://sp.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eh.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mk.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ma.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hl.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lf.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lx.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kn.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dn.haigaiapp.cn

================================================================================
来源：http://pt.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wb.newstarts.cn

================================================================================
来源：http://fj.panjiajie.cn

[Q01] 创建表
来源：http://da.bookmarksfly.cn

CREATE TABLE users (
来源：http://ue.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rf.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://ql.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://eq.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yv.shxzskj.cn

);
来源：http://sm.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://hw.shtwfgs.cn

CREATE TABLE orders (
来源：http://fb.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hk.asd995.cn

user_id INT NOT NULL,
来源：http://sa.szsharing.cn

amount DECIMAL(10, 2),
来源：http://ya.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kx.szxytkj.cn

);
来源：http://tj.9csxet.cn

[Q03] 增加列
来源：http://pa.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gj.lnxyls.cn

[Q04] 修改列类型
来源：http://gd.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jz.chemitech.net.cn

[Q05] 重命名列
来源：http://xw.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bs.huanxung.cn

[Q06] 删除列
来源：http://sb.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fp.huixiangedu.cn

[Q07] 删除表
来源：http://cg.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://sh.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://so.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ay.lnxyls.cn

[Q09] 创建唯一索引
来源：http://do.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://df.huixiangedu.cn

[Q10] 插入单行
来源：http://tx.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://db.hnjuh.cn

[Q11] 一次插入多行
来源：http://pp.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dc.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://cx.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kh.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jo.nicolike.cn

[Q13] 忽略重复插入
来源：http://ai.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tq.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://fw.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xf.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lm.huixinmuqiang.cn

[Q15] 查询全部
来源：http://xf.huanxung.cn

SELECT * FROM users;
来源：http://wp.muxihuayi.cn

[Q16] 查询指定列
来源：http://ob.hnjuh.cn

SELECT id, name FROM users;
来源：http://of.nicolike.cn

[Q17] 条件查询
来源：http://bw.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cd.chemitech.net.cn

[Q18] 模糊匹配
来源：http://zl.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pp.shxzukj.cn

[Q19] 范围查询
来源：http://ix.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://no.chemitech.net.cn

[Q20] IN 列表
来源：http://yy.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jq.shxzukj.cn

[Q21] 空值判断
来源：http://ke.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xu.nszjky.cn

[Q22] 排序
来源：http://nm.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tl.szxytkj.cn

[Q23] 分页
来源：http://ck.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qx.gzmigu.cn

[Q24] 去重
来源：http://sd.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://dm.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://os.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qb.gzmigu.cn

[Q26] 计数
来源：http://gi.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://li.asd995.cn

[Q27] 条件计数
来源：http://hh.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xj.yuexingan06.cn

[Q28] 求和与平均
来源：http://iw.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kk.jctech888.com.cn

[Q29] 最大最小值
来源：http://rt.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yq.yuexingan06.cn

[Q30] 分组统计
来源：http://yx.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kw.9csxet.cn

[Q31] 分组后过滤
来源：http://qh.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yt.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://pe.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ac.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bd.lnxyls.cn

[Q33] 多列分组
来源：http://yl.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vx.shxzukj.cn

[Q34] 每组取第一条
来源：http://zp.hahajie.cn

SELECT * FROM (
来源：http://hp.muxihuayi.cn


<!-- 参考信息 -->