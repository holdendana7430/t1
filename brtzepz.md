代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bn.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uy.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://zd.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gf.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ag.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ca.nszjky.cn

[N11] 二叉树中序遍历
来源：http://qe.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fi.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://wq.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ny.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hl.colortex.cn

Java: // 手写递归
来源：http://wq.shxzskj.cn

Go:   // 手写递归
来源：http://on.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hf.9csxet.cn

C#:   // 手写递归
来源：http://zb.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tn.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sc.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nc.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jy.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ki.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tb.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ne.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ig.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jv.wgjwhj.cn

================================================================================
来源：http://rp.panjiajie.cn

O. 并发与异步
来源：http://bx.huixinmuqiang.cn

================================================================================
来源：http://vq.9csxet.cn

[O01] 启动一个线程
来源：http://qa.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xs.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rz.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bx.colortex.cn

TS:   // 同 JS
来源：http://dt.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://jr.huixiangedu.cn

Go:   go f()
来源：http://se.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://eg.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://vm.nszjky.cn

[O02] 使用线程池
来源：http://it.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qz.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lb.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://zo.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://ec.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zh.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xu.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mk.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ld.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://jv.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://ll.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://vk.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ln.gzmigu.cn

TS:   // 同 JS
来源：http://on.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://ty.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uo.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qz.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://ec.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://gj.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://qf.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qt.521024.cn

JS:   async function f() { await g(); }
来源：http://un.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zr.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gc.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pn.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yn.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://kc.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://mc.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://ob.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dd.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://hm.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://vw.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ka.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uh.nicolike.cn

Ruby: threads.map(&:join)
来源：http://va.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tt.huixinmuqiang.cn

[O06] 使用进程池
来源：http://iu.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ja.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iv.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://tx.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://up.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yc.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wk.huixiangedu.cn

Ruby: // fork 块
来源：http://td.jctech888.com.cn

C#:   Parallel.For
来源：http://mi.szsharing.cn

================================================================================
来源：http://or.nicolike.cn

P. 常用工具函数
来源：http://lm.521024.cn

================================================================================
来源：http://fs.shtwfgs.cn

[P01] 生成 UUID
来源：http://ke.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://sr.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ay.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://fr.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://vf.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://cu.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://wm.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://nn.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://lu.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://bz.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lj.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vq.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gu.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gy.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gx.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wn.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jc.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ja.panjiajie.cn

[P03] 生成短随机字符串
来源：http://aq.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xt.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jt.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bo.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oq.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ko.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bz.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jh.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gl.nszjky.cn

[P04] 求长度
来源：http://su.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sa.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tt.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jw.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dd.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://oq.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://ua.9csxet.cn

Ruby: x.length;  x.size
来源：http://az.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bz.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://vz.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sk.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://do.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ox.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fr.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://he.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lq.yuntaijiaju.cn

Ruby: a == b
来源：http://hz.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xx.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kp.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ja.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://pk.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pd.newstarts.cn

TS:   if (x == null) {}
来源：http://xq.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://re.hnjuh.cn

Go:   if x == nil {}
来源：http://pc.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lh.9csxet.cn

C#:   if (x is null) {}
来源：http://vq.szsharing.cn

[P07] 防抖与节流
来源：http://uc.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fx.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://hj.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yz.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gw.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vq.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ct.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fa.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wb.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://il.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ec.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lk.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ml.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ny.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rf.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nh.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ez.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://od.huixiangedu.cn

================================================================================
来源：http://of.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ue.huixinmuqiang.cn

================================================================================
来源：http://mu.jctech888.com.cn

[Q01] 创建表
来源：http://ds.9csxet.cn

CREATE TABLE users (
来源：http://mu.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xg.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://ww.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://ev.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qo.haigaiapp.cn

);
来源：http://jg.szxytkj.cn

[Q02] 创建带外键的表
来源：http://qa.bjjhwx.cn

CREATE TABLE orders (
来源：http://ox.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uq.huanxung.cn

user_id INT NOT NULL,
来源：http://ga.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://wt.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fk.chemitech.net.cn

);
来源：http://ns.wgjwhj.cn

[Q03] 增加列
来源：http://vj.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gr.panjiajie.cn

