代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rc.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qf.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rt.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oh.nicolike.cn

[N05] 最大公约数
来源：http://qu.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://mu.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://or.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xe.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qb.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nm.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nf.521024.cn

Ruby: a.gcd(b)
来源：http://ea.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eg.hahajie.cn

[N06] 判断回文字符串
来源：http://ej.hahajie.cn

Py:   s == s[::-1]
来源：http://kv.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://cb.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://vv.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://wn.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ku.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://cg.shtwfgs.cn

Ruby: s == s.reverse
来源：http://nw.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xv.asd995.cn

[N07] 两数之和（返回下标）
来源：http://vj.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ih.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pw.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zq.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://rn.chemitech.net.cn

Java: // 手写 HashMap
来源：http://sw.newstarts.cn

Go:   // 手写 map[int]int
来源：http://cn.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://iu.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sl.huixinmuqiang.cn

[N08] 生成全排列
来源：http://iv.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://bt.hnjuh.cn

PHP:  // 手写递归交换
来源：http://xb.newstarts.cn

JS:   // 手写回溯递归
来源：http://am.newstarts.cn

TS:   // 手写回溯递归
来源：http://gu.nicolike.cn

Java: // 手写回溯递归
来源：http://sq.panjiajie.cn

Go:   // 手写回溯递归
来源：http://ym.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://if.nicolike.cn

C#:   // 手写回溯递归
来源：http://rl.szsharing.cn

[N09] 栈与队列
来源：http://md.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qb.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pi.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sm.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kw.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vy.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ua.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qs.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://de.9csxet.cn

[N10] 链表节点定义
来源：http://yw.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ez.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fd.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xj.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eb.521024.cn

Java: class Node { int v; Node next; }
来源：http://qo.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kg.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eh.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lv.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://dm.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zs.shxzukj.cn

PHP:  // 手写递归函数
来源：http://ol.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jm.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sx.521024.cn

Java: // 手写递归
来源：http://la.shtwfgs.cn

Go:   // 手写递归
来源：http://wu.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vw.huixiangedu.cn

C#:   // 手写递归
来源：http://th.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nt.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wy.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nq.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://el.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qp.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nz.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jn.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yb.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oe.jianghongdianzi.cn

================================================================================
来源：http://if.newstarts.cn

O. 并发与异步
来源：http://zo.9csxet.cn

================================================================================
来源：http://zi.nszjky.cn

[O01] 启动一个线程
来源：http://xg.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nu.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lv.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://as.colortex.cn

TS:   // 同 JS
来源：http://zg.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://vl.haigaiapp.cn

Go:   go f()
来源：http://hr.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://wi.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://se.jianghongdianzi.cn

[O02] 使用线程池
来源：http://ec.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fr.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rz.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://br.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://je.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kb.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yn.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ay.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ap.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://er.hahajie.cn

Py:   with lock: shared += 1
来源：http://re.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://le.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wo.colortex.cn

TS:   // 同 JS
来源：http://im.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://lf.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bq.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lv.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://xu.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://ra.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://hl.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ge.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://zx.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://si.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wl.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ni.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lx.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://oj.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://yq.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://mu.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ut.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://kh.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://pf.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ui.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cq.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://xo.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xh.asd995.cn

[O06] 使用进程池
来源：http://ky.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xq.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wd.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://nv.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://dk.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hy.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ka.colortex.cn

Ruby: // fork 块
来源：http://ix.huixinmuqiang.cn

C#:   Parallel.For
来源：http://qj.colortex.cn

================================================================================
来源：http://qq.hnjuh.cn

P. 常用工具函数
来源：http://nt.huixiangedu.cn

================================================================================
来源：http://xg.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://ja.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://ex.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gw.asd995.cn

JS:   crypto.randomUUID()
来源：http://xs.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://qe.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://ms.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://bc.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://se.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://nj.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://sk.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fl.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://si.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sh.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oe.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ka.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ft.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yx.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ob.huanxung.cn

[P03] 生成短随机字符串
来源：http://zs.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uc.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wu.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fl.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qw.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nw.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oe.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sk.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wh.huixiangedu.cn

