代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://id.colortex.cn

[N10] 链表节点定义
来源：http://sg.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ik.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ln.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kg.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zf.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://sz.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://za.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hl.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uh.szsharing.cn

[N11] 二叉树中序遍历
来源：http://xt.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gz.9csxet.cn

PHP:  // 手写递归函数
来源：http://jp.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nz.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yj.shtwfgs.cn

Java: // 手写递归
来源：http://nl.jctech888.com.cn

Go:   // 手写递归
来源：http://ia.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zx.muxihuayi.cn

C#:   // 手写递归
来源：http://dg.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://co.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ol.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xb.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://io.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wy.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tc.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vb.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cy.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gw.521024.cn

================================================================================
来源：http://oe.521024.cn

O. 并发与异步
来源：http://qu.jianghongdianzi.cn

================================================================================
来源：http://et.yuexingan06.cn

[O01] 启动一个线程
来源：http://ev.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cy.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ac.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qo.jctech888.com.cn

TS:   // 同 JS
来源：http://ut.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://qc.bjjhwx.cn

Go:   go f()
来源：http://fu.9csxet.cn

Ruby: Thread.new { f }
来源：http://ko.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://pi.hnjuh.cn

[O02] 使用线程池
来源：http://kx.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mo.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hs.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://fa.521024.cn

TS:   // worker_threads 线程池
来源：http://dl.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tr.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://je.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://do.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://he.hahajie.cn

[O03] 加锁保护共享数据
来源：http://bm.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://pb.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fu.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dh.huanxung.cn

TS:   // 同 JS
来源：http://tz.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://lb.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ti.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pf.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://zh.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://yw.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://ob.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cs.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://kh.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ez.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qx.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ow.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ei.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://zh.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://sd.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://cx.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yk.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://yi.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://ar.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vg.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rs.huanxung.cn

Ruby: threads.map(&:join)
来源：http://ff.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ze.521024.cn

[O06] 使用进程池
来源：http://ln.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yy.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gu.colortex.cn

JS:   // child_process / cluster 模块
来源：http://li.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://zh.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mg.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nd.yuexingan06.cn

Ruby: // fork 块
来源：http://kc.shtwfgs.cn

C#:   Parallel.For
来源：http://sh.bookmarksfly.cn

================================================================================
来源：http://qh.bookmarksfly.cn

P. 常用工具函数
来源：http://hg.hnjuh.cn

================================================================================
来源：http://it.bjjhwx.cn

[P01] 生成 UUID
来源：http://zl.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://rg.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ro.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://xo.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://xi.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://ol.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://mw.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://sp.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://ej.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://kz.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dm.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ya.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vj.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ai.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ck.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hc.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wm.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://st.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://tm.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hv.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ta.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://th.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nx.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fy.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://py.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ic.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lg.huanxung.cn

[P04] 求长度
来源：http://qk.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rp.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bl.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wd.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://io.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://ev.521024.cn

Go:   len(arr);  len(m)
来源：http://gq.szsharing.cn

Ruby: x.length;  x.size
来源：http://ie.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://po.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://kj.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://af.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tc.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ym.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cv.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vt.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jw.szxytkj.cn

Ruby: a == b
来源：http://lc.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iy.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ef.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pg.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://lk.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rp.yuexingan06.cn

TS:   if (x == null) {}
来源：http://ro.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://of.wgjwhj.cn

Go:   if x == nil {}
来源：http://pr.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ch.shxzukj.cn

C#:   if (x is null) {}
来源：http://mn.yuexingan06.cn

[P07] 防抖与节流
来源：http://cc.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oy.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://ho.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://on.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kk.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wf.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yr.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zj.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://og.colortex.cn

[P08] 处理浮点精度问题
来源：http://yo.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xj.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ez.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cy.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qk.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pa.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hm.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cv.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uo.jctech888.com.cn

================================================================================
来源：http://fs.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sp.shtwfgs.cn

================================================================================
来源：http://bp.haigaiapp.cn

[Q01] 创建表
来源：http://sc.asd995.cn

CREATE TABLE users (
来源：http://ks.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zi.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://tb.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://xp.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tn.szsharing.cn

);
来源：http://yu.9csxet.cn

[Q02] 创建带外键的表
来源：http://de.szsharing.cn

