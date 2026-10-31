代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ba.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sk.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ky.huixiangedu.cn

[N04] 斐波那契数列
来源：http://vh.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pz.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cu.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hb.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eq.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ty.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zp.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dn.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kh.yuexingan06.cn

[N05] 最大公约数
来源：http://ei.asd995.cn

Py:   math.gcd(a, b)
来源：http://qh.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uf.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xl.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://up.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zb.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eb.hnjuh.cn

Ruby: a.gcd(b)
来源：http://zp.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mn.newstarts.cn

[N06] 判断回文字符串
来源：http://iy.shxzukj.cn

Py:   s == s[::-1]
来源：http://ru.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://se.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://cx.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://kq.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ua.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ec.muxihuayi.cn

Ruby: s == s.reverse
来源：http://zd.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rk.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://xy.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ey.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ib.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ir.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://ou.lnxyls.cn

Java: // 手写 HashMap
来源：http://yn.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://io.lnxyls.cn

Ruby: // 手写 Hash
来源：http://pt.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ln.chemitech.net.cn

[N08] 生成全排列
来源：http://br.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://os.szsharing.cn

PHP:  // 手写递归交换
来源：http://fu.lnxyls.cn

JS:   // 手写回溯递归
来源：http://zi.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://qw.wgjwhj.cn

Java: // 手写回溯递归
来源：http://sg.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://rk.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://br.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://tg.wgjwhj.cn

[N09] 栈与队列
来源：http://xv.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hb.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://le.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oh.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hb.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iu.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ge.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pj.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eo.lnxyls.cn

[N10] 链表节点定义
来源：http://bz.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://as.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ne.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://un.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iz.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://xw.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://es.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qd.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wz.huanxung.cn

[N11] 二叉树中序遍历
来源：http://fy.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jh.hahajie.cn

PHP:  // 手写递归函数
来源：http://eu.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://it.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tu.jianghongdianzi.cn

Java: // 手写递归
来源：http://ys.bjjhwx.cn

Go:   // 手写递归
来源：http://iw.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ak.hnjuh.cn

C#:   // 手写递归
来源：http://jl.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ee.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ri.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jl.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://np.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ko.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dh.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pg.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pw.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dy.lnxyls.cn

================================================================================
来源：http://ze.huixiangedu.cn

O. 并发与异步
来源：http://wi.huixinmuqiang.cn

================================================================================
来源：http://gb.panjiajie.cn

[O01] 启动一个线程
来源：http://ly.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jm.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ws.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dw.shxzukj.cn

TS:   // 同 JS
来源：http://ms.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://pq.shxzukj.cn

Go:   go f()
来源：http://vl.nszjky.cn

Ruby: Thread.new { f }
来源：http://pp.hahajie.cn

C#:   Task.Run(() => F());
来源：http://os.shtwfgs.cn

[O02] 使用线程池
来源：http://lb.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ly.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ww.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://bu.colortex.cn

TS:   // worker_threads 线程池
来源：http://bi.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iw.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://so.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ln.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tk.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://kc.szxytkj.cn

Py:   with lock: shared += 1
来源：http://iy.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://bv.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://id.nicolike.cn

TS:   // 同 JS
来源：http://ax.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://bl.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mz.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hn.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://dp.asd995.cn

[O04] 定义异步函数并等待
来源：http://na.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://cv.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bj.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://sz.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xe.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pb.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xc.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ge.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://kw.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://or.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://gf.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qk.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://op.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://li.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gq.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gi.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://zc.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uh.szxytkj.cn

[O06] 使用进程池
来源：http://hq.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ws.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tn.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://xb.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://wb.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://js.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eo.bjjhwx.cn

Ruby: // fork 块
来源：http://ok.jctech888.com.cn

C#:   Parallel.For
来源：http://jp.9csxet.cn

================================================================================
来源：http://hd.wgjwhj.cn

P. 常用工具函数
来源：http://jj.jctech888.com.cn

================================================================================
来源：http://yy.szsharing.cn

[P01] 生成 UUID
来源：http://gf.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://gs.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wu.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://jh.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://dk.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://lq.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://yx.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://uz.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://bt.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://fi.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ls.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pw.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aw.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eo.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://la.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ba.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nv.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wt.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://kk.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jx.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nt.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ia.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ck.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qq.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ba.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mc.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ac.szxytkj.cn

