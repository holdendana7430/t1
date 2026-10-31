代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://sh.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cp.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://mh.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hu.asd995.cn

PHP:  // 手写递归函数
来源：http://vy.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cl.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yz.bookmarksfly.cn

Java: // 手写递归
来源：http://rh.haigaiapp.cn

Go:   // 手写递归
来源：http://zs.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fd.nicolike.cn

C#:   // 手写递归
来源：http://jl.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yi.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://of.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vv.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cj.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pj.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hq.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kf.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ja.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sn.huixiangedu.cn

================================================================================
来源：http://wz.jianghongdianzi.cn

O. 并发与异步
来源：http://rh.panjiajie.cn

================================================================================
来源：http://oh.shxzskj.cn

[O01] 启动一个线程
来源：http://mx.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kg.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sf.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fq.521024.cn

TS:   // 同 JS
来源：http://qv.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://ix.haigaiapp.cn

Go:   go f()
来源：http://jx.nicolike.cn

Ruby: Thread.new { f }
来源：http://zk.nicolike.cn

C#:   Task.Run(() => F());
来源：http://or.colortex.cn

[O02] 使用线程池
来源：http://bv.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gs.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kq.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://le.nicolike.cn

TS:   // worker_threads 线程池
来源：http://de.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yu.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hc.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xr.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fn.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://nx.newstarts.cn

Py:   with lock: shared += 1
来源：http://tm.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://pl.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vd.bjjhwx.cn

TS:   // 同 JS
来源：http://pu.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://mx.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gz.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xu.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://bg.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://ku.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://nn.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tz.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ls.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pp.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sd.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mi.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bx.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://rx.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://ny.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://zl.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oo.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://bq.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://zz.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tz.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pw.hahajie.cn

Ruby: threads.map(&:join)
来源：http://kp.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xd.nszjky.cn

[O06] 使用进程池
来源：http://wd.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cg.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ww.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://cz.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://he.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wr.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bu.hahajie.cn

Ruby: // fork 块
来源：http://wj.yuntaijiaju.cn

C#:   Parallel.For
来源：http://na.chemitech.net.cn

================================================================================
来源：http://wp.chemitech.net.cn

P. 常用工具函数
来源：http://ac.wgjwhj.cn

================================================================================
来源：http://ze.panjiajie.cn

[P01] 生成 UUID
来源：http://aq.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://gm.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qm.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://xw.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://gx.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://tb.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://wl.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://ik.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://hx.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://aw.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jp.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rz.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jw.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vm.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lk.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qw.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ma.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://li.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://fk.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hb.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gn.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hu.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zs.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qt.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jx.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ti.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mr.asd995.cn

[P04] 求长度
来源：http://nd.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vu.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ie.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lf.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mr.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://ag.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://mm.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ze.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oq.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://pa.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bu.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ji.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ox.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bg.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cq.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://se.jctech888.com.cn

Ruby: a == b
来源：http://do.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zd.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mx.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pt.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://hl.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hp.szsharing.cn

TS:   if (x == null) {}
来源：http://bn.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zf.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://yk.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ch.chemitech.net.cn

C#:   if (x is null) {}
来源：http://um.gzmigu.cn

[P07] 防抖与节流
来源：http://vr.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qq.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://at.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ul.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yz.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wq.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rf.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rp.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jd.hahajie.cn

[P08] 处理浮点精度问题
来源：http://qb.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kr.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sz.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mg.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ta.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nm.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vn.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qe.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xj.yuexingan06.cn

================================================================================
来源：http://ll.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jh.shxzskj.cn

================================================================================
来源：http://kj.jianghongdianzi.cn

[Q01] 创建表
来源：http://tv.shxzukj.cn

CREATE TABLE users (
来源：http://pi.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ns.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://dn.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://wc.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uu.shxzskj.cn

);
来源：http://qp.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://kz.newstarts.cn

CREATE TABLE orders (
来源：http://yv.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cp.shtwfgs.cn

user_id INT NOT NULL,
来源：http://my.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://dk.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lm.chemitech.net.cn

);
来源：http://hg.shtwfgs.cn

[Q03] 增加列
来源：http://fg.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hx.huanxung.cn

[Q04] 修改列类型
来源：http://vz.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nn.szsharing.cn

[Q05] 重命名列
来源：http://ev.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vm.huanxung.cn

