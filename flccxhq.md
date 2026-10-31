代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://te.newstarts.cn

[N10] 链表节点定义
来源：http://sx.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nd.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rj.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hl.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mw.asd995.cn

Java: class Node { int v; Node next; }
来源：http://rt.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zj.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mu.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pe.asd995.cn

[N11] 二叉树中序遍历
来源：http://vs.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://io.panjiajie.cn

PHP:  // 手写递归函数
来源：http://wk.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hd.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ct.huixinmuqiang.cn

Java: // 手写递归
来源：http://tc.nicolike.cn

Go:   // 手写递归
来源：http://wg.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jf.shxzskj.cn

C#:   // 手写递归
来源：http://zu.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cm.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uo.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ca.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://np.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tf.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fa.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vk.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qw.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://os.hnjuh.cn

================================================================================
来源：http://zy.asd995.cn

O. 并发与异步
来源：http://zi.newstarts.cn

================================================================================
来源：http://xx.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://fv.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hk.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ga.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sl.yuexingan06.cn

TS:   // 同 JS
来源：http://ng.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://cq.lnxyls.cn

Go:   go f()
来源：http://iz.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://jp.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://id.yuntaijiaju.cn

[O02] 使用线程池
来源：http://cn.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jm.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zy.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://rt.asd995.cn

TS:   // worker_threads 线程池
来源：http://lr.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cd.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fp.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://av.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ve.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://cz.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://pd.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://ci.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ik.asd995.cn

TS:   // 同 JS
来源：http://lf.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://nh.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dz.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://te.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://jy.hahajie.cn

[O04] 定义异步函数并等待
来源：http://ky.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://zi.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uk.521024.cn

JS:   async function f() { await g(); }
来源：http://dg.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qn.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tw.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yw.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cx.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://kr.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://eb.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://kf.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://un.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://lj.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://bo.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oq.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ej.nicolike.cn

Ruby: threads.map(&:join)
来源：http://ja.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ti.jctech888.com.cn

[O06] 使用进程池
来源：http://re.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bt.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gb.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://mf.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://uz.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ab.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uv.bookmarksfly.cn

Ruby: // fork 块
来源：http://zv.huanxung.cn

C#:   Parallel.For
来源：http://mz.haigaiapp.cn

================================================================================
来源：http://xd.haigaiapp.cn

P. 常用工具函数
来源：http://ec.lnxyls.cn

================================================================================
来源：http://oh.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://fg.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://tm.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wq.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://cs.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://sm.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://ru.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://pm.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://oe.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://cm.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://wy.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xd.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qm.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zp.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dg.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zj.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tt.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://as.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rj.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://nv.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://za.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ex.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://su.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jv.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://em.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://np.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qz.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ei.shxzukj.cn

[P04] 求长度
来源：http://fp.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sn.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bg.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ph.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kt.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://hk.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://pc.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://zd.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bj.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://av.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mq.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ks.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mf.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nn.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xu.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cn.jianghongdianzi.cn

Ruby: a == b
来源：http://dr.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://je.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nx.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bu.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://ak.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mm.shtwfgs.cn

TS:   if (x == null) {}
来源：http://qs.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://db.asd995.cn

Go:   if x == nil {}
来源：http://kx.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yu.haigaiapp.cn

C#:   if (x is null) {}
来源：http://xj.chemitech.net.cn

[P07] 防抖与节流
来源：http://mt.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nd.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://uo.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wl.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wb.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ld.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dl.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nr.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nt.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://qh.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bx.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://do.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://le.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zo.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ke.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eq.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dx.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bz.colortex.cn

================================================================================
来源：http://hc.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uu.bookmarksfly.cn

================================================================================
来源：http://tn.huixinmuqiang.cn

[Q01] 创建表
来源：http://vq.gzmigu.cn

CREATE TABLE users (
来源：http://tr.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bh.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://zs.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://rj.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jx.bookmarksfly.cn

);
来源：http://rt.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://tm.panjiajie.cn

CREATE TABLE orders (
来源：http://az.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ks.gzmigu.cn

user_id INT NOT NULL,
来源：http://ax.huanxung.cn

amount DECIMAL(10, 2),
来源：http://rv.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vm.bookmarksfly.cn

);
来源：http://pj.colortex.cn

