代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://km.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kh.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ua.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tx.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ta.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://et.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ll.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ig.hnjuh.cn

[N05] 最大公约数
来源：http://zg.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://qu.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xw.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ng.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hr.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oq.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ut.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://nq.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qm.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://ed.lnxyls.cn

Py:   s == s[::-1]
来源：http://bl.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://kh.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://zf.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://sd.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mw.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://lt.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://kw.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zk.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://cw.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bu.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lt.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wa.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://vz.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://uj.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://bs.huanxung.cn

Ruby: // 手写 Hash
来源：http://xy.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qd.newstarts.cn

[N08] 生成全排列
来源：http://iw.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://pi.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://jw.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://dd.9csxet.cn

TS:   // 手写回溯递归
来源：http://uy.szsharing.cn

Java: // 手写回溯递归
来源：http://wr.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://rg.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://oj.szxytkj.cn

C#:   // 手写回溯递归
来源：http://re.nicolike.cn

[N09] 栈与队列
来源：http://ig.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oj.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oe.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tb.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gs.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pa.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kp.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ef.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jj.chemitech.net.cn

[N10] 链表节点定义
来源：http://xn.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tu.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sq.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://og.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fk.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://ra.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://az.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dv.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://os.nszjky.cn

[N11] 二叉树中序遍历
来源：http://fk.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wf.szsharing.cn

PHP:  // 手写递归函数
来源：http://fp.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sb.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ej.nszjky.cn

Java: // 手写递归
来源：http://gj.shtwfgs.cn

Go:   // 手写递归
来源：http://ub.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mo.521024.cn

C#:   // 手写递归
来源：http://yy.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nv.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://it.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mn.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kl.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vs.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ke.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rh.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mh.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fh.colortex.cn

================================================================================
来源：http://mf.szsharing.cn

O. 并发与异步
来源：http://pq.shxzukj.cn

================================================================================
来源：http://ho.bjjhwx.cn

[O01] 启动一个线程
来源：http://ip.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ch.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bc.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fu.521024.cn

TS:   // 同 JS
来源：http://yd.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://kf.521024.cn

Go:   go f()
来源：http://rd.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://bs.nicolike.cn

C#:   Task.Run(() => F());
来源：http://ad.wgjwhj.cn

[O02] 使用线程池
来源：http://rh.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pa.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pa.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://pp.nicolike.cn

TS:   // worker_threads 线程池
来源：http://sf.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kl.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://og.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ci.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qp.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://di.asd995.cn

Py:   with lock: shared += 1
来源：http://cc.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://yj.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vs.jianghongdianzi.cn

TS:   // 同 JS
来源：http://vz.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://cc.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xj.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cq.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://kq.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://te.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://gg.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://no.colortex.cn

JS:   async function f() { await g(); }
来源：http://ta.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://st.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://be.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zr.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ka.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://lj.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://kb.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://bb.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://my.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://rz.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://db.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yz.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://un.hahajie.cn

Ruby: threads.map(&:join)
来源：http://mb.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bd.lnxyls.cn

[O06] 使用进程池
来源：http://xe.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://af.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ro.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://ru.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://mt.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nk.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rb.asd995.cn

Ruby: // fork 块
来源：http://mm.muxihuayi.cn

C#:   Parallel.For
来源：http://lj.panjiajie.cn

================================================================================
来源：http://bz.wgjwhj.cn

P. 常用工具函数
来源：http://bn.newstarts.cn

================================================================================
来源：http://ef.asd995.cn

[P01] 生成 UUID
来源：http://eh.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://kr.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oy.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://eq.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://co.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://ax.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://je.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://hl.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://if.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://hh.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ia.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gy.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kd.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ib.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nc.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sr.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iq.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yv.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://yp.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cw.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fm.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aj.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oo.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xs.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pu.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://om.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wd.jianghongdianzi.cn

[P04] 求长度
来源：http://jf.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hf.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tm.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wg.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jx.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://gb.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://yy.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://sa.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vt.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://wf.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eq.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zg.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cx.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dt.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://he.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xu.wgjwhj.cn