[P04] 求长度
来源：http://sj.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vd.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bc.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ng.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sm.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://xo.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://ov.hahajie.cn

Ruby: x.length;  x.size
来源：http://rp.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wz.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://jj.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hr.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nx.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qc.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bv.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ox.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uk.shxzskj.cn

Ruby: a == b
来源：http://ny.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sy.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ul.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zz.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://ol.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ab.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://of.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ba.szxytkj.cn

Go:   if x == nil {}
来源：http://ra.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://of.chemitech.net.cn

C#:   if (x is null) {}
来源：http://wd.lnxyls.cn

[P07] 防抖与节流
来源：http://jk.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vs.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://xg.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nh.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qw.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zo.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dx.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bt.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://md.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://fk.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vj.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xx.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mt.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qt.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rx.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ip.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uz.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xs.shtwfgs.cn

================================================================================
来源：http://cd.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ze.huanxung.cn

================================================================================
来源：http://rr.newstarts.cn

[Q01] 创建表
来源：http://vn.jianghongdianzi.cn

CREATE TABLE users (
来源：http://sw.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://od.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://yn.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://zn.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://no.huanxung.cn

);
来源：http://gs.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://ob.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://ni.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ge.szxytkj.cn

user_id INT NOT NULL,
来源：http://gq.nszjky.cn

amount DECIMAL(10, 2),
来源：http://fw.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wf.nicolike.cn

);
来源：http://rz.9csxet.cn

[Q03] 增加列
来源：http://jy.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://od.nszjky.cn

[Q04] 修改列类型
来源：http://cd.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fg.gzmigu.cn

[Q05] 重命名列
来源：http://ie.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xe.colortex.cn

[Q06] 删除列
来源：http://ek.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://il.szxytkj.cn

[Q07] 删除表
来源：http://mg.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://pv.colortex.cn

[Q08] 创建普通索引
来源：http://yv.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://za.nicolike.cn

[Q09] 创建唯一索引
来源：http://id.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ni.asd995.cn

[Q10] 插入单行
来源：http://ym.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dr.nicolike.cn

[Q11] 一次插入多行
来源：http://th.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ih.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://he.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pu.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hg.9csxet.cn

[Q13] 忽略重复插入
来源：http://we.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fv.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://si.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hd.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dz.muxihuayi.cn

[Q15] 查询全部
来源：http://al.huixinmuqiang.cn

SELECT * FROM users;
来源：http://hg.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://gf.jctech888.com.cn

SELECT id, name FROM users;
来源：http://fp.521024.cn

[Q17] 条件查询
来源：http://jb.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pu.shxzskj.cn

[Q18] 模糊匹配
来源：http://ey.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ll.bookmarksfly.cn

[Q19] 范围查询
来源：http://yr.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tw.jianghongdianzi.cn

[Q20] IN 列表
来源：http://jb.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vn.shxzukj.cn

[Q21] 空值判断
来源：http://wf.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ud.hahajie.cn

[Q22] 排序
来源：http://tg.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nc.nszjky.cn

[Q23] 分页
来源：http://iv.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wm.shxzukj.cn

[Q24] 去重
来源：http://vm.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://hl.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://kg.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ap.haigaiapp.cn

[Q26] 计数
来源：http://ai.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://ys.huixinmuqiang.cn

[Q27] 条件计数
来源：http://pq.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kr.newstarts.cn

[Q28] 求和与平均
来源：http://ro.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iv.colortex.cn

[Q29] 最大最小值
来源：http://nw.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qh.nszjky.cn

[Q30] 分组统计
来源：http://sz.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nu.shxzskj.cn

[Q31] 分组后过滤
来源：http://fw.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yo.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://my.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vs.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ar.521024.cn

[Q33] 多列分组
来源：http://ne.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xe.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://ks.muxihuayi.cn

SELECT * FROM (
来源：http://tq.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yv.huixiangedu.cn

) t WHERE rn = 1;
来源：http://ox.shtwfgs.cn

[Q35] 内连接
来源：http://ht.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tn.yuntaijiaju.cn

[Q36] 左连接
来源：http://px.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ia.panjiajie.cn

[Q37] 右连接
来源：http://yu.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kf.wgjwhj.cn


<!-- 参考信息 -->