[P04] 求长度
来源：http://ga.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hj.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uh.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gm.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hb.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://aj.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://nn.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://fa.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mf.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://ep.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ws.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tp.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sh.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tu.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hb.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jk.panjiajie.cn

Ruby: a == b
来源：http://gh.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sz.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rl.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ff.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://ts.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://en.nszjky.cn

TS:   if (x == null) {}
来源：http://xm.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vr.asd995.cn

Go:   if x == nil {}
来源：http://fs.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ke.huixiangedu.cn

C#:   if (x is null) {}
来源：http://jj.shxzukj.cn

[P07] 防抖与节流
来源：http://vj.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ej.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://il.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zg.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tc.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://je.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zo.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vj.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ow.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://wd.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vs.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ew.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rf.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zu.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aa.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wh.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://an.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ar.521024.cn

================================================================================
来源：http://dm.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qd.lnxyls.cn

================================================================================
来源：http://se.panjiajie.cn

[Q01] 创建表
来源：http://pc.chemitech.net.cn

CREATE TABLE users (
来源：http://gm.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hu.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://xr.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://mx.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ls.newstarts.cn

);
来源：http://wd.hnjuh.cn

[Q02] 创建带外键的表
来源：http://cd.szxytkj.cn

CREATE TABLE orders (
来源：http://jb.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dk.panjiajie.cn

user_id INT NOT NULL,
来源：http://jz.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://lh.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ws.gzmigu.cn

);
来源：http://ld.bookmarksfly.cn

[Q03] 增加列
来源：http://je.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qx.shxzukj.cn

[Q04] 修改列类型
来源：http://qs.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ju.newstarts.cn

[Q05] 重命名列
来源：http://ln.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cg.yuexingan06.cn

[Q06] 删除列
来源：http://ph.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jj.szxytkj.cn

[Q07] 删除表
来源：http://il.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://af.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://dr.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hm.szxytkj.cn

[Q09] 创建唯一索引
来源：http://ta.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lp.chemitech.net.cn

[Q10] 插入单行
来源：http://ii.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yi.colortex.cn

[Q11] 一次插入多行
来源：http://du.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bv.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://ak.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uk.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://we.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://mk.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://os.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://qw.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fb.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zl.lnxyls.cn

[Q15] 查询全部
来源：http://xq.nszjky.cn

SELECT * FROM users;
来源：http://lq.szsharing.cn

[Q16] 查询指定列
来源：http://pv.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://kh.jctech888.com.cn

[Q17] 条件查询
来源：http://yg.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eq.jctech888.com.cn

[Q18] 模糊匹配
来源：http://da.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qu.lnxyls.cn

[Q19] 范围查询
来源：http://cu.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://st.shtwfgs.cn

[Q20] IN 列表
来源：http://tf.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vo.hahajie.cn

[Q21] 空值判断
来源：http://lc.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nw.huixinmuqiang.cn

[Q22] 排序
来源：http://xk.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://on.panjiajie.cn

[Q23] 分页
来源：http://lq.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://un.szsharing.cn

[Q24] 去重
来源：http://po.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://vh.newstarts.cn

[Q25] 只取前 N 条
来源：http://gn.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ox.huanxung.cn

[Q26] 计数
来源：http://va.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://xb.hnjuh.cn

[Q27] 条件计数
来源：http://pd.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dj.huixiangedu.cn

[Q28] 求和与平均
来源：http://dr.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lz.wgjwhj.cn

[Q29] 最大最小值
来源：http://vt.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://er.haigaiapp.cn

[Q30] 分组统计
来源：http://tk.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ts.wgjwhj.cn

[Q31] 分组后过滤
来源：http://kn.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nj.9csxet.cn

[Q32] 分组拼接字符串
来源：http://dy.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wj.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cb.panjiajie.cn

[Q33] 多列分组
来源：http://fn.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ad.jctech888.com.cn

[Q34] 每组取第一条
来源：http://kg.colortex.cn

SELECT * FROM (
来源：http://nu.haigaiapp.cn


<!-- 参考信息 -->