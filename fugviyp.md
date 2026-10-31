代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ka.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ph.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://il.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ap.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ka.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cw.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ld.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rx.hahajie.cn

[N05] 最大公约数
来源：http://cl.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://zf.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wv.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qz.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ed.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ef.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jr.asd995.cn

Ruby: a.gcd(b)
来源：http://np.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://no.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://vr.bjjhwx.cn

Py:   s == s[::-1]
来源：http://pn.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://er.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://zt.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://fo.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yk.newstarts.cn

Go:   // 双指针从两端比较
来源：http://rw.szxytkj.cn

Ruby: s == s.reverse
来源：http://wz.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ne.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://te.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ub.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wq.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qo.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://tf.muxihuayi.cn

Java: // 手写 HashMap
来源：http://kx.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://yr.gzmigu.cn

Ruby: // 手写 Hash
来源：http://zi.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jv.huanxung.cn

[N08] 生成全排列
来源：http://nn.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://ji.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://yj.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ay.szsharing.cn

TS:   // 手写回溯递归
来源：http://lg.shxzskj.cn

Java: // 手写回溯递归
来源：http://en.shxzskj.cn

Go:   // 手写回溯递归
来源：http://mt.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://lx.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://xc.lnxyls.cn

[N09] 栈与队列
来源：http://ye.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://go.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wt.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zm.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://na.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://up.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ll.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rh.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wk.muxihuayi.cn

[N10] 链表节点定义
来源：http://de.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xl.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://su.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sk.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://op.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://nq.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ys.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vv.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qp.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://bp.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cq.szxytkj.cn

PHP:  // 手写递归函数
来源：http://uo.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wz.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vc.nszjky.cn

Java: // 手写递归
来源：http://vj.9csxet.cn

Go:   // 手写递归
来源：http://cf.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cq.shxzukj.cn

C#:   // 手写递归
来源：http://yh.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pm.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://na.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fw.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tg.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xw.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bq.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ax.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iv.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nv.gzmigu.cn

================================================================================
来源：http://lw.szsharing.cn

O. 并发与异步
来源：http://zo.wgjwhj.cn

================================================================================
来源：http://jm.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://ut.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qn.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://po.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://em.panjiajie.cn

TS:   // 同 JS
来源：http://vr.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://pk.shtwfgs.cn

Go:   go f()
来源：http://ta.hnjuh.cn

Ruby: Thread.new { f }
来源：http://up.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://ab.chemitech.net.cn

[O02] 使用线程池
来源：http://ut.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ta.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qo.colortex.cn

JS:   // worker_threads 线程池
来源：http://lz.newstarts.cn

TS:   // worker_threads 线程池
来源：http://gk.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ot.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dw.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ua.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ws.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://qu.newstarts.cn

Py:   with lock: shared += 1
来源：http://md.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ft.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ef.colortex.cn

TS:   // 同 JS
来源：http://ya.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://ll.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mz.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kh.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://zf.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://mi.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://wu.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mk.nicolike.cn

JS:   async function f() { await g(); }
来源：http://nd.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fc.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gg.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jv.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oj.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://eg.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://jt.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://ts.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rj.colortex.cn

JS:   await Promise.all(tasks)
来源：http://vf.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://lf.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://en.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://un.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://zq.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oc.jctech888.com.cn

[O06] 使用进程池
来源：http://sc.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ya.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://al.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://ao.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://pd.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pb.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eo.huanxung.cn

Ruby: // fork 块
来源：http://cf.huixinmuqiang.cn

C#:   Parallel.For
来源：http://tw.asd995.cn

================================================================================
来源：http://ad.shtwfgs.cn

P. 常用工具函数
来源：http://oz.jctech888.com.cn

================================================================================
来源：http://ja.huanxung.cn

[P01] 生成 UUID
来源：http://is.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://aj.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qa.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://eg.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://ww.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://zi.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://yt.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://jm.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://cf.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://hv.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fz.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ab.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qf.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mv.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cq.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vv.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nz.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tx.szxytkj.cn

[P03] 生成短随机字符串
来源：http://cm.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bn.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cb.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ux.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sm.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ox.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://at.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kz.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kf.521024.cn

[P04] 求长度
来源：http://hz.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kq.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vx.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tz.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zg.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://jv.szsharing.cn

