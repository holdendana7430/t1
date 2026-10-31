代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yx.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rc.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tq.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ya.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gk.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vo.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kk.yuntaijiaju.cn

[N05] 最大公约数
来源：http://nc.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://gc.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zz.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yt.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aj.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mi.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jt.hnjuh.cn

Ruby: a.gcd(b)
来源：http://ip.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uj.hahajie.cn

[N06] 判断回文字符串
来源：http://et.bjjhwx.cn

Py:   s == s[::-1]
来源：http://fz.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://qz.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://kx.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://jz.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bn.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://wr.521024.cn

Ruby: s == s.reverse
来源：http://we.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://am.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://lt.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xg.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://su.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ry.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://tn.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://ek.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://qd.newstarts.cn

Ruby: // 手写 Hash
来源：http://vr.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hs.chemitech.net.cn

[N08] 生成全排列
来源：http://ix.colortex.cn

Py:   itertools.permutations(arr)
来源：http://kf.szxytkj.cn

PHP:  // 手写递归交换
来源：http://vx.szsharing.cn

JS:   // 手写回溯递归
来源：http://pg.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://ok.chemitech.net.cn

Java: // 手写回溯递归
来源：http://pp.colortex.cn

Go:   // 手写回溯递归
来源：http://xy.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://qs.shxzskj.cn

C#:   // 手写回溯递归
来源：http://gg.521024.cn

[N09] 栈与队列
来源：http://fr.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vk.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jb.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lh.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ui.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nt.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fc.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gm.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gg.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://ha.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jc.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mk.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vf.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wl.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://qi.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fy.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zm.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qi.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://it.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tu.panjiajie.cn

PHP:  // 手写递归函数
来源：http://nv.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aj.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wu.521024.cn

Java: // 手写递归
来源：http://vr.newstarts.cn

Go:   // 手写递归
来源：http://nw.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ea.shxzskj.cn

C#:   // 手写递归
来源：http://sn.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kl.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sj.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ej.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cb.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lq.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rc.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://un.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jx.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zi.szsharing.cn

================================================================================
来源：http://hz.newstarts.cn

O. 并发与异步
来源：http://qq.asd995.cn

================================================================================
来源：http://tu.szsharing.cn

[O01] 启动一个线程
来源：http://al.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tw.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vp.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bi.nszjky.cn

TS:   // 同 JS
来源：http://py.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://pq.nicolike.cn

Go:   go f()
来源：http://ht.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://rx.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://cm.haigaiapp.cn

[O02] 使用线程池
来源：http://ow.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lr.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ks.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://oo.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://yq.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lp.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lw.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yf.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jx.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://bi.szsharing.cn

Py:   with lock: shared += 1
来源：http://gi.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://fr.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cb.colortex.cn

TS:   // 同 JS
来源：http://pj.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://hw.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nq.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qe.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://dr.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://jk.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://wl.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yx.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://be.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bs.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ax.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wp.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kr.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://ld.521024.cn

[O05] 并发执行并等待全部完成
来源：http://um.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://dh.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hm.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://ye.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://in.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tj.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iz.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://nh.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ao.nicolike.cn

[O06] 使用进程池
来源：http://us.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wh.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wx.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://mx.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://qn.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jn.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bo.chemitech.net.cn

Ruby: // fork 块
来源：http://io.huixinmuqiang.cn

C#:   Parallel.For
来源：http://bs.huixiangedu.cn

================================================================================
来源：http://nt.lnxyls.cn

P. 常用工具函数
来源：http://wa.colortex.cn

================================================================================
来源：http://ef.panjiajie.cn

[P01] 生成 UUID
来源：http://iy.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://xu.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pg.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://xb.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://oq.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://of.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://yx.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://nl.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://ct.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://iw.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bz.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zg.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jn.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ko.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sw.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xj.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oy.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fe.hahajie.cn

[P03] 生成短随机字符串
来源：http://gc.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://os.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iw.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://go.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ak.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bk.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pt.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ca.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://og.yuexingan06.cn

[P04] 求长度
来源：http://zd.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zp.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pa.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ne.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yl.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://ng.huanxung.cn

Go:   len(arr);  len(m)
来源：http://rc.huanxung.cn

