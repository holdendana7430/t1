代发 wailian999

Go:   // 手写递归
来源：http://td.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mf.wgjwhj.cn

C#:   // 手写递归
来源：http://tw.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bx.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eb.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dk.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pj.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xx.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rj.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iu.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ho.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ud.lnxyls.cn

================================================================================
来源：http://zl.9csxet.cn

O. 并发与异步
来源：http://kf.chemitech.net.cn

================================================================================
来源：http://hb.muxihuayi.cn

[O01] 启动一个线程
来源：http://gh.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tb.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://no.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tr.shxzskj.cn

TS:   // 同 JS
来源：http://fw.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://ey.wgjwhj.cn

Go:   go f()
来源：http://eo.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://wx.asd995.cn

C#:   Task.Run(() => F());
来源：http://ik.jianghongdianzi.cn

[O02] 使用线程池
来源：http://th.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xz.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nz.9csxet.cn

JS:   // worker_threads 线程池
来源：http://yn.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://zf.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://la.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ny.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gr.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nr.9csxet.cn

[O03] 加锁保护共享数据
来源：http://ud.gzmigu.cn

Py:   with lock: shared += 1
来源：http://kq.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://je.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ut.yuntaijiaju.cn

TS:   // 同 JS
来源：http://jx.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://mr.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://td.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vt.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://ao.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://qx.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://cz.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ak.hahajie.cn

JS:   async function f() { await g(); }
来源：http://ud.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gy.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aj.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uh.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wm.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://mo.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://yw.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://tw.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mq.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://jz.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://yf.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bk.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ji.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://bg.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hn.lnxyls.cn

[O06] 使用进程池
来源：http://cm.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://az.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yu.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://tl.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://wk.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nx.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ai.bookmarksfly.cn

Ruby: // fork 块
来源：http://pe.jctech888.com.cn

C#:   Parallel.For
来源：http://ie.jianghongdianzi.cn

================================================================================
来源：http://nc.nszjky.cn

P. 常用工具函数
来源：http://gs.wgjwhj.cn

================================================================================
来源：http://ci.asd995.cn

[P01] 生成 UUID
来源：http://bi.asd995.cn

Py:   str(uuid.uuid4())
来源：http://pk.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zp.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://ld.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://lq.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://ob.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://jp.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://wz.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://vo.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://ww.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gk.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://do.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dy.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uh.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yr.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pm.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ky.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sb.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://ua.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://af.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xh.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fm.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lk.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gp.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cg.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://il.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ev.szsharing.cn

[P04] 求长度
来源：http://ub.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hj.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xk.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ub.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ma.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://ef.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://jw.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://ox.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vz.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://qw.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cb.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pz.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jj.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://js.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qe.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yo.bjjhwx.cn

Ruby: a == b
来源：http://re.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vi.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qp.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fc.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://jz.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hb.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://yn.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://as.9csxet.cn

Go:   if x == nil {}
来源：http://ba.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xn.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://ju.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ua.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wc.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://pf.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rf.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ac.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mb.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kr.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zk.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aj.huanxung.cn

[P08] 处理浮点精度问题
来源：http://am.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eq.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kk.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kp.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://we.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yc.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ro.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xy.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://by.nszjky.cn

================================================================================
来源：http://gp.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mm.wgjwhj.cn

================================================================================
来源：http://lb.bjjhwx.cn

[Q01] 创建表
来源：http://ov.bookmarksfly.cn

CREATE TABLE users (
来源：http://dy.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cr.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://gs.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://rx.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rl.bookmarksfly.cn

);
来源：http://ug.shxzskj.cn

[Q02] 创建带外键的表
来源：http://pw.yuexingan06.cn

CREATE TABLE orders (
来源：http://rd.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cw.jctech888.com.cn

user_id INT NOT NULL,
来源：http://gh.newstarts.cn

amount DECIMAL(10, 2),
来源：http://cm.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uz.asd995.cn

);
来源：http://ik.shxzukj.cn

[Q03] 增加列
来源：http://bc.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rw.szxytkj.cn

[Q04] 修改列类型
来源：http://jb.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tr.wgjwhj.cn

[Q05] 重命名列
来源：http://zo.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://no.hahajie.cn

[Q06] 删除列
来源：http://na.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wz.nszjky.cn

