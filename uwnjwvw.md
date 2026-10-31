代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hw.521024.cn

PHP:  // 手写递归交换
来源：http://tg.521024.cn

JS:   // 手写回溯递归
来源：http://lu.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://rx.szsharing.cn

Java: // 手写回溯递归
来源：http://fc.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://ra.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://pu.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://jd.jianghongdianzi.cn

[N09] 栈与队列
来源：http://ut.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://js.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ek.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wy.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ep.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gc.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ie.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kp.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ke.shtwfgs.cn

[N10] 链表节点定义
来源：http://ff.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gw.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yy.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ds.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ma.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://dx.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://il.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zc.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pa.nszjky.cn

[N11] 二叉树中序遍历
来源：http://rf.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ag.nszjky.cn

PHP:  // 手写递归函数
来源：http://su.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sj.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lr.panjiajie.cn

Java: // 手写递归
来源：http://yy.hnjuh.cn

Go:   // 手写递归
来源：http://jk.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ta.9csxet.cn

C#:   // 手写递归
来源：http://pp.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wo.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pt.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zw.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sd.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ea.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yr.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lt.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ei.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rn.szxytkj.cn

================================================================================
来源：http://yw.521024.cn

O. 并发与异步
来源：http://vs.hahajie.cn

================================================================================
来源：http://sp.newstarts.cn

[O01] 启动一个线程
来源：http://zw.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://po.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xx.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pa.gzmigu.cn

TS:   // 同 JS
来源：http://cq.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://gt.hahajie.cn

Go:   go f()
来源：http://go.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://ne.9csxet.cn

C#:   Task.Run(() => F());
来源：http://he.muxihuayi.cn

[O02] 使用线程池
来源：http://us.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uc.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ro.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://fz.asd995.cn

TS:   // worker_threads 线程池
来源：http://tl.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vd.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tu.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jk.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aj.szsharing.cn

[O03] 加锁保护共享数据
来源：http://ly.shxzukj.cn

Py:   with lock: shared += 1
来源：http://vb.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://mt.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fu.asd995.cn

TS:   // 同 JS
来源：http://fi.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://oy.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ca.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bz.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ji.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://jn.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://ba.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ff.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://ol.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zs.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uo.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ya.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ev.521024.cn

C#:   async Task F() { await G(); }
来源：http://ci.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://xk.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://xq.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://be.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://qw.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://tj.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xy.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ik.nicolike.cn

Ruby: threads.map(&:join)
来源：http://xf.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://al.panjiajie.cn

[O06] 使用进程池
来源：http://gn.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jk.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ji.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://kf.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://ok.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wg.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jc.huixinmuqiang.cn

Ruby: // fork 块
来源：http://cp.shxzskj.cn

C#:   Parallel.For
来源：http://gg.521024.cn

================================================================================
来源：http://ox.asd995.cn

P. 常用工具函数
来源：http://kb.asd995.cn

================================================================================
来源：http://nz.hahajie.cn

[P01] 生成 UUID
来源：http://cp.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://ns.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bm.huanxung.cn

JS:   crypto.randomUUID()
来源：http://kg.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://no.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://lk.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://ns.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://pa.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://hb.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://jt.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wa.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mj.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gj.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://by.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ch.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gq.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sr.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sn.shxzskj.cn

[P03] 生成短随机字符串
来源：http://nu.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tf.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fb.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hr.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sv.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qu.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jz.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://db.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zr.hnjuh.cn

[P04] 求长度
来源：http://gy.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wz.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ix.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jn.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nq.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://rs.newstarts.cn

Go:   len(arr);  len(m)
来源：http://oq.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://qm.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sa.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://fi.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ru.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mr.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pw.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gz.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fl.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xh.9csxet.cn

Ruby: a == b
来源：http://py.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://af.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hf.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ja.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://ba.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://if.asd995.cn

TS:   if (x == null) {}
来源：http://vt.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qq.nszjky.cn

Go:   if x == nil {}
来源：http://hf.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dr.bjjhwx.cn

C#:   if (x is null) {}
来源：http://pm.yuexingan06.cn

[P07] 防抖与节流
来源：http://ub.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ra.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://wf.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zl.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vu.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ob.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://og.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ua.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gl.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://ls.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ve.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vb.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mt.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pp.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fd.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oi.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://th.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hg.huixinmuqiang.cn

