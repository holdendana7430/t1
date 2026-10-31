代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jp.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hp.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nw.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ny.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oa.szsharing.cn

[N10] 链表节点定义
来源：http://mu.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gc.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wg.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tz.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fb.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://ib.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lv.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mj.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sc.szsharing.cn

[N11] 二叉树中序遍历
来源：http://sy.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hd.gzmigu.cn

PHP:  // 手写递归函数
来源：http://br.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://um.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ex.bookmarksfly.cn

Java: // 手写递归
来源：http://iz.panjiajie.cn

Go:   // 手写递归
来源：http://kl.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ef.yuexingan06.cn

C#:   // 手写递归
来源：http://kf.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ff.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zh.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uk.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ve.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://je.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nz.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hy.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://al.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lv.chemitech.net.cn

================================================================================
来源：http://hv.jianghongdianzi.cn

O. 并发与异步
来源：http://ch.panjiajie.cn

================================================================================
来源：http://fg.szsharing.cn

[O01] 启动一个线程
来源：http://ul.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zb.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ri.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yu.wgjwhj.cn

TS:   // 同 JS
来源：http://ff.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://ht.huanxung.cn

Go:   go f()
来源：http://tw.hnjuh.cn

Ruby: Thread.new { f }
来源：http://mn.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://js.panjiajie.cn

[O02] 使用线程池
来源：http://ji.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://au.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pc.nszjky.cn

JS:   // worker_threads 线程池
来源：http://oh.nszjky.cn

TS:   // worker_threads 线程池
来源：http://iu.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wq.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ts.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://na.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ti.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://cd.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://fg.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://as.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nj.haigaiapp.cn

TS:   // 同 JS
来源：http://hy.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://fq.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ka.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jj.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://sv.hahajie.cn

[O04] 定义异步函数并等待
来源：http://hm.colortex.cn

Py:   async def f():⏎    await g()
来源：http://kz.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nb.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://fk.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://es.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ig.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tq.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xh.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://ng.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://wr.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://hx.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jp.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://wn.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://uy.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zx.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jk.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://ly.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zw.wgjwhj.cn

[O06] 使用进程池
来源：http://va.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lz.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hc.521024.cn

JS:   // child_process / cluster 模块
来源：http://zi.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://qw.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zd.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cy.yuntaijiaju.cn

Ruby: // fork 块
来源：http://yd.bookmarksfly.cn

C#:   Parallel.For
来源：http://kd.huanxung.cn

================================================================================
来源：http://af.bjjhwx.cn

P. 常用工具函数
来源：http://nh.gzmigu.cn

================================================================================
来源：http://zb.gzmigu.cn

[P01] 生成 UUID
来源：http://ff.521024.cn

Py:   str(uuid.uuid4())
来源：http://gl.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ti.szsharing.cn

JS:   crypto.randomUUID()
来源：http://gx.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://xu.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://lv.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://to.asd995.cn

Ruby: SecureRandom.uuid
来源：http://no.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://bx.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://jj.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bs.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qy.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yk.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zt.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vi.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gv.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bo.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vb.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://kn.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xd.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rk.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hn.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ib.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uk.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bf.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vs.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fl.wgjwhj.cn

[P04] 求长度
来源：http://mj.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ie.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ij.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wf.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ql.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://zr.colortex.cn

Go:   len(arr);  len(m)
来源：http://ae.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://su.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pe.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://se.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xr.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://op.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dt.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xw.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dx.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cj.huanxung.cn

Ruby: a == b
来源：http://xs.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xp.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ro.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://va.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://ui.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fz.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://ms.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zu.gzmigu.cn

Go:   if x == nil {}
来源：http://og.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tq.shxzukj.cn

C#:   if (x is null) {}
来源：http://pw.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://qi.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jf.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://zq.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mh.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rd.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mm.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ym.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://je.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vb.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://ti.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xv.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eu.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wh.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dc.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xe.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fj.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rw.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iq.shxzskj.cn

================================================================================
来源：http://ej.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://of.huixinmuqiang.cn

================================================================================
来源：http://wi.nicolike.cn

[Q01] 创建表
来源：http://fo.nicolike.cn

CREATE TABLE users (
来源：http://qh.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cj.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://bx.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://vg.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ue.szxytkj.cn

);
来源：http://ex.panjiajie.cn

