代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dd.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xi.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mm.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ri.yuntaijiaju.cn

[N05] 最大公约数
来源：http://bq.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://wc.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kh.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://po.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ch.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sd.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://af.gzmigu.cn

Ruby: a.gcd(b)
来源：http://mw.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lf.chemitech.net.cn

[N06] 判断回文字符串
来源：http://ev.szxytkj.cn

Py:   s == s[::-1]
来源：http://tn.szsharing.cn

PHP:  $s === strrev($s);
来源：http://xx.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://ki.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://sj.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jh.szsharing.cn

Go:   // 双指针从两端比较
来源：http://vw.asd995.cn

Ruby: s == s.reverse
来源：http://zq.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ms.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://bs.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ns.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ph.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sj.521024.cn

TS:   // 手写 Map<string, number>
来源：http://cb.szxytkj.cn

Java: // 手写 HashMap
来源：http://sk.colortex.cn

Go:   // 手写 map[int]int
来源：http://ow.huanxung.cn

Ruby: // 手写 Hash
来源：http://bk.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://db.shtwfgs.cn

[N08] 生成全排列
来源：http://mv.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://uc.shxzskj.cn

PHP:  // 手写递归交换
来源：http://kv.9csxet.cn

JS:   // 手写回溯递归
来源：http://dm.hnjuh.cn

TS:   // 手写回溯递归
来源：http://be.wgjwhj.cn

Java: // 手写回溯递归
来源：http://wf.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://hq.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://qx.9csxet.cn

C#:   // 手写回溯递归
来源：http://tt.wgjwhj.cn

[N09] 栈与队列
来源：http://uf.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ia.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cc.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://me.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://je.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hj.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yf.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xh.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sp.gzmigu.cn

[N10] 链表节点定义
来源：http://my.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nh.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jz.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jo.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hq.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://an.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://co.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yy.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qd.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://jj.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gm.hnjuh.cn

PHP:  // 手写递归函数
来源：http://qy.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gj.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xo.yuexingan06.cn

Java: // 手写递归
来源：http://il.huixiangedu.cn

Go:   // 手写递归
来源：http://hy.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vj.colortex.cn

C#:   // 手写递归
来源：http://mo.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bq.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ja.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://da.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xx.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yx.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lk.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ui.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uk.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qj.chemitech.net.cn

================================================================================
来源：http://se.shxzukj.cn

O. 并发与异步
来源：http://zv.bookmarksfly.cn

================================================================================
来源：http://hj.chemitech.net.cn

[O01] 启动一个线程
来源：http://xo.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jc.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xb.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lc.bjjhwx.cn

TS:   // 同 JS
来源：http://xg.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://fl.shtwfgs.cn

Go:   go f()
来源：http://py.gzmigu.cn

Ruby: Thread.new { f }
来源：http://fv.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://uh.yuexingan06.cn

[O02] 使用线程池
来源：http://ej.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qn.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yr.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://ns.huanxung.cn

TS:   // worker_threads 线程池
来源：http://yq.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yl.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bu.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mu.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xj.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://ih.asd995.cn

Py:   with lock: shared += 1
来源：http://lb.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ca.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wt.gzmigu.cn

TS:   // 同 JS
来源：http://kl.521024.cn

Java: synchronized (this) { shared++; }
来源：http://zu.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vw.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hw.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://uw.colortex.cn

[O04] 定义异步函数并等待
来源：http://sv.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://kx.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xl.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://bd.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xv.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://za.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ea.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jd.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://kt.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://vs.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://td.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hc.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://zz.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://cn.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pf.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mu.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://fr.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hd.asd995.cn

[O06] 使用进程池
来源：http://bw.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bq.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ym.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://fb.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://im.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ow.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xs.shxzskj.cn

Ruby: // fork 块
来源：http://zx.hnjuh.cn

C#:   Parallel.For
来源：http://wc.hnjuh.cn

================================================================================
来源：http://cf.huixinmuqiang.cn

P. 常用工具函数
来源：http://gt.szsharing.cn

================================================================================
来源：http://sx.shxzskj.cn

[P01] 生成 UUID
来源：http://wj.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://rp.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tj.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://hq.hahajie.cn

TS:   crypto.randomUUID()
来源：http://rd.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://xp.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://jd.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://ji.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://zz.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://pj.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wb.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nq.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ug.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zz.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gr.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ds.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vz.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ct.newstarts.cn

[P03] 生成短随机字符串
来源：http://ca.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bw.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wb.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hh.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://we.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bl.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vt.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dz.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ch.yuexingan06.cn