[Q03] 增加列
来源：http://db.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wu.gzmigu.cn

[Q04] 修改列类型
来源：http://hl.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kx.hahajie.cn

[Q05] 重命名列
来源：http://wm.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://np.huixinmuqiang.cn

[Q06] 删除列
来源：http://dj.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ll.nszjky.cn

[Q07] 删除表
来源：http://qx.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://jg.colortex.cn

[Q08] 创建普通索引
来源：http://hp.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wr.nicolike.cn

[Q09] 创建唯一索引
来源：http://lc.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yl.szxytkj.cn

[Q10] 插入单行
来源：http://we.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ee.gzmigu.cn

[Q11] 一次插入多行
来源：http://ap.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yl.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://op.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tx.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mw.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://ps.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ts.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://sx.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://td.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ud.gzmigu.cn

[Q15] 查询全部
来源：http://be.panjiajie.cn

SELECT * FROM users;
来源：http://cr.szsharing.cn

[Q16] 查询指定列
来源：http://in.colortex.cn

SELECT id, name FROM users;
来源：http://lz.huanxung.cn

[Q17] 条件查询
来源：http://uo.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wp.9csxet.cn

[Q18] 模糊匹配
来源：http://jh.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://me.nicolike.cn

[Q19] 范围查询
来源：http://wy.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ok.huanxung.cn

[Q20] IN 列表
来源：http://ug.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ba.hahajie.cn

[Q21] 空值判断
来源：http://wf.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://om.newstarts.cn

[Q22] 排序
来源：http://gl.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zv.yuntaijiaju.cn

[Q23] 分页
来源：http://xl.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sg.bookmarksfly.cn

[Q24] 去重
来源：http://jo.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://do.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://me.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ij.hahajie.cn

[Q26] 计数
来源：http://fo.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://bi.muxihuayi.cn

[Q27] 条件计数
来源：http://xx.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ur.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://mc.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qz.huanxung.cn

[Q29] 最大最小值
来源：http://sc.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hv.lnxyls.cn

[Q30] 分组统计
来源：http://ne.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hb.newstarts.cn

[Q31] 分组后过滤
来源：http://ca.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tk.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://xh.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wt.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://of.nszjky.cn

[Q33] 多列分组
来源：http://jw.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jz.jctech888.com.cn

[Q34] 每组取第一条
来源：http://tw.9csxet.cn

SELECT * FROM (
来源：http://ej.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ac.521024.cn

) t WHERE rn = 1;
来源：http://zk.yuntaijiaju.cn

[Q35] 内连接
来源：http://rt.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ad.huixinmuqiang.cn

[Q36] 左连接
来源：http://hi.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://is.newstarts.cn

[Q37] 右连接
来源：http://fe.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jd.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hb.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qh.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://fh.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nm.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yd.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ry.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vx.colortex.cn

[Q41] 多表连接
来源：http://oi.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uc.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://fe.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://mq.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://ai.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://nm.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cy.bookmarksfly.cn

[Q43] 标量子查询
来源：http://jq.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gs.muxihuayi.cn

[Q44] IN 子查询
来源：http://qs.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://od.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://cu.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yk.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kf.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zj.nicolike.cn

[Q47] 与平均值比较
来源：http://na.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dz.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://ra.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kh.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://zb.haigaiapp.cn

[Q49] 更新单行
来源：http://um.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wd.shxzukj.cn

[Q50] 批量更新
来源：http://wo.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gn.lnxyls.cn

[Q51] 用子查询更新
来源：http://zg.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cz.hahajie.cn

[Q52] 删除指定行
来源：http://gg.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://xg.lnxyls.cn

[Q53] 按条件删除
来源：http://am.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gj.huixinmuqiang.cn

[Q54] 清空表
来源：http://za.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://hh.asd995.cn

[Q55] 排名（并列占位）
来源：http://gt.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://li.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://ts.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pv.colortex.cn

[Q57] 行号
来源：http://nw.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ob.gzmigu.cn

[Q58] 累计求和
来源：http://cm.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cw.nicolike.cn

[Q59] 分组内累计
来源：http://mx.panjiajie.cn


<!-- 参考信息 -->