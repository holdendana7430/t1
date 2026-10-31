代发 wailian999

Go:   // 手写 map[int]int
来源：http://xb.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://uw.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rt.nicolike.cn

[N08] 生成全排列
来源：http://db.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://cy.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://it.szxytkj.cn

JS:   // 手写回溯递归
来源：http://qi.nicolike.cn

TS:   // 手写回溯递归
来源：http://kr.szsharing.cn

Java: // 手写回溯递归
来源：http://au.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://ee.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://xs.lnxyls.cn

C#:   // 手写回溯递归
来源：http://um.huixinmuqiang.cn

[N09] 栈与队列
来源：http://sl.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uy.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ps.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hy.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ub.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bg.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ax.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qd.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hl.colortex.cn

[N10] 链表节点定义
来源：http://nz.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qw.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mw.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ss.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://on.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://jj.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gv.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qf.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://da.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://xo.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pg.newstarts.cn

PHP:  // 手写递归函数
来源：http://fn.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wq.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mx.huanxung.cn

Java: // 手写递归
来源：http://oj.shxzskj.cn

Go:   // 手写递归
来源：http://li.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lp.gzmigu.cn

C#:   // 手写递归
来源：http://oh.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qr.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bs.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uy.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kt.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xp.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dc.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jl.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xf.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yh.chemitech.net.cn

================================================================================
来源：http://bs.nicolike.cn

O. 并发与异步
来源：http://sg.szsharing.cn

================================================================================
来源：http://gg.nszjky.cn

[O01] 启动一个线程
来源：http://ky.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://au.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uc.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wz.huanxung.cn

TS:   // 同 JS
来源：http://sy.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://vc.szxytkj.cn

Go:   go f()
来源：http://bh.shxzskj.cn

Ruby: Thread.new { f }
来源：http://ji.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://wc.huixiangedu.cn

[O02] 使用线程池
来源：http://gq.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fa.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yo.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://lc.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://hv.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cf.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qi.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://co.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qy.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://kb.shxzskj.cn

Py:   with lock: shared += 1
来源：http://do.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://zd.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oa.hahajie.cn

TS:   // 同 JS
来源：http://jz.521024.cn

Java: synchronized (this) { shared++; }
来源：http://nw.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fv.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rv.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://tn.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://co.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://bu.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vj.newstarts.cn

JS:   async function f() { await g(); }
来源：http://fm.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kb.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yi.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kr.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qb.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://xv.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://rr.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://bh.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mi.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://fs.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://ew.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ts.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://do.9csxet.cn

Ruby: threads.map(&:join)
来源：http://kv.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oq.szsharing.cn

[O06] 使用进程池
来源：http://af.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cx.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pj.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://lc.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://xc.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vs.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ik.asd995.cn

Ruby: // fork 块
来源：http://ka.shxzskj.cn

C#:   Parallel.For
来源：http://lh.hahajie.cn

================================================================================
来源：http://cq.huixiangedu.cn

P. 常用工具函数
来源：http://zf.521024.cn

================================================================================
来源：http://am.colortex.cn

[P01] 生成 UUID
来源：http://dy.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://et.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gx.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://ww.asd995.cn

TS:   crypto.randomUUID()
来源：http://de.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://vz.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://wa.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://go.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://ax.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://jd.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iy.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xv.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://po.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://im.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dc.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ld.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ux.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mr.nszjky.cn

[P03] 生成短随机字符串
来源：http://tf.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hd.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ch.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mw.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://an.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tj.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yx.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sm.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ls.gzmigu.cn

[P04] 求长度
来源：http://fq.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fb.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iv.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ko.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://za.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://sz.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://sf.newstarts.cn

Ruby: x.length;  x.size
来源：http://dh.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://et.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://nf.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://le.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rc.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pq.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kh.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uj.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://od.jctech888.com.cn

Ruby: a == b
来源：http://bg.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mm.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vu.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mn.colortex.cn

PHP:  if (empty($x)) {}
来源：http://xn.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pf.shxzskj.cn

TS:   if (x == null) {}
来源：http://pr.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ei.nszjky.cn

Go:   if x == nil {}
来源：http://vm.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ni.shxzskj.cn

C#:   if (x is null) {}
来源：http://rv.9csxet.cn

[P07] 防抖与节流
来源：http://cp.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lr.521024.cn

PHP:  // 手写时间戳比较
来源：http://ge.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sb.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mx.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yj.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pa.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vm.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://np.nicolike.cn

