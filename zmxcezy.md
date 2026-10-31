代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tq.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nu.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ld.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eg.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tx.hahajie.cn

[N10] 链表节点定义
来源：http://gw.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gc.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ni.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://st.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cp.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://ih.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ry.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bt.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gi.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://sy.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xu.shxzskj.cn

PHP:  // 手写递归函数
来源：http://pg.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kt.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dt.yuntaijiaju.cn

Java: // 手写递归
来源：http://pm.shxzukj.cn

Go:   // 手写递归
来源：http://xo.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://od.521024.cn

C#:   // 手写递归
来源：http://yt.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ao.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jm.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yk.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oe.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eg.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gw.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://he.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ye.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.szsharing.cn

================================================================================
来源：http://hc.bookmarksfly.cn

O. 并发与异步
来源：http://se.shtwfgs.cn

================================================================================
来源：http://ag.lnxyls.cn

[O01] 启动一个线程
来源：http://xi.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kr.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nq.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ku.nszjky.cn

TS:   // 同 JS
来源：http://mo.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://fo.9csxet.cn

Go:   go f()
来源：http://xl.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://gk.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://dr.yuexingan06.cn

[O02] 使用线程池
来源：http://ph.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mx.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ip.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://yb.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://vs.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tm.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jr.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oc.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vz.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://cf.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://jh.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://dr.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cd.gzmigu.cn

TS:   // 同 JS
来源：http://ip.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://em.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fb.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hj.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://eu.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://vl.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://zh.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hf.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://xu.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gt.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jv.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ti.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mx.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://av.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://tb.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://ek.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tx.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://lw.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://lw.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ny.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wx.szsharing.cn

Ruby: threads.map(&:join)
来源：http://gh.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ad.huanxung.cn

[O06] 使用进程池
来源：http://db.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hq.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yb.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://td.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://da.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nl.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fr.hnjuh.cn

Ruby: // fork 块
来源：http://gk.panjiajie.cn

C#:   Parallel.For
来源：http://xz.shtwfgs.cn

================================================================================
来源：http://sw.nszjky.cn

P. 常用工具函数
来源：http://dn.9csxet.cn

================================================================================
来源：http://ce.szsharing.cn

[P01] 生成 UUID
来源：http://zm.521024.cn

Py:   str(uuid.uuid4())
来源：http://ab.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://av.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://xw.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://ct.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://is.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://yb.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://gc.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://xh.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://tn.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hs.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aq.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jq.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uo.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oz.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://du.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://df.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xr.panjiajie.cn

[P03] 生成短随机字符串
来源：http://xs.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uz.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ui.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zy.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wk.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xp.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rc.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xm.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rf.hahajie.cn

[P04] 求长度
来源：http://mh.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gj.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mo.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ml.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ly.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://zy.hahajie.cn

Go:   len(arr);  len(m)
来源：http://ut.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://zk.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ab.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://xa.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lf.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ux.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hq.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aq.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dt.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gc.nszjky.cn

Ruby: a == b
来源：http://zh.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jp.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nz.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dw.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://aa.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ow.bjjhwx.cn

TS:   if (x == null) {}
来源：http://au.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fe.wgjwhj.cn

Go:   if x == nil {}
来源：http://ul.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vh.shxzskj.cn

C#:   if (x is null) {}
来源：http://ev.newstarts.cn

[P07] 防抖与节流
来源：http://qh.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fd.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://fl.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tg.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qw.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nr.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ld.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ut.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fp.nicolike.cn

[P08] 处理浮点精度问题
来源：http://le.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://il.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xz.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qz.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jb.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://np.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qa.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ak.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yt.9csxet.cn

================================================================================
来源：http://dw.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://he.shxzskj.cn

================================================================================
来源：http://of.hnjuh.cn

[Q01] 创建表
来源：http://ry.huixinmuqiang.cn

CREATE TABLE users (
来源：http://xh.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ny.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://gs.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://py.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fd.huixinmuqiang.cn

);
来源：http://bm.colortex.cn

[Q02] 创建带外键的表
来源：http://rs.chemitech.net.cn

CREATE TABLE orders (
来源：http://fn.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ul.szxytkj.cn

user_id INT NOT NULL,
来源：http://cn.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://he.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fi.hnjuh.cn

);
来源：http://zs.szsharing.cn

