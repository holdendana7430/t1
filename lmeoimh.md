代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://st.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zt.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://te.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ag.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://uc.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ls.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yf.nszjky.cn

Java: // 手写递归
来源：http://gt.bookmarksfly.cn

Go:   // 手写递归
来源：http://ue.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vm.szxytkj.cn

C#:   // 手写递归
来源：http://wd.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jr.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hx.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fe.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kz.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pt.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bm.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bq.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://za.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sl.haigaiapp.cn

================================================================================
来源：http://pr.shxzskj.cn

O. 并发与异步
来源：http://eg.hahajie.cn

================================================================================
来源：http://rx.shxzskj.cn

[O01] 启动一个线程
来源：http://ho.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fh.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zt.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pl.bjjhwx.cn

TS:   // 同 JS
来源：http://qk.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://kx.wgjwhj.cn

Go:   go f()
来源：http://co.asd995.cn

Ruby: Thread.new { f }
来源：http://al.colortex.cn

C#:   Task.Run(() => F());
来源：http://tl.jianghongdianzi.cn

[O02] 使用线程池
来源：http://vz.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eh.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ah.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://sn.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://nv.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://if.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qt.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bt.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mo.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://vb.hahajie.cn

Py:   with lock: shared += 1
来源：http://ti.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://vd.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://za.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ls.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://ar.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wn.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fm.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://au.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://pa.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://cy.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vw.newstarts.cn

JS:   async function f() { await g(); }
来源：http://pz.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://st.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wc.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://my.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fb.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://kz.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://fv.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://tb.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ib.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://sa.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://ko.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gn.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cy.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://qn.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nq.shtwfgs.cn

[O06] 使用进程池
来源：http://vy.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cv.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ou.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://zg.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://lj.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vp.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zx.hahajie.cn

Ruby: // fork 块
来源：http://ns.lnxyls.cn

C#:   Parallel.For
来源：http://tn.9csxet.cn

================================================================================
来源：http://lm.shxzukj.cn

P. 常用工具函数
来源：http://wg.newstarts.cn

================================================================================
来源：http://zq.chemitech.net.cn

[P01] 生成 UUID
来源：http://av.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://sf.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jq.nszjky.cn

JS:   crypto.randomUUID()
来源：http://vy.521024.cn

TS:   crypto.randomUUID()
来源：http://po.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://gd.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://dw.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://pb.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://to.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://sl.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xe.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rf.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ur.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fh.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lf.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gd.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xt.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ai.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://db.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ht.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bq.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sy.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://va.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ob.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://up.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uv.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wz.shxzukj.cn

[P04] 求长度
来源：http://wm.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qe.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://et.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nr.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kc.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://pq.asd995.cn

Go:   len(arr);  len(m)
来源：http://vg.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://pa.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kg.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://lw.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ro.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tp.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ue.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ld.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://om.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://og.gzmigu.cn

Ruby: a == b
来源：http://er.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lz.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mr.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fb.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://kk.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pg.bjjhwx.cn

TS:   if (x == null) {}
来源：http://sj.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tb.newstarts.cn

Go:   if x == nil {}
来源：http://zb.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tp.shxzskj.cn

C#:   if (x is null) {}
来源：http://pl.wgjwhj.cn

[P07] 防抖与节流
来源：http://lz.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cf.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://oo.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://as.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sm.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ze.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ys.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ek.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ke.asd995.cn

[P08] 处理浮点精度问题
来源：http://ne.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wr.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xh.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rs.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://go.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ml.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://as.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://df.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ug.asd995.cn

================================================================================
来源：http://yr.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pr.chemitech.net.cn

================================================================================
来源：http://ys.bookmarksfly.cn

[Q01] 创建表
来源：http://kq.huanxung.cn

CREATE TABLE users (
来源：http://wm.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ly.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://ws.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://rt.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ob.yuntaijiaju.cn

);
来源：http://ta.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://ii.asd995.cn

CREATE TABLE orders (
来源：http://xl.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qd.hahajie.cn

user_id INT NOT NULL,
来源：http://gi.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://eg.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xs.9csxet.cn

);
来源：http://lj.shxzukj.cn

[Q03] 增加列
来源：http://nx.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yy.newstarts.cn

[Q04] 修改列类型
来源：http://td.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aa.jianghongdianzi.cn

