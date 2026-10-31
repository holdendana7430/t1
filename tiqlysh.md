代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kn.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wf.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cy.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ur.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gz.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iw.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qg.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oc.gzmigu.cn

[N05] 最大公约数
来源：http://cq.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://ew.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bl.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fr.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://at.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jw.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ih.521024.cn

Ruby: a.gcd(b)
来源：http://dx.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sf.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://af.bjjhwx.cn

Py:   s == s[::-1]
来源：http://km.szsharing.cn

PHP:  $s === strrev($s);
来源：http://sd.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://wd.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://vh.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://co.9csxet.cn

Go:   // 双指针从两端比较
来源：http://gr.hnjuh.cn

Ruby: s == s.reverse
来源：http://kb.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pl.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://wi.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vs.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vp.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xn.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://my.newstarts.cn

Java: // 手写 HashMap
来源：http://vf.hahajie.cn

Go:   // 手写 map[int]int
来源：http://ag.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://uo.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wu.muxihuayi.cn

[N08] 生成全排列
来源：http://yq.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://lo.panjiajie.cn

PHP:  // 手写递归交换
来源：http://eg.panjiajie.cn

JS:   // 手写回溯递归
来源：http://kp.521024.cn

TS:   // 手写回溯递归
来源：http://ig.lnxyls.cn

Java: // 手写回溯递归
来源：http://tu.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://jx.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://em.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://qj.asd995.cn

[N09] 栈与队列
来源：http://tp.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lc.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ko.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bt.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://al.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zc.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fb.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://so.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://te.521024.cn

[N10] 链表节点定义
来源：http://nb.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xj.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://id.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nd.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fx.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://uj.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ie.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kl.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tu.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://vc.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qs.szsharing.cn

PHP:  // 手写递归函数
来源：http://pf.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oh.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pt.szsharing.cn

Java: // 手写递归
来源：http://ws.shxzukj.cn

Go:   // 手写递归
来源：http://aj.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mo.bjjhwx.cn

C#:   // 手写递归
来源：http://mo.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ck.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sw.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zm.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nf.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uo.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fu.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mv.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yc.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nv.shxzukj.cn

================================================================================
来源：http://qt.bookmarksfly.cn

O. 并发与异步
来源：http://zm.muxihuayi.cn

================================================================================
来源：http://ku.huixiangedu.cn

[O01] 启动一个线程
来源：http://vv.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jb.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ew.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pq.huixiangedu.cn

TS:   // 同 JS
来源：http://lk.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://sl.panjiajie.cn

Go:   go f()
来源：http://gn.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://vu.hahajie.cn

C#:   Task.Run(() => F());
来源：http://am.shxzukj.cn

[O02] 使用线程池
来源：http://as.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cm.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nj.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://nk.9csxet.cn

TS:   // worker_threads 线程池
来源：http://xl.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bz.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xl.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dl.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oo.nszjky.cn

[O03] 加锁保护共享数据
来源：http://tx.szsharing.cn

Py:   with lock: shared += 1
来源：http://ae.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://du.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ty.hahajie.cn

TS:   // 同 JS
来源：http://rs.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://tp.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pt.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://af.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://rn.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://wq.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://sv.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ws.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://od.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mo.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eh.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uy.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ko.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://uf.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://gx.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://fh.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qg.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://lv.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://zl.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ed.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ln.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://hz.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vz.huixinmuqiang.cn

[O06] 使用进程池
来源：http://zg.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nc.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ey.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://qu.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://nn.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xt.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pc.9csxet.cn

Ruby: // fork 块
来源：http://io.nszjky.cn

C#:   Parallel.For
来源：http://ua.521024.cn

================================================================================
来源：http://ua.jctech888.com.cn

P. 常用工具函数
来源：http://tr.lnxyls.cn

================================================================================
来源：http://ot.szsharing.cn

[P01] 生成 UUID
来源：http://gp.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://tp.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sw.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://tn.colortex.cn

TS:   crypto.randomUUID()
来源：http://hl.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://gz.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://cz.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://rj.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://sd.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ff.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yp.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bh.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vd.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jb.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hh.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bp.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rx.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ke.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://cu.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ny.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rg.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pj.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ru.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rf.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ko.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vl.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zo.huixinmuqiang.cn

