代发 wailian999

[N05] 最大公约数
来源：http://cl.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://wr.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xl.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iv.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mv.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rs.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ra.asd995.cn

Ruby: a.gcd(b)
来源：http://pw.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://si.szxytkj.cn

[N06] 判断回文字符串
来源：http://vs.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://yz.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://uo.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://ey.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://fr.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fz.asd995.cn

Go:   // 双指针从两端比较
来源：http://ed.nszjky.cn

Ruby: s == s.reverse
来源：http://at.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://um.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://yk.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ee.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mm.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jn.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://sx.newstarts.cn

Java: // 手写 HashMap
来源：http://ft.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://nd.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ls.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zq.panjiajie.cn

[N08] 生成全排列
来源：http://fh.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://tq.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://fg.hahajie.cn

JS:   // 手写回溯递归
来源：http://qe.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://vl.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://iv.nszjky.cn

Go:   // 手写回溯递归
来源：http://yj.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://ov.lnxyls.cn

C#:   // 手写回溯递归
来源：http://ge.asd995.cn

[N09] 栈与队列
来源：http://mc.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kq.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://am.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pz.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oz.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kf.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jq.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ve.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ee.nicolike.cn

[N10] 链表节点定义
来源：http://mz.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dl.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://op.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bk.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pq.colortex.cn

Java: class Node { int v; Node next; }
来源：http://mu.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ku.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kz.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xj.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://su.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ez.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://wd.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wi.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://di.shtwfgs.cn

Java: // 手写递归
来源：http://ci.huixinmuqiang.cn

Go:   // 手写递归
来源：http://ku.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iz.bjjhwx.cn

C#:   // 手写递归
来源：http://es.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jw.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vh.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jn.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zm.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vk.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ni.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lc.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gu.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ts.nicolike.cn

================================================================================
来源：http://qb.shxzukj.cn

O. 并发与异步
来源：http://ax.9csxet.cn

================================================================================
来源：http://jh.szsharing.cn

[O01] 启动一个线程
来源：http://oo.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rj.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qh.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bo.yuexingan06.cn

TS:   // 同 JS
来源：http://fw.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://uf.nicolike.cn

Go:   go f()
来源：http://ku.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://bv.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://xa.wgjwhj.cn

[O02] 使用线程池
来源：http://ky.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jn.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jt.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://nt.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://jp.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sy.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vb.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uy.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qt.nicolike.cn

[O03] 加锁保护共享数据
来源：http://ev.gzmigu.cn

Py:   with lock: shared += 1
来源：http://jm.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://qr.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lj.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ut.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://px.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hw.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fl.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://nh.szsharing.cn

[O04] 定义异步函数并等待
来源：http://vv.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://wr.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zk.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://lb.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nc.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hc.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uc.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wa.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://cy.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://ks.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://pc.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://il.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://hi.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://yw.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ur.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qh.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://tt.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rm.wgjwhj.cn

[O06] 使用进程池
来源：http://cn.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://la.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ek.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://iy.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://qk.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ix.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kw.nicolike.cn

Ruby: // fork 块
来源：http://ft.9csxet.cn

C#:   Parallel.For
来源：http://qa.huixinmuqiang.cn

================================================================================
来源：http://fl.bookmarksfly.cn

P. 常用工具函数
来源：http://vs.asd995.cn

================================================================================
来源：http://rq.newstarts.cn

[P01] 生成 UUID
来源：http://ns.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://le.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wl.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://dg.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://ys.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://yp.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://to.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://ee.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://zp.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://ht.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ka.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xs.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jg.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mh.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tn.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hl.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wn.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vb.nszjky.cn

[P03] 生成短随机字符串
来源：http://da.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cs.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oi.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mu.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xi.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ku.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cz.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ak.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fu.hahajie.cn

[P04] 求长度
来源：http://nw.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zy.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pc.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ky.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dv.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://ds.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://zz.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://bc.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mj.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://le.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ds.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mz.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ui.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ce.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://et.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lz.shxzukj.cn

Ruby: a == b
来源：http://za.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://db.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gs.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ld.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://vp.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cf.jctech888.com.cn