[Q05] 重命名列
来源：http://jg.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ml.shxzukj.cn

[Q06] 删除列
来源：http://kw.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yj.chemitech.net.cn

[Q07] 删除表
来源：http://ug.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://sr.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://ax.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eh.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://ud.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aq.huixinmuqiang.cn

[Q10] 插入单行
来源：http://ao.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ey.newstarts.cn

[Q11] 一次插入多行
来源：http://pu.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dt.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://wu.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sw.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ma.newstarts.cn

[Q13] 忽略重复插入
来源：http://bi.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qw.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://hb.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sx.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lf.shtwfgs.cn

[Q15] 查询全部
来源：http://wx.shxzukj.cn

SELECT * FROM users;
来源：http://ko.muxihuayi.cn

[Q16] 查询指定列
来源：http://de.shtwfgs.cn

SELECT id, name FROM users;
来源：http://sv.bookmarksfly.cn

[Q17] 条件查询
来源：http://sj.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dk.szxytkj.cn

[Q18] 模糊匹配
来源：http://sh.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mz.nszjky.cn

[Q19] 范围查询
来源：http://eu.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mj.muxihuayi.cn

[Q20] IN 列表
来源：http://za.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xn.gzmigu.cn

[Q21] 空值判断
来源：http://fe.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ue.hahajie.cn

[Q22] 排序
来源：http://db.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sc.chemitech.net.cn

[Q23] 分页
来源：http://ty.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bh.huanxung.cn

[Q24] 去重
来源：http://ke.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://po.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://di.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hy.gzmigu.cn

[Q26] 计数
来源：http://vb.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://za.newstarts.cn

[Q27] 条件计数
来源：http://pw.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kz.panjiajie.cn

[Q28] 求和与平均
来源：http://ic.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ca.szxytkj.cn

[Q29] 最大最小值
来源：http://ni.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wg.yuntaijiaju.cn

[Q30] 分组统计
来源：http://wa.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ce.huixiangedu.cn

[Q31] 分组后过滤
来源：http://uv.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gw.521024.cn

[Q32] 分组拼接字符串
来源：http://wc.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ji.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ks.haigaiapp.cn

[Q33] 多列分组
来源：http://rl.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xk.newstarts.cn

[Q34] 每组取第一条
来源：http://fp.newstarts.cn

SELECT * FROM (
来源：http://vu.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sv.hahajie.cn

) t WHERE rn = 1;
来源：http://sr.521024.cn

[Q35] 内连接
来源：http://ja.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fq.szsharing.cn

[Q36] 左连接
来源：http://bc.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ky.huixinmuqiang.cn

[Q37] 右连接
来源：http://ak.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tu.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ev.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cs.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://iu.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wh.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dc.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fv.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ta.chemitech.net.cn

[Q41] 多表连接
来源：http://jo.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bf.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://vb.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://vk.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://iz.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://dw.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pq.shxzukj.cn

[Q43] 标量子查询
来源：http://pi.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iu.muxihuayi.cn

[Q44] IN 子查询
来源：http://ba.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://os.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://nx.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ym.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://if.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yz.gzmigu.cn

[Q47] 与平均值比较
来源：http://bx.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xx.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://yq.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ah.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://oe.hahajie.cn

[Q49] 更新单行
来源：http://at.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tl.9csxet.cn

[Q50] 批量更新
来源：http://no.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oh.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://ux.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uu.panjiajie.cn

[Q52] 删除指定行
来源：http://sc.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://fl.wgjwhj.cn

[Q53] 按条件删除
来源：http://zk.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ph.panjiajie.cn

[Q54] 清空表
来源：http://ws.asd995.cn

TRUNCATE TABLE logs;
来源：http://vp.521024.cn

[Q55] 排名（并列占位）
来源：http://kz.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tv.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://dx.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yw.huixinmuqiang.cn

[Q57] 行号
来源：http://hn.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://le.szsharing.cn

[Q58] 累计求和
来源：http://xc.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lf.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://qw.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cx.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://wg.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bk.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jq.colortex.cn

[Q61] 移动平均
来源：http://gy.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kk.jctech888.com.cn

[Q62] 分组占比
来源：http://ds.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xy.nszjky.cn


<!-- 参考信息 -->