CREATE TABLE orders (
来源：http://if.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wb.bjjhwx.cn

user_id INT NOT NULL,
来源：http://fa.hahajie.cn

amount DECIMAL(10, 2),
来源：http://yp.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ib.yuntaijiaju.cn

);
来源：http://xr.yuexingan06.cn

[Q03] 增加列
来源：http://zx.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qz.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://ka.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ka.gzmigu.cn

[Q05] 重命名列
来源：http://sl.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gh.jianghongdianzi.cn

[Q06] 删除列
来源：http://js.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://am.lnxyls.cn

[Q07] 删除表
来源：http://nd.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://qz.gzmigu.cn

[Q08] 创建普通索引
来源：http://dy.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qt.9csxet.cn

[Q09] 创建唯一索引
来源：http://ro.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ax.hahajie.cn

[Q10] 插入单行
来源：http://jn.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hn.nicolike.cn

[Q11] 一次插入多行
来源：http://lb.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sd.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://mn.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fw.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ww.nicolike.cn

[Q13] 忽略重复插入
来源：http://mf.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qs.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://up.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sk.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ru.szsharing.cn

[Q15] 查询全部
来源：http://zi.shxzukj.cn

SELECT * FROM users;
来源：http://rx.newstarts.cn

[Q16] 查询指定列
来源：http://si.hnjuh.cn

SELECT id, name FROM users;
来源：http://hd.chemitech.net.cn

[Q17] 条件查询
来源：http://ea.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://it.9csxet.cn

[Q18] 模糊匹配
来源：http://os.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tg.yuexingan06.cn

[Q19] 范围查询
来源：http://ny.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nc.lnxyls.cn

[Q20] IN 列表
来源：http://rd.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tg.colortex.cn

[Q21] 空值判断
来源：http://aa.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://th.nszjky.cn

[Q22] 排序
来源：http://id.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://am.jctech888.com.cn

[Q23] 分页
来源：http://iv.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://db.yuexingan06.cn

[Q24] 去重
来源：http://jp.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://yc.shxzukj.cn

[Q25] 只取前 N 条
来源：http://fu.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fy.nicolike.cn

[Q26] 计数
来源：http://ej.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://mk.muxihuayi.cn

[Q27] 条件计数
来源：http://rd.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kx.nicolike.cn

[Q28] 求和与平均
来源：http://vr.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fl.asd995.cn

[Q29] 最大最小值
来源：http://pc.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jm.jctech888.com.cn

[Q30] 分组统计
来源：http://ez.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ny.haigaiapp.cn

[Q31] 分组后过滤
来源：http://fg.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zb.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://kp.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eq.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aj.muxihuayi.cn

[Q33] 多列分组
来源：http://ns.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pn.nszjky.cn

[Q34] 每组取第一条
来源：http://av.colortex.cn

SELECT * FROM (
来源：http://se.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qy.521024.cn

) t WHERE rn = 1;
来源：http://ez.bookmarksfly.cn

[Q35] 内连接
来源：http://ad.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hv.jianghongdianzi.cn

[Q36] 左连接
来源：http://zc.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iq.colortex.cn

[Q37] 右连接
来源：http://va.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gi.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bt.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sh.asd995.cn

[Q39] 自连接（查上下级）
来源：http://jq.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cj.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ml.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://co.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dq.yuexingan06.cn

[Q41] 多表连接
来源：http://id.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sm.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://qc.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://by.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://np.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://wn.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xw.huixiangedu.cn

[Q43] 标量子查询
来源：http://zg.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hx.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://lh.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jm.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://hx.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cn.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zh.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pu.jctech888.com.cn

[Q47] 与平均值比较
来源：http://fx.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mp.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://rv.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hd.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://zw.jctech888.com.cn

[Q49] 更新单行
来源：http://qm.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qn.haigaiapp.cn

[Q50] 批量更新
来源：http://wh.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ho.hahajie.cn

[Q51] 用子查询更新
来源：http://im.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nh.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://or.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://uw.newstarts.cn

[Q53] 按条件删除
来源：http://ds.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eh.9csxet.cn

[Q54] 清空表
来源：http://fn.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://bw.nicolike.cn

[Q55] 排名（并列占位）
来源：http://ge.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fy.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://ya.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fu.asd995.cn

[Q57] 行号
来源：http://uy.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ws.chemitech.net.cn

[Q58] 累计求和
来源：http://qt.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rr.hnjuh.cn

[Q59] 分组内累计
来源：http://sf.nicolike.cn


<!-- 参考信息 -->