[Q06] 删除列
来源：http://vh.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xo.huixinmuqiang.cn

[Q07] 删除表
来源：http://fo.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://uy.asd995.cn

[Q08] 创建普通索引
来源：http://tt.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mj.colortex.cn

[Q09] 创建唯一索引
来源：http://kf.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mn.chemitech.net.cn

[Q10] 插入单行
来源：http://wt.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lu.chemitech.net.cn

[Q11] 一次插入多行
来源：http://mr.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rj.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://sa.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://co.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://se.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://ej.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zn.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://tk.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dp.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xw.huanxung.cn

[Q15] 查询全部
来源：http://pv.jianghongdianzi.cn

SELECT * FROM users;
来源：http://de.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://cb.muxihuayi.cn

SELECT id, name FROM users;
来源：http://mm.newstarts.cn

[Q17] 条件查询
来源：http://ow.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jw.huanxung.cn

[Q18] 模糊匹配
来源：http://od.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ry.yuexingan06.cn

[Q19] 范围查询
来源：http://xq.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hr.hnjuh.cn

[Q20] IN 列表
来源：http://mw.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ry.jctech888.com.cn

[Q21] 空值判断
来源：http://rz.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vl.huixinmuqiang.cn

[Q22] 排序
来源：http://eb.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qs.bjjhwx.cn

[Q23] 分页
来源：http://fp.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://we.muxihuayi.cn

[Q24] 去重
来源：http://so.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://dv.panjiajie.cn

[Q25] 只取前 N 条
来源：http://bs.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sb.muxihuayi.cn

[Q26] 计数
来源：http://tp.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://rw.huixinmuqiang.cn

[Q27] 条件计数
来源：http://cx.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ji.bjjhwx.cn

[Q28] 求和与平均
来源：http://sv.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sb.9csxet.cn

[Q29] 最大最小值
来源：http://ex.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yq.asd995.cn

[Q30] 分组统计
来源：http://lj.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jw.521024.cn

[Q31] 分组后过滤
来源：http://yw.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xx.newstarts.cn

[Q32] 分组拼接字符串
来源：http://qa.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ck.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zo.gzmigu.cn

[Q33] 多列分组
来源：http://uj.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sj.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://si.wgjwhj.cn

SELECT * FROM (
来源：http://nb.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xi.nicolike.cn

) t WHERE rn = 1;
来源：http://rd.haigaiapp.cn

[Q35] 内连接
来源：http://rb.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://da.chemitech.net.cn

[Q36] 左连接
来源：http://qz.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ha.newstarts.cn

[Q37] 右连接
来源：http://ni.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rc.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iq.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fb.521024.cn

[Q39] 自连接（查上下级）
来源：http://of.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wu.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vh.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xm.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fk.haigaiapp.cn

[Q41] 多表连接
来源：http://ki.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rf.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://ce.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://is.colortex.cn

[Q42] 连接条件附加过滤
来源：http://ek.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://iu.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ed.nicolike.cn

[Q43] 标量子查询
来源：http://um.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://es.nszjky.cn

[Q44] IN 子查询
来源：http://vn.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aq.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://gq.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://us.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gz.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cy.hnjuh.cn

[Q47] 与平均值比较
来源：http://kp.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ix.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://bf.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mh.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://xf.colortex.cn

[Q49] 更新单行
来源：http://ky.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xp.panjiajie.cn

[Q50] 批量更新
来源：http://pf.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lf.yuexingan06.cn

[Q51] 用子查询更新
来源：http://lp.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vb.muxihuayi.cn

[Q52] 删除指定行
来源：http://hu.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://us.szxytkj.cn

[Q53] 按条件删除
来源：http://zl.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xe.chemitech.net.cn

[Q54] 清空表
来源：http://lp.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://nv.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://rq.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yn.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ah.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mr.huixiangedu.cn

[Q57] 行号
来源：http://xp.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xp.newstarts.cn

[Q58] 累计求和
来源：http://ye.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://st.nicolike.cn

[Q59] 分组内累计
来源：http://pe.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sz.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://mf.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tw.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kt.huanxung.cn

[Q61] 移动平均
来源：http://jt.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wf.szxytkj.cn

[Q62] 分组占比
来源：http://rq.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ng.bookmarksfly.cn


<!-- 参考信息 -->