[Q02] 创建带外键的表
来源：http://ma.nszjky.cn

CREATE TABLE orders (
来源：http://ju.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://un.chemitech.net.cn

user_id INT NOT NULL,
来源：http://lf.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://oy.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nv.hahajie.cn

);
来源：http://fj.gzmigu.cn

[Q03] 增加列
来源：http://vz.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ye.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://ao.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ws.newstarts.cn

[Q05] 重命名列
来源：http://fx.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uc.gzmigu.cn

[Q06] 删除列
来源：http://zr.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dw.huanxung.cn

[Q07] 删除表
来源：http://zf.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://xd.wgjwhj.cn

[Q08] 创建普通索引
来源：http://ad.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lr.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://yx.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nt.yuntaijiaju.cn

[Q10] 插入单行
来源：http://uk.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ot.muxihuayi.cn

[Q11] 一次插入多行
来源：http://tp.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yw.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://ug.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uv.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ke.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://nk.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kx.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://fe.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wl.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sm.newstarts.cn

[Q15] 查询全部
来源：http://id.yuntaijiaju.cn

SELECT * FROM users;
来源：http://sh.newstarts.cn

[Q16] 查询指定列
来源：http://jf.newstarts.cn

SELECT id, name FROM users;
来源：http://lw.shtwfgs.cn

[Q17] 条件查询
来源：http://st.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pa.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://pz.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ud.wgjwhj.cn

[Q19] 范围查询
来源：http://eh.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dx.colortex.cn

[Q20] IN 列表
来源：http://bm.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sg.wgjwhj.cn

[Q21] 空值判断
来源：http://bs.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://de.huanxung.cn

[Q22] 排序
来源：http://io.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uz.lnxyls.cn

[Q23] 分页
来源：http://co.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jo.shxzskj.cn

[Q24] 去重
来源：http://xl.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://vr.huanxung.cn

[Q25] 只取前 N 条
来源：http://ab.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fj.jianghongdianzi.cn

[Q26] 计数
来源：http://fi.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://ou.chemitech.net.cn

[Q27] 条件计数
来源：http://mn.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zp.yuexingan06.cn

[Q28] 求和与平均
来源：http://mw.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fp.huixiangedu.cn

[Q29] 最大最小值
来源：http://zl.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fg.lnxyls.cn

[Q30] 分组统计
来源：http://ea.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wr.panjiajie.cn

[Q31] 分组后过滤
来源：http://kf.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fn.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://kr.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kd.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://to.asd995.cn

[Q33] 多列分组
来源：http://bf.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fg.gzmigu.cn

[Q34] 每组取第一条
来源：http://vo.nicolike.cn

SELECT * FROM (
来源：http://rk.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jh.asd995.cn

) t WHERE rn = 1;
来源：http://bt.huanxung.cn

[Q35] 内连接
来源：http://su.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gc.bjjhwx.cn

[Q36] 左连接
来源：http://wk.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cu.haigaiapp.cn

[Q37] 右连接
来源：http://cf.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jf.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://or.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hg.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://kt.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://es.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ma.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ag.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://my.nszjky.cn

[Q41] 多表连接
来源：http://ne.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ic.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://fq.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://km.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://fz.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://bu.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cr.hnjuh.cn

[Q43] 标量子查询
来源：http://an.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tz.521024.cn

[Q44] IN 子查询
来源：http://pe.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oj.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://yt.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ms.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://df.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ve.asd995.cn

[Q47] 与平均值比较
来源：http://vz.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zc.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://iu.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ou.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://uk.szxytkj.cn

[Q49] 更新单行
来源：http://nk.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ut.panjiajie.cn

[Q50] 批量更新
来源：http://ib.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ld.asd995.cn

[Q51] 用子查询更新
来源：http://nr.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tu.lnxyls.cn

[Q52] 删除指定行
来源：http://ni.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://nx.haigaiapp.cn

[Q53] 按条件删除
来源：http://ag.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bs.chemitech.net.cn

[Q54] 清空表
来源：http://oh.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://mh.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://zl.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ml.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://ig.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fa.hnjuh.cn

[Q57] 行号
来源：http://ms.9csxet.cn


<!-- 参考信息 -->