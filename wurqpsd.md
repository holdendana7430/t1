代发 wailian999

Java: // 手写回溯递归
来源：http://ej.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://rg.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://sb.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://an.nszjky.cn

[N09] 栈与队列
来源：http://or.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ur.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qf.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qk.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ww.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jm.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vw.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mv.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ii.lnxyls.cn

[N10] 链表节点定义
来源：http://rt.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bi.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ks.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://in.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fh.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://pd.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oh.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sl.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dd.huanxung.cn

[N11] 二叉树中序遍历
来源：http://ut.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lo.huanxung.cn

PHP:  // 手写递归函数
来源：http://ti.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zg.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ye.jctech888.com.cn

Java: // 手写递归
来源：http://ss.chemitech.net.cn

Go:   // 手写递归
来源：http://fr.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rx.yuexingan06.cn

C#:   // 手写递归
来源：http://wk.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cr.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://br.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fi.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uk.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ku.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zs.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://im.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vf.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://us.muxihuayi.cn

================================================================================
来源：http://un.colortex.cn

O. 并发与异步
来源：http://mw.asd995.cn

================================================================================
来源：http://ld.bjjhwx.cn

[O01] 启动一个线程
来源：http://kw.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://va.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qf.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xh.bjjhwx.cn

TS:   // 同 JS
来源：http://uk.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://br.wgjwhj.cn

Go:   go f()
来源：http://mz.asd995.cn

Ruby: Thread.new { f }
来源：http://vo.521024.cn

C#:   Task.Run(() => F());
来源：http://tu.lnxyls.cn

[O02] 使用线程池
来源：http://ex.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ys.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gv.nszjky.cn

JS:   // worker_threads 线程池
来源：http://wr.colortex.cn

TS:   // worker_threads 线程池
来源：http://cn.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gx.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://el.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sb.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uw.asd995.cn

[O03] 加锁保护共享数据
来源：http://ik.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://uj.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://lb.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eh.yuntaijiaju.cn

TS:   // 同 JS
来源：http://qb.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://xq.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bl.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yn.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://sl.szsharing.cn

[O04] 定义异步函数并等待
来源：http://sv.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://cc.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ga.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://tj.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eq.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hu.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ao.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uc.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://zc.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://xo.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://fg.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ry.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://pv.colortex.cn

TS:   await Promise.all(tasks)
来源：http://gx.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://id.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://em.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://jw.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pc.wgjwhj.cn

[O06] 使用进程池
来源：http://ca.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wp.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yx.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://sz.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://om.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ww.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ly.chemitech.net.cn

Ruby: // fork 块
来源：http://be.huixinmuqiang.cn

C#:   Parallel.For
来源：http://vu.9csxet.cn

================================================================================
来源：http://kh.yuntaijiaju.cn

P. 常用工具函数
来源：http://io.chemitech.net.cn

================================================================================
来源：http://vw.bookmarksfly.cn

[P01] 生成 UUID
来源：http://qw.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://ii.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fh.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://qw.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ys.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://nk.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://pl.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://mr.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ps.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://pd.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tn.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dh.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wz.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qc.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oj.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kk.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dk.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xj.lnxyls.cn

[P03] 生成短随机字符串
来源：http://di.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://od.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dt.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yx.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jh.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wm.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zn.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://en.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pt.hahajie.cn

[P04] 求长度
来源：http://rb.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://er.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dd.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ci.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cq.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://pq.521024.cn

Go:   len(arr);  len(m)
来源：http://ai.nszjky.cn

Ruby: x.length;  x.size
来源：http://xw.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://aw.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://kc.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yv.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xa.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ea.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zk.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mh.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://js.colortex.cn

Ruby: a == b
来源：http://tm.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sx.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://km.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vu.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ms.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://py.hahajie.cn

TS:   if (x == null) {}
来源：http://em.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://io.szxytkj.cn

Go:   if x == nil {}
来源：http://pg.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zh.huanxung.cn

C#:   if (x is null) {}
来源：http://ux.newstarts.cn

[P07] 防抖与节流
来源：http://az.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ps.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://hv.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fy.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jj.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vt.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lc.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mw.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lc.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://ql.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cz.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bp.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hg.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wh.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ty.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cl.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eq.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://as.colortex.cn

================================================================================
来源：http://cr.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bj.yuntaijiaju.cn

