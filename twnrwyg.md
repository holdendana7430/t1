代发 wailian999

Go:   // 手写 map[int]int
来源：http://si.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://au.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oo.9csxet.cn

[N08] 生成全排列
来源：http://li.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://mk.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://it.lnxyls.cn

JS:   // 手写回溯递归
来源：http://ya.hahajie.cn

TS:   // 手写回溯递归
来源：http://qz.nszjky.cn

Java: // 手写回溯递归
来源：http://ai.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://mv.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://pj.hnjuh.cn

C#:   // 手写回溯递归
来源：http://fs.yuntaijiaju.cn

[N09] 栈与队列
来源：http://rj.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zy.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tm.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xn.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kn.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zn.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://on.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://va.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cy.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://ka.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://co.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bg.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qn.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ut.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://xz.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zh.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mf.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zi.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://ij.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nj.hnjuh.cn

PHP:  // 手写递归函数
来源：http://ky.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wv.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dw.jianghongdianzi.cn

Java: // 手写递归
来源：http://qf.chemitech.net.cn

Go:   // 手写递归
来源：http://io.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bt.panjiajie.cn

C#:   // 手写递归
来源：http://tr.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vi.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nh.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hs.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ou.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ip.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wq.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dx.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qe.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sf.jianghongdianzi.cn

================================================================================
来源：http://xh.nszjky.cn

O. 并发与异步
来源：http://zt.shxzskj.cn

================================================================================
来源：http://jm.wgjwhj.cn

[O01] 启动一个线程
来源：http://xd.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xg.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gr.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fo.yuexingan06.cn

TS:   // 同 JS
来源：http://jk.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://jw.nszjky.cn

Go:   go f()
来源：http://lq.newstarts.cn

Ruby: Thread.new { f }
来源：http://zb.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://rj.haigaiapp.cn

[O02] 使用线程池
来源：http://wn.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rq.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wz.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://eh.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://kt.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ml.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dw.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ip.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ny.nicolike.cn

[O03] 加锁保护共享数据
来源：http://ps.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://qj.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://pj.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ug.bjjhwx.cn

TS:   // 同 JS
来源：http://ej.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://sd.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ps.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jg.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://no.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://mi.colortex.cn

Py:   async def f():⏎    await g()
来源：http://br.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ce.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://js.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://le.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mr.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dn.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vs.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://gn.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://en.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://nh.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rg.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://wa.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://pi.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qf.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://df.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://yl.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vn.muxihuayi.cn

[O06] 使用进程池
来源：http://pf.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pw.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ds.521024.cn

JS:   // child_process / cluster 模块
来源：http://lk.colortex.cn

TS:   // child_process / cluster 模块
来源：http://mi.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ws.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oi.colortex.cn

Ruby: // fork 块
来源：http://hm.nszjky.cn

C#:   Parallel.For
来源：http://zg.521024.cn

================================================================================
来源：http://ms.panjiajie.cn

P. 常用工具函数
来源：http://td.haigaiapp.cn

================================================================================
来源：http://bi.lnxyls.cn

[P01] 生成 UUID
来源：http://rq.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://cf.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iv.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://ff.asd995.cn

TS:   crypto.randomUUID()
来源：http://qw.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://cl.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://ix.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://gi.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://dv.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://zl.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nc.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uc.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nt.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ht.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aa.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rk.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jl.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mq.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://rs.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pg.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://or.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ms.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lh.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pf.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://co.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://by.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ek.huixiangedu.cn

[P04] 求长度
来源：http://ww.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://te.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ev.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eh.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oy.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://wz.nicolike.cn

Go:   len(arr);  len(m)
来源：http://il.521024.cn

Ruby: x.length;  x.size
来源：http://vr.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rv.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://xe.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yw.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pv.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iw.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pn.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yr.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qi.521024.cn

Ruby: a == b
来源：http://mi.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ha.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://az.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ba.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://yx.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ln.wgjwhj.cn

TS:   if (x == null) {}
来源：http://xp.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jc.yuexingan06.cn

Go:   if x == nil {}
来源：http://gi.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ml.szxytkj.cn

C#:   if (x is null) {}
来源：http://sy.chemitech.net.cn