[Q07] 删除表
来源：http://fp.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://yl.colortex.cn

[Q08] 创建普通索引
来源：http://jk.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sa.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://wj.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bu.panjiajie.cn

[Q10] 插入单行
来源：http://vn.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sw.bjjhwx.cn

[Q11] 一次插入多行
来源：http://nh.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rp.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://rc.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qb.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kv.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://uy.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yp.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://vs.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vj.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yc.shxzukj.cn

[Q15] 查询全部
来源：http://nw.huixinmuqiang.cn

SELECT * FROM users;
来源：http://cs.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://sh.521024.cn

SELECT id, name FROM users;
来源：http://ij.hnjuh.cn

[Q17] 条件查询
来源：http://uj.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uv.panjiajie.cn

[Q18] 模糊匹配
来源：http://jt.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fn.yuntaijiaju.cn

[Q19] 范围查询
来源：http://zy.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dw.yuexingan06.cn

[Q20] IN 列表
来源：http://tj.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uz.lnxyls.cn

[Q21] 空值判断
来源：http://mr.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://un.haigaiapp.cn

[Q22] 排序
来源：http://lc.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wj.huixiangedu.cn

[Q23] 分页
来源：http://my.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://el.yuexingan06.cn

[Q24] 去重
来源：http://ka.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://de.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://bh.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qz.panjiajie.cn

[Q26] 计数
来源：http://ao.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://gk.lnxyls.cn

[Q27] 条件计数
来源：http://sb.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qq.shxzukj.cn

[Q28] 求和与平均
来源：http://lk.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rh.shxzukj.cn

[Q29] 最大最小值
来源：http://wr.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tg.huixinmuqiang.cn

[Q30] 分组统计
来源：http://yw.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gx.chemitech.net.cn

[Q31] 分组后过滤
来源：http://uz.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yv.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://qe.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iv.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qh.huixiangedu.cn

[Q33] 多列分组
来源：http://mm.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://us.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://et.szsharing.cn

SELECT * FROM (
来源：http://pl.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ht.haigaiapp.cn

) t WHERE rn = 1;
来源：http://lo.huanxung.cn

[Q35] 内连接
来源：http://tx.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zy.huixiangedu.cn

[Q36] 左连接
来源：http://df.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ox.newstarts.cn

[Q37] 右连接
来源：http://fq.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xz.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wp.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://si.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://do.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ic.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zg.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hm.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ii.shxzskj.cn

[Q41] 多表连接
来源：http://el.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jx.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://zx.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://zh.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://wv.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://mi.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xe.nicolike.cn

[Q43] 标量子查询
来源：http://eu.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ei.hnjuh.cn

[Q44] IN 子查询
来源：http://ix.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kp.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://ji.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uj.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nj.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bl.szxytkj.cn

[Q47] 与平均值比较
来源：http://zd.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://js.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://ll.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yn.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://es.yuntaijiaju.cn

[Q49] 更新单行
来源：http://ew.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ue.521024.cn

[Q50] 批量更新
来源：http://km.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ji.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://zn.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rz.shtwfgs.cn

[Q52] 删除指定行
来源：http://hl.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://ic.lnxyls.cn

[Q53] 按条件删除
来源：http://rp.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xo.chemitech.net.cn

[Q54] 清空表
来源：http://zc.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://il.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://wx.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qs.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://wm.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ge.muxihuayi.cn

[Q57] 行号
来源：http://nc.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gr.hahajie.cn

[Q58] 累计求和
来源：http://hs.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://av.gzmigu.cn

[Q59] 分组内累计
来源：http://pk.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vc.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://or.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rn.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://py.huanxung.cn

[Q61] 移动平均
来源：http://jp.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gi.huanxung.cn

[Q62] 分组占比
来源：http://hx.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lp.yuexingan06.cn

[Q63] 开启事务
来源：http://at.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mq.muxihuayi.cn

[Q64] 提交事务
来源：http://tw.huixinmuqiang.cn

COMMIT;
来源：http://jb.panjiajie.cn

[Q65] 回滚事务
来源：http://hb.yuexingan06.cn

ROLLBACK;
来源：http://ut.huanxung.cn

[Q66] 行锁查询
来源：http://nb.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zb.shxzskj.cn


<!-- 参考信息 -->