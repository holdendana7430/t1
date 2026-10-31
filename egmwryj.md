代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kg.bookmarksfly.cn

[N10] 链表节点定义
来源：http://sh.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hv.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://me.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ca.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lj.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://kb.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://px.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vd.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uu.asd995.cn

[N11] 二叉树中序遍历
来源：http://og.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yu.newstarts.cn

PHP:  // 手写递归函数
来源：http://cm.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tf.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zj.jianghongdianzi.cn

Java: // 手写递归
来源：http://dl.haigaiapp.cn

Go:   // 手写递归
来源：http://bw.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ko.yuexingan06.cn

C#:   // 手写递归
来源：http://br.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bu.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ar.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://td.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cx.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ag.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qm.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jb.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dz.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kg.yuexingan06.cn

================================================================================
来源：http://rs.szxytkj.cn

O. 并发与异步
来源：http://jb.gzmigu.cn

================================================================================
来源：http://kg.jctech888.com.cn

[O01] 启动一个线程
来源：http://hn.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kj.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yp.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vq.haigaiapp.cn

TS:   // 同 JS
来源：http://ji.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://ej.haigaiapp.cn

Go:   go f()
来源：http://ub.gzmigu.cn

Ruby: Thread.new { f }
来源：http://gd.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://dp.nicolike.cn

[O02] 使用线程池
来源：http://sc.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://us.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wd.asd995.cn

JS:   // worker_threads 线程池
来源：http://bo.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://ea.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ts.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ni.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fx.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://et.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://li.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://uc.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://wr.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tz.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ef.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://lc.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pj.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mk.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ab.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://pa.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://if.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pf.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://jl.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bz.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pw.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pf.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://my.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://jm.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://mv.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://vz.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pr.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://qx.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://ta.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://il.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tr.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://hp.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kn.gzmigu.cn

[O06] 使用进程池
来源：http://be.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nm.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cq.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://of.521024.cn

TS:   // child_process / cluster 模块
来源：http://qd.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tm.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dv.gzmigu.cn

Ruby: // fork 块
来源：http://te.asd995.cn

C#:   Parallel.For
来源：http://kw.9csxet.cn

================================================================================
来源：http://ra.muxihuayi.cn

P. 常用工具函数
来源：http://fj.szxytkj.cn

================================================================================
来源：http://va.huixiangedu.cn

[P01] 生成 UUID
来源：http://vk.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://yq.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aq.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://xh.colortex.cn

TS:   crypto.randomUUID()
来源：http://vw.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://fz.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://md.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://ik.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://hp.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://na.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kr.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://si.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kn.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ba.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pb.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jo.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cy.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://st.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://on.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gu.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pv.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hw.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hq.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://od.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fl.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aa.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ks.shxzskj.cn

[P04] 求长度
来源：http://fz.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://te.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bi.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oe.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://we.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://tj.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://fp.szxytkj.cn

Ruby: x.length;  x.size
来源：http://fo.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gv.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ej.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rn.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vv.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gf.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ub.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eq.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ql.shtwfgs.cn

Ruby: a == b
来源：http://rs.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xh.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gt.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ue.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://nu.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tm.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://zk.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ix.bjjhwx.cn

Go:   if x == nil {}
来源：http://mg.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mb.colortex.cn

C#:   if (x is null) {}
来源：http://wn.huixiangedu.cn

[P07] 防抖与节流
来源：http://sd.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wh.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://lo.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oz.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tk.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wa.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vq.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zr.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mb.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://tu.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bu.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ra.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cv.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://md.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vu.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tn.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tw.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ff.jctech888.com.cn

================================================================================
来源：http://lu.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fk.hnjuh.cn

================================================================================
来源：http://ac.huixinmuqiang.cn

[Q01] 创建表
来源：http://mg.shxzukj.cn

CREATE TABLE users (
来源：http://rh.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ij.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://lu.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://vf.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ca.panjiajie.cn

);
来源：http://rz.shxzskj.cn

[Q02] 创建带外键的表
来源：http://kv.panjiajie.cn

