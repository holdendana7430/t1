代发 wailian999

[N05] 最大公约数
来源：http://tj.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://dm.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wr.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sv.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vs.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qr.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kg.521024.cn

Ruby: a.gcd(b)
来源：http://ly.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ap.hahajie.cn

[N06] 判断回文字符串
来源：http://sl.hnjuh.cn

Py:   s == s[::-1]
来源：http://ue.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://gg.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://kb.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://hf.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ra.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://qd.szxytkj.cn

Ruby: s == s.reverse
来源：http://em.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lj.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://gs.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qq.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://md.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hf.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://gx.huanxung.cn

Java: // 手写 HashMap
来源：http://cr.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://mo.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://rq.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ya.hnjuh.cn

[N08] 生成全排列
来源：http://ts.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://re.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://va.shxzukj.cn

JS:   // 手写回溯递归
来源：http://gr.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://bn.bjjhwx.cn

Java: // 手写回溯递归
来源：http://bq.colortex.cn

Go:   // 手写回溯递归
来源：http://yu.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://ds.lnxyls.cn

C#:   // 手写回溯递归
来源：http://pi.gzmigu.cn

[N09] 栈与队列
来源：http://df.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nj.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cw.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vq.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ub.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hi.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vv.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jt.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ht.lnxyls.cn

[N10] 链表节点定义
来源：http://bu.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gn.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dd.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dx.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kq.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://nl.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cx.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yr.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hx.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://fe.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ye.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://ok.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sd.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jl.hnjuh.cn

Java: // 手写递归
来源：http://jk.chemitech.net.cn

Go:   // 手写递归
来源：http://dr.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ry.lnxyls.cn

C#:   // 手写递归
来源：http://lc.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ob.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bi.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bt.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://si.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fv.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rp.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ve.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://as.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yz.bookmarksfly.cn

================================================================================
来源：http://kq.chemitech.net.cn

O. 并发与异步
来源：http://wd.szsharing.cn

================================================================================
来源：http://sa.9csxet.cn

[O01] 启动一个线程
来源：http://oh.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tq.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gv.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ja.nicolike.cn

TS:   // 同 JS
来源：http://nm.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://kp.nszjky.cn

Go:   go f()
来源：http://je.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://cq.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://dt.szxytkj.cn

[O02] 使用线程池
来源：http://wr.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lv.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hd.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://ms.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://og.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ml.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sv.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ez.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kr.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://qw.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://pr.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ps.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://on.bookmarksfly.cn

TS:   // 同 JS
来源：http://ji.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://ro.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://md.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kk.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://zo.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://td.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://sm.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rg.huanxung.cn

JS:   async function f() { await g(); }
来源：http://qr.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hi.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://st.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qc.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ci.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://zt.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://lb.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ll.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fu.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://nw.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://yj.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bf.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tl.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://jg.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uq.muxihuayi.cn

[O06] 使用进程池
来源：http://yz.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jt.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ia.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://bz.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://qs.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dz.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lr.nicolike.cn

Ruby: // fork 块
来源：http://ar.bjjhwx.cn

C#:   Parallel.For
来源：http://qy.shtwfgs.cn

================================================================================
来源：http://im.huixiangedu.cn

P. 常用工具函数
来源：http://lj.gzmigu.cn

================================================================================
来源：http://mj.lnxyls.cn

[P01] 生成 UUID
来源：http://ib.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://is.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sn.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://hw.nszjky.cn

TS:   crypto.randomUUID()
来源：http://be.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://id.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://ql.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://zv.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://xu.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://kb.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ti.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oc.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mp.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vz.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kb.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tp.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bg.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eb.nicolike.cn

[P03] 生成短随机字符串
来源：http://qp.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ul.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qr.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vw.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tp.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yy.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wz.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yf.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gj.haigaiapp.cn

[P04] 求长度
来源：http://xn.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lu.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dj.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zc.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iw.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://wn.newstarts.cn

Go:   len(arr);  len(m)
来源：http://pf.asd995.cn

Ruby: x.length;  x.size
来源：http://fl.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dh.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://oi.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qi.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lg.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tb.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://io.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rk.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cw.yuexingan06.cn