TS:   if (x == null) {}
来源：http://zs.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wv.wgjwhj.cn

Go:   if x == nil {}
来源：http://no.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sc.huixiangedu.cn

C#:   if (x is null) {}
来源：http://gu.szxytkj.cn

[P07] 防抖与节流
来源：http://ol.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pq.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://ps.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lp.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ph.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hh.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hg.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ul.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lu.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://aa.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aa.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pi.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bg.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://et.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://au.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gj.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fq.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rd.bookmarksfly.cn

================================================================================
来源：http://ym.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zi.asd995.cn

================================================================================
来源：http://gn.muxihuayi.cn

[Q01] 创建表
来源：http://bm.haigaiapp.cn

CREATE TABLE users (
来源：http://nc.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ot.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://wn.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://dp.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://he.szsharing.cn

);
来源：http://un.9csxet.cn

[Q02] 创建带外键的表
来源：http://wv.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://fa.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xk.shxzukj.cn

user_id INT NOT NULL,
来源：http://sq.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://ds.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://od.gzmigu.cn

);
来源：http://tf.muxihuayi.cn

[Q03] 增加列
来源：http://dk.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yw.huanxung.cn

[Q04] 修改列类型
来源：http://kr.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tv.asd995.cn

[Q05] 重命名列
来源：http://ex.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ma.jctech888.com.cn

[Q06] 删除列
来源：http://js.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sd.hnjuh.cn

[Q07] 删除表
来源：http://vj.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://tj.hnjuh.cn

[Q08] 创建普通索引
来源：http://jr.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oz.huanxung.cn

[Q09] 创建唯一索引
来源：http://vt.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bg.shtwfgs.cn

[Q10] 插入单行
来源：http://ds.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pq.colortex.cn

[Q11] 一次插入多行
来源：http://dc.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dx.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://rs.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lh.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pz.shxzukj.cn

[Q13] 忽略重复插入
来源：http://en.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ws.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://po.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gk.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://da.muxihuayi.cn

[Q15] 查询全部
来源：http://fu.haigaiapp.cn

SELECT * FROM users;
来源：http://la.huanxung.cn

[Q16] 查询指定列
来源：http://dd.9csxet.cn

SELECT id, name FROM users;
来源：http://lt.colortex.cn

[Q17] 条件查询
来源：http://pj.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iz.hnjuh.cn

[Q18] 模糊匹配
来源：http://et.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lx.huixinmuqiang.cn

[Q19] 范围查询
来源：http://qu.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lt.chemitech.net.cn

[Q20] IN 列表
来源：http://hr.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qj.hahajie.cn

[Q21] 空值判断
来源：http://tw.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eq.lnxyls.cn

[Q22] 排序
来源：http://gg.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wg.jianghongdianzi.cn

[Q23] 分页
来源：http://tz.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vm.yuntaijiaju.cn

[Q24] 去重
来源：http://kd.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ic.521024.cn

[Q25] 只取前 N 条
来源：http://gx.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ia.jctech888.com.cn

[Q26] 计数
来源：http://bd.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://st.panjiajie.cn

[Q27] 条件计数
来源：http://rs.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mp.lnxyls.cn

[Q28] 求和与平均
来源：http://ox.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rk.shtwfgs.cn

[Q29] 最大最小值
来源：http://nb.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zf.yuexingan06.cn

[Q30] 分组统计
来源：http://ae.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tg.panjiajie.cn

[Q31] 分组后过滤
来源：http://hf.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oe.colortex.cn

[Q32] 分组拼接字符串
来源：http://zg.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://la.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://az.chemitech.net.cn

[Q33] 多列分组
来源：http://wd.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vg.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://nj.yuexingan06.cn

SELECT * FROM (
来源：http://zr.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mb.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://qh.huanxung.cn

[Q35] 内连接
来源：http://uk.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bh.hahajie.cn

[Q36] 左连接
来源：http://fk.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sf.lnxyls.cn

[Q37] 右连接
来源：http://gt.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bj.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://us.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://be.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://ox.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zh.wgjwhj.cn


<!-- 参考信息 -->