CREATE TABLE orders (
来源：http://mj.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mt.hahajie.cn

user_id INT NOT NULL,
来源：http://tc.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://jl.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://og.huixinmuqiang.cn

);
来源：http://yp.huixinmuqiang.cn

[Q03] 增加列
来源：http://do.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ko.nszjky.cn

[Q04] 修改列类型
来源：http://ih.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gi.yuexingan06.cn

[Q05] 重命名列
来源：http://jz.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jm.huixiangedu.cn

[Q06] 删除列
来源：http://ys.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ig.bjjhwx.cn

[Q07] 删除表
来源：http://wg.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://zn.szxytkj.cn

[Q08] 创建普通索引
来源：http://qy.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xp.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://bi.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ls.huixinmuqiang.cn

[Q10] 插入单行
来源：http://xi.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sv.shxzskj.cn

[Q11] 一次插入多行
来源：http://gz.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mw.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://qh.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fc.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ct.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://hy.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://me.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://in.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dk.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lj.huanxung.cn

[Q15] 查询全部
来源：http://fh.shtwfgs.cn

SELECT * FROM users;
来源：http://ej.bookmarksfly.cn

[Q16] 查询指定列
来源：http://wq.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://ih.hnjuh.cn

[Q17] 条件查询
来源：http://oy.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ib.muxihuayi.cn

[Q18] 模糊匹配
来源：http://vl.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pa.chemitech.net.cn

[Q19] 范围查询
来源：http://sn.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pa.shxzukj.cn

[Q20] IN 列表
来源：http://ii.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bj.hahajie.cn

[Q21] 空值判断
来源：http://qv.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gb.szsharing.cn

[Q22] 排序
来源：http://iw.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mn.asd995.cn

[Q23] 分页
来源：http://ai.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wo.huixinmuqiang.cn

[Q24] 去重
来源：http://dx.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://yz.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://po.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wy.haigaiapp.cn

[Q26] 计数
来源：http://fw.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://ni.hnjuh.cn

[Q27] 条件计数
来源：http://uk.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://al.bjjhwx.cn

[Q28] 求和与平均
来源：http://lf.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://me.szsharing.cn

[Q29] 最大最小值
来源：http://vk.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mh.shxzskj.cn

[Q30] 分组统计
来源：http://bb.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mw.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://jf.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bh.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://za.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ur.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mh.huixiangedu.cn

[Q33] 多列分组
来源：http://vc.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sy.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ji.muxihuayi.cn

SELECT * FROM (
来源：http://fx.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ao.colortex.cn

) t WHERE rn = 1;
来源：http://qe.yuexingan06.cn

[Q35] 内连接
来源：http://ug.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wf.huixiangedu.cn

[Q36] 左连接
来源：http://hy.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bw.asd995.cn

[Q37] 右连接
来源：http://mk.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ef.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xo.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://al.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://pi.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hw.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ir.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pj.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uk.yuexingan06.cn

[Q41] 多表连接
来源：http://xh.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ft.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://or.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://po.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://iz.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://nx.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lm.nicolike.cn

[Q43] 标量子查询
来源：http://xr.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ny.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://jc.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ui.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://vr.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nj.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lo.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://es.hnjuh.cn

[Q47] 与平均值比较
来源：http://jn.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bq.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://ds.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gn.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://zm.haigaiapp.cn

[Q49] 更新单行
来源：http://zu.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mx.asd995.cn

[Q50] 批量更新
来源：http://tu.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ua.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://pu.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ss.colortex.cn

[Q52] 删除指定行
来源：http://lo.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://pw.colortex.cn

[Q53] 按条件删除
来源：http://cf.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zz.huanxung.cn

[Q54] 清空表
来源：http://gg.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://hd.nicolike.cn

[Q55] 排名（并列占位）
来源：http://gt.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ok.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://ap.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sj.gzmigu.cn

[Q57] 行号
来源：http://mj.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kh.szxytkj.cn

[Q58] 累计求和
来源：http://pd.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kr.jctech888.com.cn

[Q59] 分组内累计
来源：http://wq.wgjwhj.cn


<!-- 参考信息 -->