================================================================================
来源：http://fn.nszjky.cn

[Q01] 创建表
来源：http://ph.shxzskj.cn

CREATE TABLE users (
来源：http://yz.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qx.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://vz.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://xz.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ao.newstarts.cn

);
来源：http://ct.gzmigu.cn

[Q02] 创建带外键的表
来源：http://cj.shxzukj.cn

CREATE TABLE orders (
来源：http://gm.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aq.gzmigu.cn

user_id INT NOT NULL,
来源：http://dm.nszjky.cn

amount DECIMAL(10, 2),
来源：http://sb.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://su.newstarts.cn

);
来源：http://sy.shtwfgs.cn

[Q03] 增加列
来源：http://iw.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rv.9csxet.cn

[Q04] 修改列类型
来源：http://yv.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fm.shtwfgs.cn

[Q05] 重命名列
来源：http://sf.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://um.jianghongdianzi.cn

[Q06] 删除列
来源：http://xd.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yk.asd995.cn

[Q07] 删除表
来源：http://mq.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://bq.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://pj.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ss.hahajie.cn

[Q09] 创建唯一索引
来源：http://rk.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://km.hnjuh.cn

[Q10] 插入单行
来源：http://ca.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ux.521024.cn

[Q11] 一次插入多行
来源：http://fp.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jk.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://ap.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iv.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ku.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://ol.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ry.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ci.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ev.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cb.shxzukj.cn

[Q15] 查询全部
来源：http://yb.bjjhwx.cn

SELECT * FROM users;
来源：http://am.nszjky.cn

[Q16] 查询指定列
来源：http://tu.9csxet.cn

SELECT id, name FROM users;
来源：http://bw.gzmigu.cn

[Q17] 条件查询
来源：http://pn.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wj.shxzukj.cn

[Q18] 模糊匹配
来源：http://tq.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nl.shxzskj.cn

[Q19] 范围查询
来源：http://ct.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ne.muxihuayi.cn

[Q20] IN 列表
来源：http://oq.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://be.hnjuh.cn

[Q21] 空值判断
来源：http://ln.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gr.huanxung.cn

[Q22] 排序
来源：http://ee.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ou.asd995.cn

[Q23] 分页
来源：http://eg.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ju.shxzukj.cn

[Q24] 去重
来源：http://ib.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://rs.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://ql.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pp.chemitech.net.cn

[Q26] 计数
来源：http://vp.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://nq.huixinmuqiang.cn

[Q27] 条件计数
来源：http://fy.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hv.shtwfgs.cn

[Q28] 求和与平均
来源：http://kh.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tz.asd995.cn

[Q29] 最大最小值
来源：http://nd.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://px.bookmarksfly.cn

[Q30] 分组统计
来源：http://ms.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ec.huanxung.cn

[Q31] 分组后过滤
来源：http://un.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kn.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://vu.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mi.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fl.jianghongdianzi.cn

[Q33] 多列分组
来源：http://al.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xg.muxihuayi.cn

[Q34] 每组取第一条
来源：http://hp.shxzukj.cn

SELECT * FROM (
来源：http://wy.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ty.lnxyls.cn

) t WHERE rn = 1;
来源：http://qp.yuntaijiaju.cn

[Q35] 内连接
来源：http://gx.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bu.bjjhwx.cn

[Q36] 左连接
来源：http://pm.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hi.huanxung.cn

[Q37] 右连接
来源：http://zc.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zr.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ev.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wb.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://pq.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sp.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://us.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ax.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mh.huixinmuqiang.cn

[Q41] 多表连接
来源：http://gd.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ku.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://ig.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://hp.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://lj.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://xi.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pa.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://kp.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xv.nszjky.cn

[Q44] IN 子查询
来源：http://pg.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ba.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://pe.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ar.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sr.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://io.9csxet.cn

[Q47] 与平均值比较
来源：http://tp.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ti.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://qf.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cf.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://xy.huixinmuqiang.cn

[Q49] 更新单行
来源：http://la.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oq.nszjky.cn

[Q50] 批量更新
来源：http://uu.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hh.shxzskj.cn

[Q51] 用子查询更新
来源：http://yg.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ic.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://kn.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://nw.lnxyls.cn

[Q53] 按条件删除
来源：http://cz.huixiangedu.cn


<!-- 参考信息 -->