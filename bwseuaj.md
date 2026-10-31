代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xu.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lu.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://lh.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://br.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yq.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ww.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://jv.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ss.shxzskj.cn

PHP:  // 手写递归函数
来源：http://hw.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sq.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pp.yuntaijiaju.cn

Java: // 手写递归
来源：http://am.szsharing.cn

Go:   // 手写递归
来源：http://zy.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://im.wgjwhj.cn

C#:   // 手写递归
来源：http://mg.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lr.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cf.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fc.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bz.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://md.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kp.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yx.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oy.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lr.colortex.cn

================================================================================
来源：http://rr.521024.cn

O. 并发与异步
来源：http://wu.hnjuh.cn

================================================================================
来源：http://vn.shxzskj.cn

[O01] 启动一个线程
来源：http://xg.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cg.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kn.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fv.shxzskj.cn

TS:   // 同 JS
来源：http://cr.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://dg.muxihuayi.cn

Go:   go f()
来源：http://wx.9csxet.cn

Ruby: Thread.new { f }
来源：http://ae.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://nq.asd995.cn

[O02] 使用线程池
来源：http://fs.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sv.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fk.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://wn.asd995.cn

TS:   // worker_threads 线程池
来源：http://fi.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ai.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pu.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dp.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://of.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://wn.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://dt.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://pt.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bw.chemitech.net.cn

TS:   // 同 JS
来源：http://dh.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://ri.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fv.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dd.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://xx.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://qz.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://fd.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xs.huanxung.cn

JS:   async function f() { await g(); }
来源：http://du.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rr.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://id.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ta.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tp.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://rd.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://yd.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://vc.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nj.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://re.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://en.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ha.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://et.newstarts.cn

Ruby: threads.map(&:join)
来源：http://dz.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nb.muxihuayi.cn

[O06] 使用进程池
来源：http://tq.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jh.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hn.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://ap.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://dz.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ph.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qk.hnjuh.cn

Ruby: // fork 块
来源：http://rn.muxihuayi.cn

C#:   Parallel.For
来源：http://vi.jctech888.com.cn

================================================================================
来源：http://xd.newstarts.cn

P. 常用工具函数
来源：http://xm.colortex.cn

================================================================================
来源：http://jt.521024.cn

[P01] 生成 UUID
来源：http://wf.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://zb.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gi.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://nw.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://zf.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://uq.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://yj.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://om.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://qr.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://sd.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xe.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fz.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mk.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://io.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bo.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jo.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://my.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sr.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://xh.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nu.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rh.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://te.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zn.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mh.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nd.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mo.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yw.shxzukj.cn

[P04] 求长度
来源：http://wi.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hb.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dj.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tk.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kn.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://av.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://nv.huanxung.cn

Ruby: x.length;  x.size
来源：http://sb.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rp.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://gv.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ei.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wj.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://by.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bz.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ts.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ot.huixiangedu.cn

Ruby: a == b
来源：http://gb.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sm.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ms.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hh.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://en.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lh.chemitech.net.cn

TS:   if (x == null) {}
来源：http://gb.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bc.lnxyls.cn

Go:   if x == nil {}
来源：http://ie.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://us.shxzukj.cn

C#:   if (x is null) {}
来源：http://cw.bookmarksfly.cn

[P07] 防抖与节流
来源：http://mq.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gx.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://ap.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nu.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qt.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bw.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://re.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cs.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fq.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ku.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bp.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sh.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bf.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gu.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nq.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xw.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dl.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ex.huixinmuqiang.cn

================================================================================
来源：http://ve.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wg.gzmigu.cn

================================================================================
来源：http://rx.521024.cn

[Q01] 创建表
来源：http://jz.nicolike.cn

CREATE TABLE users (
来源：http://rm.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lj.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://lu.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://hw.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ue.gzmigu.cn

);
来源：http://sb.shxzukj.cn

[Q02] 创建带外键的表
来源：http://rq.bookmarksfly.cn

CREATE TABLE orders (
来源：http://uj.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ls.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://hy.newstarts.cn

amount DECIMAL(10, 2),
来源：http://bz.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wi.chemitech.net.cn

);
来源：http://hb.bookmarksfly.cn