[P08] 处理浮点精度问题
来源：http://vn.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yg.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://an.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://da.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xy.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bi.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mb.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fm.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tb.muxihuayi.cn

================================================================================
来源：http://ia.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hs.nicolike.cn

================================================================================
来源：http://or.gzmigu.cn

[Q01] 创建表
来源：http://ne.521024.cn

CREATE TABLE users (
来源：http://bk.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aj.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://zv.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://xa.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ka.asd995.cn

);
来源：http://fm.colortex.cn

[Q02] 创建带外键的表
来源：http://qn.jctech888.com.cn

CREATE TABLE orders (
来源：http://nc.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wr.szxytkj.cn

user_id INT NOT NULL,
来源：http://gx.9csxet.cn

amount DECIMAL(10, 2),
来源：http://am.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wp.asd995.cn

);
来源：http://vj.newstarts.cn

[Q03] 增加列
来源：http://ra.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ee.jctech888.com.cn

[Q04] 修改列类型
来源：http://th.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fw.hnjuh.cn

[Q05] 重命名列
来源：http://ry.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iu.nszjky.cn

[Q06] 删除列
来源：http://zi.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tr.yuntaijiaju.cn

[Q07] 删除表
来源：http://rf.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://le.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://mi.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cr.nicolike.cn

[Q09] 创建唯一索引
来源：http://sc.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ff.bjjhwx.cn

[Q10] 插入单行
来源：http://vi.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oq.shtwfgs.cn

[Q11] 一次插入多行
来源：http://mc.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lf.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://ar.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lj.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dn.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://nh.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nc.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://tb.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mo.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ez.muxihuayi.cn

[Q15] 查询全部
来源：http://zg.gzmigu.cn

SELECT * FROM users;
来源：http://bo.bookmarksfly.cn

[Q16] 查询指定列
来源：http://gs.szsharing.cn

SELECT id, name FROM users;
来源：http://fq.shtwfgs.cn

[Q17] 条件查询
来源：http://jc.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rk.lnxyls.cn

[Q18] 模糊匹配
来源：http://jg.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xi.huixinmuqiang.cn

[Q19] 范围查询
来源：http://nx.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://um.nszjky.cn

[Q20] IN 列表
来源：http://ws.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vt.bookmarksfly.cn

[Q21] 空值判断
来源：http://tx.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zf.bjjhwx.cn

[Q22] 排序
来源：http://zz.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hm.haigaiapp.cn

[Q23] 分页
来源：http://kv.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://de.newstarts.cn

[Q24] 去重
来源：http://nf.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://rv.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://ox.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lq.panjiajie.cn

[Q26] 计数
来源：http://bm.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://ma.nszjky.cn

[Q27] 条件计数
来源：http://gv.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oz.nicolike.cn

[Q28] 求和与平均
来源：http://tr.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kf.yuexingan06.cn

[Q29] 最大最小值
来源：http://nd.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://no.lnxyls.cn

[Q30] 分组统计
来源：http://wv.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ng.newstarts.cn

[Q31] 分组后过滤
来源：http://nj.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ho.nszjky.cn

[Q32] 分组拼接字符串
来源：http://zw.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mg.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://op.wgjwhj.cn

[Q33] 多列分组
来源：http://jk.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xe.bjjhwx.cn

[Q34] 每组取第一条
来源：http://qt.gzmigu.cn

SELECT * FROM (
来源：http://sz.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ix.hahajie.cn

) t WHERE rn = 1;
来源：http://fg.wgjwhj.cn

[Q35] 内连接
来源：http://nm.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mk.newstarts.cn

[Q36] 左连接
来源：http://or.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ig.hahajie.cn

[Q37] 右连接
来源：http://xe.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jc.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ei.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ss.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://ur.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ad.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ty.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vu.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zc.lnxyls.cn

[Q41] 多表连接
来源：http://by.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bb.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://cw.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://xd.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://bt.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://bg.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xg.yuexingan06.cn

[Q43] 标量子查询
来源：http://sr.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kx.panjiajie.cn

[Q44] IN 子查询
来源：http://by.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tm.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://tb.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jb.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yz.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zo.nszjky.cn

[Q47] 与平均值比较
来源：http://wn.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yn.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://eb.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eh.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://sy.shxzukj.cn

[Q49] 更新单行
来源：http://ao.shtwfgs.cn


<!-- 参考信息 -->