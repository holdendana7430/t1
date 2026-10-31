代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jo.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jr.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zu.9csxet.cn

[N04] 斐波那契数列
来源：http://zh.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://no.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://su.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xq.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ef.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mu.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qc.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aa.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jr.jianghongdianzi.cn

[N05] 最大公约数
来源：http://en.521024.cn

Py:   math.gcd(a, b)
来源：http://zm.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gk.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xx.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vf.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rq.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iq.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://rs.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aq.colortex.cn

[N06] 判断回文字符串
来源：http://dg.chemitech.net.cn

Py:   s == s[::-1]
来源：http://zx.huanxung.cn

PHP:  $s === strrev($s);
来源：http://bh.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://uo.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://kd.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eb.hahajie.cn

Go:   // 双指针从两端比较
来源：http://jv.hnjuh.cn

Ruby: s == s.reverse
来源：http://bg.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cj.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://td.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lg.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zo.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iq.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://no.huixiangedu.cn

Java: // 手写 HashMap
来源：http://ge.asd995.cn

Go:   // 手写 map[int]int
来源：http://cs.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ll.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qr.shxzskj.cn

[N08] 生成全排列
来源：http://nd.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://up.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://hp.9csxet.cn

JS:   // 手写回溯递归
来源：http://pz.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://ez.yuexingan06.cn

Java: // 手写回溯递归
来源：http://bk.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ce.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ib.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://vo.jctech888.com.cn

[N09] 栈与队列
来源：http://qg.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ze.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dd.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ey.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rz.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sq.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zj.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mk.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://es.newstarts.cn

[N10] 链表节点定义
来源：http://jf.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hc.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://le.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dx.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fb.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://dm.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rh.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ew.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://df.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://qu.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ug.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://lg.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pe.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xl.nszjky.cn

Java: // 手写递归
来源：http://hd.colortex.cn

Go:   // 手写递归
来源：http://nq.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cv.hnjuh.cn

C#:   // 手写递归
来源：http://yy.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zf.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sa.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uj.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pl.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kb.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qr.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fg.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lr.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ve.jianghongdianzi.cn

================================================================================
来源：http://cp.chemitech.net.cn

O. 并发与异步
来源：http://wz.nicolike.cn

================================================================================
来源：http://ka.asd995.cn

[O01] 启动一个线程
来源：http://bw.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qp.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jp.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ae.9csxet.cn

TS:   // 同 JS
来源：http://eu.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://bg.asd995.cn

Go:   go f()
来源：http://ap.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://th.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://le.chemitech.net.cn

[O02] 使用线程池
来源：http://de.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vf.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oz.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://vp.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://ys.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ls.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yq.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sv.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ti.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://gx.szxytkj.cn

Py:   with lock: shared += 1
来源：http://wd.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://fm.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tx.shtwfgs.cn

TS:   // 同 JS
来源：http://vb.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://sj.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yq.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://el.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://hw.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://ft.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://vw.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://la.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://fj.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://br.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nk.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ie.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yk.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://ow.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://sm.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://xd.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rt.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://ym.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://wc.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jb.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uc.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ey.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qf.huixinmuqiang.cn

[O06] 使用进程池
来源：http://fn.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vc.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ez.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://ug.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://nt.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bx.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://um.yuexingan06.cn

Ruby: // fork 块
来源：http://uz.yuntaijiaju.cn

C#:   Parallel.For
来源：http://yg.szsharing.cn

================================================================================
来源：http://cb.bookmarksfly.cn

P. 常用工具函数
来源：http://jt.szsharing.cn

================================================================================
来源：http://tz.jctech888.com.cn

[P01] 生成 UUID
来源：http://bj.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://gi.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mj.newstarts.cn

JS:   crypto.randomUUID()
来源：http://kx.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://nt.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://ji.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://ue.521024.cn

Ruby: SecureRandom.uuid
来源：http://ob.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://wy.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://dx.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bh.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ww.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ga.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cg.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yn.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://og.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gc.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tp.huanxung.cn

[P03] 生成短随机字符串
来源：http://bd.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ny.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tu.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sg.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ii.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eb.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cc.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kv.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ks.wgjwhj.cn