[Q03] 增加列
来源：http://bp.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pp.jctech888.com.cn

[Q04] 修改列类型
来源：http://dh.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bp.lnxyls.cn

[Q05] 重命名列
来源：http://qr.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cq.colortex.cn

[Q06] 删除列
来源：http://bn.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bb.shxzukj.cn

[Q07] 删除表
来源：http://po.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://gr.newstarts.cn

[Q08] 创建普通索引
来源：http://sl.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kv.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://vo.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yt.asd995.cn

[Q10] 插入单行
来源：http://oy.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://od.bjjhwx.cn

[Q11] 一次插入多行
来源：http://ik.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eb.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://np.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ab.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pm.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://cs.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://je.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://fz.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://we.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cf.gzmigu.cn

[Q15] 查询全部
来源：http://nx.colortex.cn

SELECT * FROM users;
来源：http://em.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://fd.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://cj.9csxet.cn

[Q17] 条件查询
来源：http://zz.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ba.chemitech.net.cn

[Q18] 模糊匹配
来源：http://mp.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sj.szxytkj.cn

[Q19] 范围查询
来源：http://yx.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ed.muxihuayi.cn

[Q20] IN 列表
来源：http://uh.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ux.gzmigu.cn

[Q21] 空值判断
来源：http://jw.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yr.jctech888.com.cn

[Q22] 排序
来源：http://no.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ya.nszjky.cn

[Q23] 分页
来源：http://nb.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hc.huixiangedu.cn

[Q24] 去重
来源：http://ie.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://ot.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://ac.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hf.gzmigu.cn

[Q26] 计数
来源：http://uh.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://fn.panjiajie.cn

[Q27] 条件计数
来源：http://ko.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qi.panjiajie.cn

[Q28] 求和与平均
来源：http://rl.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tq.shtwfgs.cn

[Q29] 最大最小值
来源：http://el.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wj.newstarts.cn

[Q30] 分组统计
来源：http://by.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aw.shxzukj.cn

[Q31] 分组后过滤
来源：http://mk.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kz.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://sg.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dm.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tg.newstarts.cn

[Q33] 多列分组
来源：http://sg.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://au.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://sv.shtwfgs.cn

SELECT * FROM (
来源：http://az.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zf.lnxyls.cn

) t WHERE rn = 1;
来源：http://bh.huixiangedu.cn

[Q35] 内连接
来源：http://ev.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xi.huixinmuqiang.cn

[Q36] 左连接
来源：http://et.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xr.nszjky.cn

[Q37] 右连接
来源：http://hw.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ja.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xt.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zg.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://se.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xq.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sm.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yj.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mo.hnjuh.cn

[Q41] 多表连接
来源：http://td.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ij.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://lc.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://jf.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://fj.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://ec.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zk.colortex.cn

[Q43] 标量子查询
来源：http://uq.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mp.shxzukj.cn

[Q44] IN 子查询
来源：http://py.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tu.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://uj.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vv.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://us.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kf.chemitech.net.cn

[Q47] 与平均值比较
来源：http://wi.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ko.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://tq.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lz.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://rh.asd995.cn

[Q49] 更新单行
来源：http://ty.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aa.haigaiapp.cn

[Q50] 批量更新
来源：http://xd.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ql.521024.cn

[Q51] 用子查询更新
来源：http://bg.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://km.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://kv.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://zx.huixiangedu.cn

[Q53] 按条件删除
来源：http://he.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oh.yuntaijiaju.cn

[Q54] 清空表
来源：http://uy.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://oo.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://cg.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wi.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://nk.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ts.nszjky.cn

[Q57] 行号
来源：http://ee.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gk.shxzskj.cn

[Q58] 累计求和
来源：http://mx.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sg.hnjuh.cn

[Q59] 分组内累计
来源：http://nt.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qx.521024.cn

[Q60] 取上一行 / 下一行
来源：http://wp.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pp.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qk.huixinmuqiang.cn


<!-- 参考信息 -->