[P07] 防抖与节流
来源：http://ry.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ir.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://yc.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ke.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yn.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tm.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://au.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ea.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gl.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://mc.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ge.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qc.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xw.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mz.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cy.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wm.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hv.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xz.wgjwhj.cn

================================================================================
来源：http://rn.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ah.hnjuh.cn

================================================================================
来源：http://gh.huixinmuqiang.cn

[Q01] 创建表
来源：http://rs.chemitech.net.cn

CREATE TABLE users (
来源：http://df.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fh.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://ib.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://st.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bz.bjjhwx.cn

);
来源：http://pt.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://tg.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://sy.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ca.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://ae.nicolike.cn

amount DECIMAL(10, 2),
来源：http://nm.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pd.szxytkj.cn

);
来源：http://rn.yuntaijiaju.cn

[Q03] 增加列
来源：http://ou.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tl.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://kz.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ml.jianghongdianzi.cn

[Q05] 重命名列
来源：http://bc.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ax.huanxung.cn

[Q06] 删除列
来源：http://vu.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fz.jctech888.com.cn

[Q07] 删除表
来源：http://de.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://xs.huanxung.cn

[Q08] 创建普通索引
来源：http://pm.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hb.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://fk.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xl.huixiangedu.cn

[Q10] 插入单行
来源：http://wj.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ep.wgjwhj.cn

[Q11] 一次插入多行
来源：http://qc.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pk.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://js.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://th.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://em.shxzskj.cn

[Q13] 忽略重复插入
来源：http://am.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xr.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://dn.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bn.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dj.521024.cn

[Q15] 查询全部
来源：http://ok.shxzskj.cn

SELECT * FROM users;
来源：http://bj.szxytkj.cn

[Q16] 查询指定列
来源：http://uv.yuexingan06.cn

SELECT id, name FROM users;
来源：http://da.huixinmuqiang.cn

[Q17] 条件查询
来源：http://ba.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aq.jctech888.com.cn

[Q18] 模糊匹配
来源：http://sk.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sl.nicolike.cn

[Q19] 范围查询
来源：http://bd.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nj.shxzukj.cn

[Q20] IN 列表
来源：http://hc.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ku.huixinmuqiang.cn

[Q21] 空值判断
来源：http://tc.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mj.panjiajie.cn

[Q22] 排序
来源：http://ef.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ef.9csxet.cn

[Q23] 分页
来源：http://no.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iz.wgjwhj.cn

[Q24] 去重
来源：http://we.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://nr.9csxet.cn

[Q25] 只取前 N 条
来源：http://at.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tq.jianghongdianzi.cn

[Q26] 计数
来源：http://gt.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://ct.szsharing.cn

[Q27] 条件计数
来源：http://vz.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gq.newstarts.cn

[Q28] 求和与平均
来源：http://ot.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ze.lnxyls.cn

[Q29] 最大最小值
来源：http://qu.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zw.wgjwhj.cn

[Q30] 分组统计
来源：http://cr.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ua.yuexingan06.cn

[Q31] 分组后过滤
来源：http://ex.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zr.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://zt.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://va.hnjuh.cn

[Q33] 多列分组
来源：http://jc.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cg.muxihuayi.cn

[Q34] 每组取第一条
来源：http://hb.huanxung.cn

SELECT * FROM (
来源：http://ny.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vb.muxihuayi.cn

) t WHERE rn = 1;
来源：http://wk.chemitech.net.cn

[Q35] 内连接
来源：http://km.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://so.jctech888.com.cn

[Q36] 左连接
来源：http://bg.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eu.huanxung.cn

[Q37] 右连接
来源：http://uj.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://la.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://om.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://au.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://on.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dp.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://re.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ui.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gu.yuntaijiaju.cn

[Q41] 多表连接
来源：http://dx.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rb.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://cr.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://xb.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://by.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://hj.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mm.521024.cn

[Q43] 标量子查询
来源：http://ev.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dx.szsharing.cn

[Q44] IN 子查询
来源：http://fd.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://od.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://vd.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yj.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kc.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ch.bjjhwx.cn

[Q47] 与平均值比较
来源：http://en.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wb.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://wi.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fg.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://rg.lnxyls.cn

[Q49] 更新单行
来源：http://to.jctech888.com.cn


<!-- 参考信息 -->