[P04] 求长度
来源：http://aw.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://we.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://po.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fl.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://er.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://ey.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://vk.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://du.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dw.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://gi.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ot.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gm.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hc.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vk.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tm.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zf.haigaiapp.cn

Ruby: a == b
来源：http://cz.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://li.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tu.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dz.colortex.cn

PHP:  if (empty($x)) {}
来源：http://uv.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lr.bjjhwx.cn

TS:   if (x == null) {}
来源：http://yu.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ce.szxytkj.cn

Go:   if x == nil {}
来源：http://zp.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fi.szxytkj.cn

C#:   if (x is null) {}
来源：http://ui.shxzskj.cn

[P07] 防抖与节流
来源：http://ik.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kj.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://vp.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ar.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ez.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wv.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kc.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dr.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wl.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://sq.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eo.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iz.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fn.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mt.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hf.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kf.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dx.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ib.szsharing.cn

================================================================================
来源：http://xz.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pn.panjiajie.cn

================================================================================
来源：http://bo.shxzskj.cn

[Q01] 创建表
来源：http://ix.szxytkj.cn

CREATE TABLE users (
来源：http://zh.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yk.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://sx.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ta.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://so.muxihuayi.cn

);
来源：http://hf.colortex.cn

[Q02] 创建带外键的表
来源：http://wm.shtwfgs.cn

CREATE TABLE orders (
来源：http://dj.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hh.szsharing.cn

user_id INT NOT NULL,
来源：http://ka.newstarts.cn

amount DECIMAL(10, 2),
来源：http://fz.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rr.nicolike.cn

);
来源：http://qx.szsharing.cn

[Q03] 增加列
来源：http://vu.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://se.huixiangedu.cn

[Q04] 修改列类型
来源：http://cx.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ho.9csxet.cn

[Q05] 重命名列
来源：http://rh.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ck.bjjhwx.cn

[Q06] 删除列
来源：http://dk.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cn.szsharing.cn

[Q07] 删除表
来源：http://ge.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://bt.521024.cn

[Q08] 创建普通索引
来源：http://nf.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wa.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://mn.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qe.szxytkj.cn

[Q10] 插入单行
来源：http://va.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ii.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://tz.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pe.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://lb.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yc.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tc.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://is.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hx.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://kg.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qa.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yl.bjjhwx.cn

[Q15] 查询全部
来源：http://ql.szxytkj.cn

SELECT * FROM users;
来源：http://es.yuexingan06.cn

[Q16] 查询指定列
来源：http://jv.nszjky.cn

SELECT id, name FROM users;
来源：http://ch.chemitech.net.cn

[Q17] 条件查询
来源：http://hg.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fw.lnxyls.cn

[Q18] 模糊匹配
来源：http://sa.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eq.muxihuayi.cn

[Q19] 范围查询
来源：http://kv.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mh.bjjhwx.cn

[Q20] IN 列表
来源：http://wl.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vq.9csxet.cn

[Q21] 空值判断
来源：http://el.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ak.nicolike.cn

[Q22] 排序
来源：http://gi.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://la.huixinmuqiang.cn

[Q23] 分页
来源：http://yv.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lk.bookmarksfly.cn

[Q24] 去重
来源：http://vz.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://yr.9csxet.cn

[Q25] 只取前 N 条
来源：http://xb.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qa.colortex.cn

[Q26] 计数
来源：http://eh.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://xh.colortex.cn

[Q27] 条件计数
来源：http://ci.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ss.jctech888.com.cn

[Q28] 求和与平均
来源：http://wb.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oh.szxytkj.cn

[Q29] 最大最小值
来源：http://ug.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://th.asd995.cn

[Q30] 分组统计
来源：http://ri.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://li.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://vq.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zu.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://ct.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eu.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fu.gzmigu.cn

[Q33] 多列分组
来源：http://jj.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ip.colortex.cn

[Q34] 每组取第一条
来源：http://wk.nicolike.cn

SELECT * FROM (
来源：http://bh.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bv.jctech888.com.cn

) t WHERE rn = 1;
来源：http://hp.jctech888.com.cn

[Q35] 内连接
来源：http://nl.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.bookmarksfly.cn


<!-- 参考信息 -->