Ruby: a == b
来源：http://ub.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fd.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zm.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jo.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://qd.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hw.yuexingan06.cn

TS:   if (x == null) {}
来源：http://cx.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uj.szsharing.cn

Go:   if x == nil {}
来源：http://gc.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xt.nicolike.cn

C#:   if (x is null) {}
来源：http://us.newstarts.cn

[P07] 防抖与节流
来源：http://qc.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lc.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://em.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fr.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pv.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rq.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uo.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://un.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://kd.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dl.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wt.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://py.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://db.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bf.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fq.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qj.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ma.jctech888.com.cn

================================================================================
来源：http://gb.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oo.521024.cn

================================================================================
来源：http://mc.szxytkj.cn

[Q01] 创建表
来源：http://rb.muxihuayi.cn

CREATE TABLE users (
来源：http://ik.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ge.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://yy.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://ks.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wl.yuntaijiaju.cn

);
来源：http://uz.panjiajie.cn

[Q02] 创建带外键的表
来源：http://vd.huanxung.cn

CREATE TABLE orders (
来源：http://oo.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uv.shxzskj.cn

user_id INT NOT NULL,
来源：http://qt.colortex.cn

amount DECIMAL(10, 2),
来源：http://sa.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qh.shxzskj.cn

);
来源：http://gi.huanxung.cn

[Q03] 增加列
来源：http://gz.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iq.521024.cn

[Q04] 修改列类型
来源：http://al.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gl.jctech888.com.cn

[Q05] 重命名列
来源：http://if.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gp.shxzskj.cn

[Q06] 删除列
来源：http://ps.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://de.nszjky.cn

[Q07] 删除表
来源：http://bs.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://jb.shxzukj.cn

[Q08] 创建普通索引
来源：http://ip.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rb.hahajie.cn

[Q09] 创建唯一索引
来源：http://qk.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nt.9csxet.cn

[Q10] 插入单行
来源：http://sa.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sk.szxytkj.cn

[Q11] 一次插入多行
来源：http://cz.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ei.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://nn.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ck.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ge.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://ye.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jp.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://sg.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eo.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ck.shtwfgs.cn

[Q15] 查询全部
来源：http://jh.bjjhwx.cn

SELECT * FROM users;
来源：http://ym.nszjky.cn

[Q16] 查询指定列
来源：http://qz.nicolike.cn

SELECT id, name FROM users;
来源：http://kp.szxytkj.cn

[Q17] 条件查询
来源：http://yk.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hx.chemitech.net.cn

[Q18] 模糊匹配
来源：http://by.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tw.bookmarksfly.cn

[Q19] 范围查询
来源：http://lf.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hf.shxzskj.cn

[Q20] IN 列表
来源：http://lz.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ne.szsharing.cn

[Q21] 空值判断
来源：http://mn.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://en.shxzskj.cn

[Q22] 排序
来源：http://cz.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rg.lnxyls.cn

[Q23] 分页
来源：http://ep.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ia.panjiajie.cn

[Q24] 去重
来源：http://vo.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://xd.nszjky.cn

[Q25] 只取前 N 条
来源：http://ek.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vk.bookmarksfly.cn

[Q26] 计数
来源：http://nc.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://yf.huanxung.cn

[Q27] 条件计数
来源：http://zg.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hq.huixiangedu.cn

[Q28] 求和与平均
来源：http://qr.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vt.nicolike.cn

[Q29] 最大最小值
来源：http://km.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wl.huanxung.cn

[Q30] 分组统计
来源：http://gg.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dw.nicolike.cn

[Q31] 分组后过滤
来源：http://fj.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kr.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://qc.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uj.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qk.521024.cn

[Q33] 多列分组
来源：http://lm.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ub.wgjwhj.cn

[Q34] 每组取第一条
来源：http://rv.asd995.cn

SELECT * FROM (
来源：http://ra.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nw.hnjuh.cn

) t WHERE rn = 1;
来源：http://zk.jianghongdianzi.cn

[Q35] 内连接
来源：http://ml.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vs.huanxung.cn


<!-- 参考信息 -->