[Q03] 增加列
来源：http://bz.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yf.colortex.cn

[Q04] 修改列类型
来源：http://xm.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://on.wgjwhj.cn

[Q05] 重命名列
来源：http://yw.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mq.colortex.cn

[Q06] 删除列
来源：http://xl.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eh.shxzskj.cn

[Q07] 删除表
来源：http://uk.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://jo.newstarts.cn

[Q08] 创建普通索引
来源：http://ke.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yy.colortex.cn

[Q09] 创建唯一索引
来源：http://ku.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://li.huanxung.cn

[Q10] 插入单行
来源：http://fn.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zl.hnjuh.cn

[Q11] 一次插入多行
来源：http://oy.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hx.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://iq.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ly.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zd.lnxyls.cn

[Q13] 忽略重复插入
来源：http://yw.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ym.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://ml.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://je.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://id.huanxung.cn

[Q15] 查询全部
来源：http://qu.521024.cn

SELECT * FROM users;
来源：http://fu.newstarts.cn

[Q16] 查询指定列
来源：http://be.huanxung.cn

SELECT id, name FROM users;
来源：http://gd.haigaiapp.cn

[Q17] 条件查询
来源：http://jk.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ct.shxzskj.cn

[Q18] 模糊匹配
来源：http://jn.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ug.nszjky.cn

[Q19] 范围查询
来源：http://zo.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://by.shtwfgs.cn

[Q20] IN 列表
来源：http://eq.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iv.huixiangedu.cn

[Q21] 空值判断
来源：http://vx.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tg.haigaiapp.cn

[Q22] 排序
来源：http://vu.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sr.shtwfgs.cn

[Q23] 分页
来源：http://sw.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://at.bjjhwx.cn

[Q24] 去重
来源：http://et.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://ic.nicolike.cn

[Q25] 只取前 N 条
来源：http://wo.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zi.colortex.cn

[Q26] 计数
来源：http://ew.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://qw.huixiangedu.cn

[Q27] 条件计数
来源：http://bc.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nb.szxytkj.cn

[Q28] 求和与平均
来源：http://ru.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hg.shxzukj.cn

[Q29] 最大最小值
来源：http://bp.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zn.jctech888.com.cn

[Q30] 分组统计
来源：http://wa.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ux.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://bk.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bw.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://jw.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rw.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sc.hahajie.cn

[Q33] 多列分组
来源：http://ie.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zg.haigaiapp.cn

[Q34] 每组取第一条
来源：http://nh.szsharing.cn

SELECT * FROM (
来源：http://in.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lf.yuexingan06.cn

) t WHERE rn = 1;
来源：http://il.521024.cn

[Q35] 内连接
来源：http://jf.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pi.521024.cn

[Q36] 左连接
来源：http://sc.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kz.bjjhwx.cn

[Q37] 右连接
来源：http://cz.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ss.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rk.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wd.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://or.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cu.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fe.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ij.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oe.bookmarksfly.cn

[Q41] 多表连接
来源：http://ci.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ls.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://ue.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://vx.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://hf.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://ce.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ns.521024.cn

[Q43] 标量子查询
来源：http://is.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://in.521024.cn

[Q44] IN 子查询
来源：http://va.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ej.colortex.cn

[Q45] EXISTS 判断存在
来源：http://bm.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jv.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ar.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://us.huanxung.cn

[Q47] 与平均值比较
来源：http://iy.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qn.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://du.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://og.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://mp.lnxyls.cn

[Q49] 更新单行
来源：http://rt.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://de.huixinmuqiang.cn

[Q50] 批量更新
来源：http://yb.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kg.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://ct.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ad.gzmigu.cn

[Q52] 删除指定行
来源：http://hr.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://kr.haigaiapp.cn

[Q53] 按条件删除
来源：http://dm.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lv.nicolike.cn

[Q54] 清空表
来源：http://vm.nicolike.cn

TRUNCATE TABLE logs;
来源：http://ca.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://ss.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ll.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://zr.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://at.szxytkj.cn

[Q57] 行号
来源：http://mw.jctech888.com.cn


<!-- 参考信息 -->