================================================================================
来源：http://ad.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ai.huanxung.cn

================================================================================
来源：http://za.huixinmuqiang.cn

[Q01] 创建表
来源：http://ps.lnxyls.cn

CREATE TABLE users (
来源：http://kg.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wr.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://cf.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://xc.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vw.szxytkj.cn

);
来源：http://xw.szxytkj.cn

[Q02] 创建带外键的表
来源：http://xz.nicolike.cn

CREATE TABLE orders (
来源：http://gm.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://er.szxytkj.cn

user_id INT NOT NULL,
来源：http://ph.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://mo.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mt.hahajie.cn

);
来源：http://qi.yuexingan06.cn

[Q03] 增加列
来源：http://zb.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ph.chemitech.net.cn

[Q04] 修改列类型
来源：http://ph.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hn.9csxet.cn

[Q05] 重命名列
来源：http://hr.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yt.gzmigu.cn

[Q06] 删除列
来源：http://fi.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vd.shtwfgs.cn

[Q07] 删除表
来源：http://fx.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://ve.newstarts.cn

[Q08] 创建普通索引
来源：http://dz.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kb.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://gn.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://he.newstarts.cn

[Q10] 插入单行
来源：http://xt.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mp.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://ng.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nm.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://vv.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qo.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vu.asd995.cn

[Q13] 忽略重复插入
来源：http://gm.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://td.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://gz.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jx.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jg.9csxet.cn

[Q15] 查询全部
来源：http://yj.szxytkj.cn

SELECT * FROM users;
来源：http://pj.huixiangedu.cn

[Q16] 查询指定列
来源：http://bv.asd995.cn

SELECT id, name FROM users;
来源：http://pq.asd995.cn

[Q17] 条件查询
来源：http://xo.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zj.huixiangedu.cn

[Q18] 模糊匹配
来源：http://cd.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://go.bjjhwx.cn

[Q19] 范围查询
来源：http://au.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wl.shxzukj.cn

[Q20] IN 列表
来源：http://ub.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pn.hnjuh.cn

[Q21] 空值判断
来源：http://rr.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://va.asd995.cn

[Q22] 排序
来源：http://mx.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://il.huanxung.cn

[Q23] 分页
来源：http://bh.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ww.haigaiapp.cn

[Q24] 去重
来源：http://uw.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://fg.huanxung.cn

[Q25] 只取前 N 条
来源：http://ny.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://it.jianghongdianzi.cn

[Q26] 计数
来源：http://yo.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://wq.521024.cn

[Q27] 条件计数
来源：http://ps.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nw.huixiangedu.cn

[Q28] 求和与平均
来源：http://go.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yk.shxzukj.cn

[Q29] 最大最小值
来源：http://tr.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ap.colortex.cn

[Q30] 分组统计
来源：http://az.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mq.shxzukj.cn

[Q31] 分组后过滤
来源：http://fx.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ze.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://az.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://js.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lw.yuntaijiaju.cn

[Q33] 多列分组
来源：http://gy.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ph.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://uv.asd995.cn

SELECT * FROM (
来源：http://xb.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mu.szxytkj.cn

) t WHERE rn = 1;
来源：http://jd.lnxyls.cn

[Q35] 内连接
来源：http://uc.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jj.bjjhwx.cn

[Q36] 左连接
来源：http://la.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pg.szsharing.cn

[Q37] 右连接
来源：http://sp.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kw.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hf.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gn.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://xv.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eb.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qb.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://my.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ik.jctech888.com.cn

[Q41] 多表连接
来源：http://qc.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qr.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://pv.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://pg.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://sc.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://aq.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tp.nszjky.cn

[Q43] 标量子查询
来源：http://ol.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sb.hnjuh.cn

[Q44] IN 子查询
来源：http://qw.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vv.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://ib.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wh.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pm.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://er.gzmigu.cn

[Q47] 与平均值比较
来源：http://qx.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gk.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://xn.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zc.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://li.muxihuayi.cn

[Q49] 更新单行
来源：http://nz.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ft.newstarts.cn

[Q50] 批量更新
来源：http://uj.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ka.colortex.cn

[Q51] 用子查询更新
来源：http://iu.muxihuayi.cn


<!-- 参考信息 -->