Go:   len(arr);  len(m)
来源：http://uk.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://dm.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://st.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://tu.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sf.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lw.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://um.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ru.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fx.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vo.nszjky.cn

Ruby: a == b
来源：http://cf.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://so.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hj.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xm.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://jc.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zs.haigaiapp.cn

TS:   if (x == null) {}
来源：http://kd.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dl.hahajie.cn

Go:   if x == nil {}
来源：http://oq.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pe.haigaiapp.cn

C#:   if (x is null) {}
来源：http://cn.gzmigu.cn

[P07] 防抖与节流
来源：http://bo.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pj.521024.cn

PHP:  // 手写时间戳比较
来源：http://ps.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xv.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nc.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dg.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://la.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ih.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bg.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://kt.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cv.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ch.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kq.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jx.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vc.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jo.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bt.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://db.shxzukj.cn

================================================================================
来源：http://ji.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hg.shtwfgs.cn

================================================================================
来源：http://xa.jianghongdianzi.cn

[Q01] 创建表
来源：http://dh.haigaiapp.cn

CREATE TABLE users (
来源：http://rs.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eq.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://zr.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://ez.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yt.hahajie.cn

);
来源：http://lj.nicolike.cn

[Q02] 创建带外键的表
来源：http://ak.newstarts.cn

CREATE TABLE orders (
来源：http://lr.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bm.haigaiapp.cn

user_id INT NOT NULL,
来源：http://bb.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://kp.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wu.chemitech.net.cn

);
来源：http://uy.huanxung.cn

[Q03] 增加列
来源：http://my.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kz.huanxung.cn

[Q04] 修改列类型
来源：http://la.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://la.shtwfgs.cn

[Q05] 重命名列
来源：http://aq.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zn.haigaiapp.cn

[Q06] 删除列
来源：http://hb.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mt.521024.cn

[Q07] 删除表
来源：http://kb.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://az.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://el.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qt.panjiajie.cn

[Q09] 创建唯一索引
来源：http://lv.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xs.wgjwhj.cn

[Q10] 插入单行
来源：http://hv.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fj.huixiangedu.cn

[Q11] 一次插入多行
来源：http://qk.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pm.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://dz.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oe.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zn.szxytkj.cn

[Q13] 忽略重复插入
来源：http://aa.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xi.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://hz.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bv.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tr.huanxung.cn

[Q15] 查询全部
来源：http://ww.asd995.cn

SELECT * FROM users;
来源：http://cg.chemitech.net.cn

[Q16] 查询指定列
来源：http://qt.shxzukj.cn

SELECT id, name FROM users;
来源：http://fq.haigaiapp.cn

[Q17] 条件查询
来源：http://ov.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ri.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://sp.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ga.huixinmuqiang.cn

[Q19] 范围查询
来源：http://if.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qn.yuntaijiaju.cn

[Q20] IN 列表
来源：http://gf.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zo.wgjwhj.cn

[Q21] 空值判断
来源：http://py.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yt.szxytkj.cn

[Q22] 排序
来源：http://ww.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wu.shxzukj.cn

[Q23] 分页
来源：http://yv.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ez.nszjky.cn

[Q24] 去重
来源：http://ri.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://eo.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://hb.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oc.shtwfgs.cn

[Q26] 计数
来源：http://fa.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://fn.nicolike.cn

[Q27] 条件计数
来源：http://si.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tn.nicolike.cn

[Q28] 求和与平均
来源：http://ik.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ic.jctech888.com.cn

[Q29] 最大最小值
来源：http://wg.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xo.shtwfgs.cn

[Q30] 分组统计
来源：http://cb.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://av.huixiangedu.cn

[Q31] 分组后过滤
来源：http://if.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://br.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://zd.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://up.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gs.huixinmuqiang.cn

[Q33] 多列分组
来源：http://oj.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dt.chemitech.net.cn

[Q34] 每组取第一条
来源：http://tn.szsharing.cn

SELECT * FROM (
来源：http://my.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ip.muxihuayi.cn

) t WHERE rn = 1;
来源：http://pl.huixinmuqiang.cn

[Q35] 内连接
来源：http://oz.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oa.nszjky.cn


<!-- 参考信息 -->