[P04] 求长度
来源：http://ie.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vn.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yf.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uk.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vm.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://nh.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://na.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://ev.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gx.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://qe.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fb.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sn.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://og.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nc.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kj.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ga.shxzskj.cn

Ruby: a == b
来源：http://zg.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yh.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gx.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jq.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://cl.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kk.chemitech.net.cn

TS:   if (x == null) {}
来源：http://mw.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mr.chemitech.net.cn

Go:   if x == nil {}
来源：http://vq.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hw.lnxyls.cn

C#:   if (x is null) {}
来源：http://wy.shxzukj.cn

[P07] 防抖与节流
来源：http://et.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xz.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://nt.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qt.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qt.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://te.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://st.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nh.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sh.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://eb.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uh.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ia.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yz.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vm.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eo.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qq.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wk.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jj.szsharing.cn

================================================================================
来源：http://so.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://od.521024.cn

================================================================================
来源：http://gs.bjjhwx.cn

[Q01] 创建表
来源：http://qt.yuexingan06.cn

CREATE TABLE users (
来源：http://bw.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lg.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://au.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://dy.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mg.shxzukj.cn

);
来源：http://yf.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://ft.bjjhwx.cn

CREATE TABLE orders (
来源：http://lg.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lc.haigaiapp.cn

user_id INT NOT NULL,
来源：http://io.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://ce.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uj.521024.cn

);
来源：http://qk.panjiajie.cn

[Q03] 增加列
来源：http://yf.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pn.nszjky.cn

[Q04] 修改列类型
来源：http://zg.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zg.nicolike.cn

[Q05] 重命名列
来源：http://du.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://va.hahajie.cn

[Q06] 删除列
来源：http://mi.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dt.jctech888.com.cn

[Q07] 删除表
来源：http://ki.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://dx.lnxyls.cn

[Q08] 创建普通索引
来源：http://zm.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rj.colortex.cn

[Q09] 创建唯一索引
来源：http://mz.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ro.shxzskj.cn

[Q10] 插入单行
来源：http://ld.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gy.muxihuayi.cn

[Q11] 一次插入多行
来源：http://ba.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xh.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://au.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vp.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lg.9csxet.cn

[Q13] 忽略重复插入
来源：http://ge.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://em.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://of.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oj.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pf.huanxung.cn

[Q15] 查询全部
来源：http://vn.yuexingan06.cn

SELECT * FROM users;
来源：http://zl.hahajie.cn

[Q16] 查询指定列
来源：http://sn.haigaiapp.cn

SELECT id, name FROM users;
来源：http://tt.521024.cn

[Q17] 条件查询
来源：http://wz.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://df.9csxet.cn

[Q18] 模糊匹配
来源：http://in.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vj.colortex.cn

[Q19] 范围查询
来源：http://fd.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mn.haigaiapp.cn

[Q20] IN 列表
来源：http://zi.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xt.colortex.cn

[Q21] 空值判断
来源：http://uf.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lt.gzmigu.cn

[Q22] 排序
来源：http://tn.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rf.wgjwhj.cn

[Q23] 分页
来源：http://za.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tg.nszjky.cn

[Q24] 去重
来源：http://hs.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://zu.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://yc.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vp.huanxung.cn

[Q26] 计数
来源：http://bi.521024.cn

SELECT COUNT(*) FROM users;
来源：http://co.chemitech.net.cn

[Q27] 条件计数
来源：http://cd.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gj.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://wk.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hl.9csxet.cn

[Q29] 最大最小值
来源：http://xv.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oc.yuntaijiaju.cn

[Q30] 分组统计
来源：http://am.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dg.521024.cn

[Q31] 分组后过滤
来源：http://hd.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ov.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://sp.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yr.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dl.gzmigu.cn

[Q33] 多列分组
来源：http://uu.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vb.shtwfgs.cn

[Q34] 每组取第一条
来源：http://qz.muxihuayi.cn

SELECT * FROM (
来源：http://gi.huanxung.cn


<!-- 参考信息 -->