[P04] 求长度
来源：http://ln.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yx.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ew.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eh.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bv.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://rj.nicolike.cn

Go:   len(arr);  len(m)
来源：http://kl.nicolike.cn

Ruby: x.length;  x.size
来源：http://sh.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qi.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://nn.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://od.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bt.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://te.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dt.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vn.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tp.521024.cn

Ruby: a == b
来源：http://ky.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ob.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ya.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://la.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://lq.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fa.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://mv.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mq.panjiajie.cn

Go:   if x == nil {}
来源：http://ff.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lk.chemitech.net.cn

C#:   if (x is null) {}
来源：http://tq.shtwfgs.cn

[P07] 防抖与节流
来源：http://ko.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yt.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://fp.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://or.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uk.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lh.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pq.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ok.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hb.newstarts.cn

[P08] 处理浮点精度问题
来源：http://fn.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ir.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oc.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ua.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://is.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cg.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wl.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wd.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yv.shtwfgs.cn

================================================================================
来源：http://ms.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tt.panjiajie.cn

================================================================================
来源：http://jg.muxihuayi.cn

[Q01] 创建表
来源：http://lu.lnxyls.cn

CREATE TABLE users (
来源：http://ho.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kf.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://cw.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://pp.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://za.9csxet.cn

);
来源：http://xv.nszjky.cn

[Q02] 创建带外键的表
来源：http://la.nicolike.cn

CREATE TABLE orders (
来源：http://sf.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cj.9csxet.cn

user_id INT NOT NULL,
来源：http://cf.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://yi.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kg.szxytkj.cn

);
来源：http://ps.shtwfgs.cn

[Q03] 增加列
来源：http://lg.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pf.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://gp.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gg.huixiangedu.cn

[Q05] 重命名列
来源：http://qw.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sk.shxzukj.cn

[Q06] 删除列
来源：http://qy.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mg.hahajie.cn

[Q07] 删除表
来源：http://us.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://gb.jctech888.com.cn

[Q08] 创建普通索引
来源：http://mc.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hq.asd995.cn

[Q09] 创建唯一索引
来源：http://na.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cs.huanxung.cn

[Q10] 插入单行
来源：http://ry.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iy.shxzukj.cn

[Q11] 一次插入多行
来源：http://vu.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cr.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://vz.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yh.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pg.hahajie.cn

[Q13] 忽略重复插入
来源：http://fk.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bg.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://xd.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rb.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nv.huixiangedu.cn

[Q15] 查询全部
来源：http://da.szxytkj.cn

SELECT * FROM users;
来源：http://pi.nicolike.cn

[Q16] 查询指定列
来源：http://vu.521024.cn

SELECT id, name FROM users;
来源：http://ki.nszjky.cn

[Q17] 条件查询
来源：http://gi.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jj.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://rj.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dz.huanxung.cn

[Q19] 范围查询
来源：http://lh.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lw.lnxyls.cn

[Q20] IN 列表
来源：http://po.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tx.newstarts.cn

[Q21] 空值判断
来源：http://sq.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yu.yuexingan06.cn

[Q22] 排序
来源：http://ob.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ig.lnxyls.cn

[Q23] 分页
来源：http://sz.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yc.haigaiapp.cn

[Q24] 去重
来源：http://mx.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://xw.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://cv.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ho.wgjwhj.cn

[Q26] 计数
来源：http://tn.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://ve.521024.cn

[Q27] 条件计数
来源：http://jt.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iz.newstarts.cn

[Q28] 求和与平均
来源：http://ur.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mo.gzmigu.cn

[Q29] 最大最小值
来源：http://qi.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kg.szsharing.cn

[Q30] 分组统计
来源：http://ul.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xc.newstarts.cn

[Q31] 分组后过滤
来源：http://aa.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cv.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://oo.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iz.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://th.asd995.cn

[Q33] 多列分组
来源：http://cx.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wz.shxzskj.cn

[Q34] 每组取第一条
来源：http://ee.huixiangedu.cn

SELECT * FROM (
来源：http://vp.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kx.muxihuayi.cn

) t WHERE rn = 1;
来源：http://sc.szsharing.cn

[Q35] 内连接
来源：http://ap.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ak.shxzskj.cn

[Q36] 左连接
来源：http://af.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xu.shtwfgs.cn

[Q37] 右连接
来源：http://cw.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zl.wgjwhj.cn


<!-- 参考信息 -->