Ruby: x.length;  x.size
来源：http://ek.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://on.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://vc.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vy.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qf.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ki.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ww.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xk.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fx.nicolike.cn

Ruby: a == b
来源：http://iz.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://py.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nl.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rg.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://hl.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ah.gzmigu.cn

TS:   if (x == null) {}
来源：http://si.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pi.bjjhwx.cn

Go:   if x == nil {}
来源：http://ly.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iu.shxzskj.cn

C#:   if (x is null) {}
来源：http://xo.asd995.cn

[P07] 防抖与节流
来源：http://af.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bn.asd995.cn

PHP:  // 手写时间戳比较
来源：http://gq.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qs.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zp.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ry.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mx.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mc.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://af.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://wt.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dl.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uy.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uy.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nd.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tu.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ks.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kk.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nv.asd995.cn

================================================================================
来源：http://ft.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://di.nszjky.cn

================================================================================
来源：http://tq.yuntaijiaju.cn

[Q01] 创建表
来源：http://vh.lnxyls.cn

CREATE TABLE users (
来源：http://kr.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ix.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://mr.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://fp.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ly.jianghongdianzi.cn

);
来源：http://gq.szxytkj.cn

[Q02] 创建带外键的表
来源：http://wv.wgjwhj.cn

CREATE TABLE orders (
来源：http://or.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pj.szxytkj.cn

user_id INT NOT NULL,
来源：http://ou.szsharing.cn

amount DECIMAL(10, 2),
来源：http://ru.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uq.szsharing.cn

);
来源：http://mi.asd995.cn

[Q03] 增加列
来源：http://qb.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tc.yuexingan06.cn

[Q04] 修改列类型
来源：http://xs.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cm.nszjky.cn

[Q05] 重命名列
来源：http://va.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jt.gzmigu.cn

[Q06] 删除列
来源：http://cn.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dk.hnjuh.cn

[Q07] 删除表
来源：http://xo.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://ck.colortex.cn

[Q08] 创建普通索引
来源：http://ga.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://np.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://me.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ol.asd995.cn

[Q10] 插入单行
来源：http://yf.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gv.yuexingan06.cn

[Q11] 一次插入多行
来源：http://tg.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ug.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://wj.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cq.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dd.hnjuh.cn

[Q13] 忽略重复插入
来源：http://cn.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cy.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://nh.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://od.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oy.haigaiapp.cn

[Q15] 查询全部
来源：http://ki.szxytkj.cn

SELECT * FROM users;
来源：http://qr.hnjuh.cn

[Q16] 查询指定列
来源：http://gs.colortex.cn

SELECT id, name FROM users;
来源：http://li.bjjhwx.cn

[Q17] 条件查询
来源：http://ds.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://az.szxytkj.cn

[Q18] 模糊匹配
来源：http://ed.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ig.hahajie.cn

[Q19] 范围查询
来源：http://ys.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hk.gzmigu.cn

[Q20] IN 列表
来源：http://dx.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xn.shxzskj.cn

[Q21] 空值判断
来源：http://lt.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dj.chemitech.net.cn

[Q22] 排序
来源：http://ja.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ty.huanxung.cn

[Q23] 分页
来源：http://bc.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shxzskj.cn

[Q24] 去重
来源：http://yo.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://cg.panjiajie.cn

[Q25] 只取前 N 条
来源：http://er.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lg.shxzskj.cn

[Q26] 计数
来源：http://dg.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://qd.huixinmuqiang.cn

[Q27] 条件计数
来源：http://vq.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://us.newstarts.cn

[Q28] 求和与平均
来源：http://kt.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ey.bjjhwx.cn

[Q29] 最大最小值
来源：http://co.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yz.jianghongdianzi.cn

[Q30] 分组统计
来源：http://dk.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zt.wgjwhj.cn

[Q31] 分组后过滤
来源：http://sm.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rj.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://wo.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ej.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ce.hnjuh.cn

[Q33] 多列分组
来源：http://ch.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://er.shtwfgs.cn

[Q34] 每组取第一条
来源：http://fl.lnxyls.cn

SELECT * FROM (
来源：http://ww.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eu.gzmigu.cn

) t WHERE rn = 1;
来源：http://ql.hnjuh.cn

[Q35] 内连接
来源：http://yi.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vo.9csxet.cn


<!-- 参考信息 -->