[Q04] 修改列类型
来源：http://aj.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lb.newstarts.cn

[Q05] 重命名列
来源：http://yb.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://do.yuexingan06.cn

[Q06] 删除列
来源：http://hd.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://af.huanxung.cn

[Q07] 删除表
来源：http://me.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://pp.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://lh.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qk.colortex.cn

[Q09] 创建唯一索引
来源：http://qt.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wq.muxihuayi.cn

[Q10] 插入单行
来源：http://wd.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kb.bjjhwx.cn

[Q11] 一次插入多行
来源：http://yj.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ts.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://gy.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ni.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kg.521024.cn

[Q13] 忽略重复插入
来源：http://zs.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rd.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://sd.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ih.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ib.hahajie.cn

[Q15] 查询全部
来源：http://eo.szxytkj.cn

SELECT * FROM users;
来源：http://vw.huixiangedu.cn

[Q16] 查询指定列
来源：http://tn.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://wx.asd995.cn

[Q17] 条件查询
来源：http://ip.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vc.hnjuh.cn

[Q18] 模糊匹配
来源：http://sl.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xs.huanxung.cn

[Q19] 范围查询
来源：http://rz.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ye.chemitech.net.cn

[Q20] IN 列表
来源：http://se.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tv.shtwfgs.cn

[Q21] 空值判断
来源：http://py.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wa.szsharing.cn

[Q22] 排序
来源：http://ub.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lw.bookmarksfly.cn

[Q23] 分页
来源：http://sb.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hn.hnjuh.cn

[Q24] 去重
来源：http://pn.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://cz.panjiajie.cn

[Q25] 只取前 N 条
来源：http://bt.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wp.colortex.cn

[Q26] 计数
来源：http://pc.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://ui.nicolike.cn

[Q27] 条件计数
来源：http://ad.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gx.muxihuayi.cn

[Q28] 求和与平均
来源：http://qz.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uv.newstarts.cn

[Q29] 最大最小值
来源：http://he.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hn.shxzskj.cn

[Q30] 分组统计
来源：http://pp.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bd.gzmigu.cn

[Q31] 分组后过滤
来源：http://oq.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ve.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://dd.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nt.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nk.gzmigu.cn

[Q33] 多列分组
来源：http://wf.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mt.panjiajie.cn

[Q34] 每组取第一条
来源：http://bk.wgjwhj.cn

SELECT * FROM (
来源：http://eg.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://se.chemitech.net.cn

) t WHERE rn = 1;
来源：http://cg.shtwfgs.cn

[Q35] 内连接
来源：http://ab.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ig.asd995.cn

[Q36] 左连接
来源：http://hc.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dm.newstarts.cn

[Q37] 右连接
来源：http://ns.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wj.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gu.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bs.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://er.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bf.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cy.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qs.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wb.huixinmuqiang.cn

[Q41] 多表连接
来源：http://is.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hg.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://tv.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://tg.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://nb.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://fo.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ge.jctech888.com.cn

[Q43] 标量子查询
来源：http://ah.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bb.szsharing.cn

[Q44] IN 子查询
来源：http://gk.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wq.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://wb.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dq.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ue.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eq.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://xy.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jt.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://pq.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bt.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://fw.huanxung.cn

[Q49] 更新单行
来源：http://ld.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lj.huixinmuqiang.cn

[Q50] 批量更新
来源：http://hu.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kd.nicolike.cn

[Q51] 用子查询更新
来源：http://mv.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uu.hnjuh.cn

[Q52] 删除指定行
来源：http://rx.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://bs.wgjwhj.cn

[Q53] 按条件删除
来源：http://ew.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xb.bjjhwx.cn

[Q54] 清空表
来源：http://rn.asd995.cn

TRUNCATE TABLE logs;
来源：http://ls.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://ga.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uq.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://hh.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vs.bookmarksfly.cn

[Q57] 行号
来源：http://bp.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uf.newstarts.cn

[Q58] 累计求和
来源：http://jg.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://my.muxihuayi.cn

[Q59] 分组内累计
来源：http://cs.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lg.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ar.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gn.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hv.hnjuh.cn


<!-- 参考信息 -->