Ruby: a == b
来源：http://rk.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cf.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lr.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qp.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://la.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rs.bjjhwx.cn

TS:   if (x == null) {}
来源：http://yx.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sa.shxzskj.cn

Go:   if x == nil {}
来源：http://om.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jq.muxihuayi.cn

C#:   if (x is null) {}
来源：http://th.asd995.cn

[P07] 防抖与节流
来源：http://bq.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ex.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://fp.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hf.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zq.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uy.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wd.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bx.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bk.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://rk.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aq.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://go.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ky.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qw.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pt.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lj.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hc.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ad.9csxet.cn

================================================================================
来源：http://td.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ja.newstarts.cn

================================================================================
来源：http://pz.muxihuayi.cn

[Q01] 创建表
来源：http://nz.jianghongdianzi.cn

CREATE TABLE users (
来源：http://hz.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ie.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://so.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://vq.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://td.shxzskj.cn

);
来源：http://ir.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://ng.yuexingan06.cn

CREATE TABLE orders (
来源：http://ls.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uk.gzmigu.cn

user_id INT NOT NULL,
来源：http://jd.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://ov.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ty.muxihuayi.cn

);
来源：http://eq.shxzukj.cn

[Q03] 增加列
来源：http://ag.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pc.newstarts.cn

[Q04] 修改列类型
来源：http://rp.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dg.wgjwhj.cn

[Q05] 重命名列
来源：http://uk.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mq.yuntaijiaju.cn

[Q06] 删除列
来源：http://ii.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mz.shxzskj.cn

[Q07] 删除表
来源：http://lv.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://ia.shxzukj.cn

[Q08] 创建普通索引
来源：http://tj.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vu.panjiajie.cn

[Q09] 创建唯一索引
来源：http://xe.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cn.muxihuayi.cn

[Q10] 插入单行
来源：http://rg.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oy.9csxet.cn

[Q11] 一次插入多行
来源：http://iq.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bs.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://az.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tr.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hr.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://jp.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tf.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://qt.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hj.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rq.haigaiapp.cn

[Q15] 查询全部
来源：http://pg.haigaiapp.cn

SELECT * FROM users;
来源：http://ge.panjiajie.cn

[Q16] 查询指定列
来源：http://op.colortex.cn

SELECT id, name FROM users;
来源：http://mx.jianghongdianzi.cn

[Q17] 条件查询
来源：http://ok.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ml.muxihuayi.cn

[Q18] 模糊匹配
来源：http://su.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ek.lnxyls.cn

[Q19] 范围查询
来源：http://my.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ud.newstarts.cn

[Q20] IN 列表
来源：http://vm.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sb.yuntaijiaju.cn

[Q21] 空值判断
来源：http://qc.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ei.hnjuh.cn

[Q22] 排序
来源：http://hw.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ca.muxihuayi.cn

[Q23] 分页
来源：http://qo.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ws.huanxung.cn

[Q24] 去重
来源：http://zh.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://vt.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://by.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vx.huixiangedu.cn

[Q26] 计数
来源：http://as.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://ej.asd995.cn

[Q27] 条件计数
来源：http://mx.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tt.asd995.cn

[Q28] 求和与平均
来源：http://dd.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://if.jctech888.com.cn

[Q29] 最大最小值
来源：http://zy.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vk.shtwfgs.cn

[Q30] 分组统计
来源：http://oc.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://si.lnxyls.cn

[Q31] 分组后过滤
来源：http://wq.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aw.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://pv.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tg.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sp.bjjhwx.cn

[Q33] 多列分组
来源：http://yp.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mi.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://ac.newstarts.cn

SELECT * FROM (
来源：http://pc.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hp.521024.cn

) t WHERE rn = 1;
来源：http://su.jianghongdianzi.cn

[Q35] 内连接
来源：http://fp.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mf.huixiangedu.cn

[Q36] 左连接
来源：http://xf.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lz.jctech888.com.cn

[Q37] 右连接
来源：http://vq.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tl.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pf.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fo.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ve.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uo.asd995.cn


<!-- 参考信息 -->