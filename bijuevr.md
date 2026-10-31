代发 wailian999

Go:   // 手写递归
来源：http://iz.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hw.shxzskj.cn

C#:   // 手写递归
来源：http://oa.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ez.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dy.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://am.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yy.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sf.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uk.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sk.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gh.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://br.yuntaijiaju.cn

================================================================================
来源：http://ll.newstarts.cn

O. 并发与异步
来源：http://ri.huanxung.cn

================================================================================
来源：http://xx.shxzskj.cn

[O01] 启动一个线程
来源：http://du.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zd.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://un.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fe.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ws.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://he.huixinmuqiang.cn

Go:   go f()
来源：http://bk.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://dl.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://am.shtwfgs.cn

[O02] 使用线程池
来源：http://tx.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ne.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lk.nszjky.cn

JS:   // worker_threads 线程池
来源：http://bj.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://bs.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yx.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fk.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gt.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nt.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://kf.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://gy.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ls.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zg.szxytkj.cn

TS:   // 同 JS
来源：http://ax.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://sb.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fy.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xg.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://ok.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://po.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://de.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mc.nicolike.cn

JS:   async function f() { await g(); }
来源：http://eg.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oe.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tx.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pb.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://km.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://hu.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://ao.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://of.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ww.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://pb.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://ph.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pw.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ah.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://ol.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fa.yuntaijiaju.cn

[O06] 使用进程池
来源：http://pr.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fp.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nc.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://fo.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://um.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sw.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://im.9csxet.cn

Ruby: // fork 块
来源：http://ab.shxzskj.cn

C#:   Parallel.For
来源：http://zf.yuexingan06.cn

================================================================================
来源：http://dd.9csxet.cn

P. 常用工具函数
来源：http://ri.colortex.cn

================================================================================
来源：http://dw.huanxung.cn

[P01] 生成 UUID
来源：http://db.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://hf.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zv.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://ml.nicolike.cn

TS:   crypto.randomUUID()
来源：http://zx.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://lf.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://ue.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://qg.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://ar.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://xg.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rj.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pu.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nr.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yt.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aj.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://no.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ao.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ak.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://lz.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ln.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wr.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://im.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pg.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://to.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://if.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zo.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://re.wgjwhj.cn

[P04] 求长度
来源：http://kq.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gd.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ya.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wd.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rh.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://mh.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://bv.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://lh.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://li.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://ma.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fn.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wf.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xl.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zd.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ob.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rn.521024.cn

Ruby: a == b
来源：http://yp.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rs.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://be.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ft.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://ge.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ha.newstarts.cn

TS:   if (x == null) {}
来源：http://yc.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cg.huixiangedu.cn

Go:   if x == nil {}
来源：http://pf.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mh.hahajie.cn

C#:   if (x is null) {}
来源：http://dq.yuexingan06.cn

[P07] 防抖与节流
来源：http://vf.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zh.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://uy.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pa.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tf.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wa.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://us.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mn.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jp.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://fc.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vd.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rs.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qy.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xk.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cp.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mn.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zi.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ve.lnxyls.cn

================================================================================
来源：http://rc.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yo.9csxet.cn

================================================================================
来源：http://sz.huixinmuqiang.cn

[Q01] 创建表
来源：http://ci.szxytkj.cn

CREATE TABLE users (
来源：http://bi.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tv.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://ze.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://kn.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ox.nicolike.cn

);
来源：http://qw.newstarts.cn

[Q02] 创建带外键的表
来源：http://lb.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://jg.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pf.hnjuh.cn

user_id INT NOT NULL,
来源：http://wf.newstarts.cn

amount DECIMAL(10, 2),
来源：http://al.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gr.haigaiapp.cn

);
来源：http://pa.chemitech.net.cn

[Q03] 增加列
来源：http://dv.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mn.colortex.cn

[Q04] 修改列类型
来源：http://mi.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kr.yuntaijiaju.cn

[Q05] 重命名列
来源：http://je.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ig.szxytkj.cn

[Q06] 删除列
来源：http://vi.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ae.shxzukj.cn

[Q07] 删除表
来源：http://dd.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://wz.bjjhwx.cn

[Q08] 创建普通索引
来源：http://ps.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ho.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://du.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zh.asd995.cn

[Q10] 插入单行
来源：http://wv.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zl.szxytkj.cn

[Q11] 一次插入多行
来源：http://pb.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ry.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://ob.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jg.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vw.nszjky.cn

[Q13] 忽略重复插入
来源：http://zm.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ul.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://gk.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bs.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ub.shtwfgs.cn

[Q15] 查询全部
来源：http://rd.newstarts.cn

SELECT * FROM users;
来源：http://dr.shxzskj.cn

[Q16] 查询指定列
来源：http://zu.colortex.cn

SELECT id, name FROM users;
来源：http://or.shtwfgs.cn

[Q17] 条件查询
来源：http://wd.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qo.nicolike.cn

[Q18] 模糊匹配
来源：http://fp.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ej.newstarts.cn

[Q19] 范围查询
来源：http://mf.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eg.haigaiapp.cn

[Q20] IN 列表
来源：http://oo.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ra.huixinmuqiang.cn

[Q21] 空值判断
来源：http://oa.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pv.haigaiapp.cn

[Q22] 排序
来源：http://in.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wu.nicolike.cn

[Q23] 分页
来源：http://qt.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zi.szsharing.cn

[Q24] 去重
来源：http://ic.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ja.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://dq.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ur.521024.cn

[Q26] 计数
来源：http://gf.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://mw.haigaiapp.cn

[Q27] 条件计数
来源：http://rp.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qq.lnxyls.cn

[Q28] 求和与平均
来源：http://fh.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nl.nszjky.cn

[Q29] 最大最小值
来源：http://st.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vh.yuntaijiaju.cn

[Q30] 分组统计
来源：http://zl.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ap.nszjky.cn

[Q31] 分组后过滤
来源：http://uh.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xg.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://ee.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gk.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://un.haigaiapp.cn

[Q33] 多列分组
来源：http://nq.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bi.9csxet.cn

[Q34] 每组取第一条
来源：http://su.huixiangedu.cn

SELECT * FROM (
来源：http://od.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hn.asd995.cn

) t WHERE rn = 1;
来源：http://ou.panjiajie.cn

[Q35] 内连接
来源：http://df.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ct.wgjwhj.cn

[Q36] 左连接
来源：http://tx.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qe.shtwfgs.cn

[Q37] 右连接
来源：http://us.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qo.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vm.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://br.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://gr.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vp.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iw.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jg.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mi.shxzukj.cn

[Q41] 多表连接
来源：http://un.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ry.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://nx.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://zi.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://sj.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://hg.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fm.bjjhwx.cn

[Q43] 标量子查询
来源：http://ro.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qp.hahajie.cn

[Q44] IN 子查询
来源：http://ld.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ui.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://sq.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://co.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wd.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://id.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://yt.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gh.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://wq.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sb.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://ly.huixiangedu.cn

[Q49] 更新单行
来源：http://lr.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xb.huixiangedu.cn

[Q50] 批量更新
来源：http://ru.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ut.jctech888.com.cn

[Q51] 用子查询更新
来源：http://vu.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mk.nicolike.cn

[Q52] 删除指定行
来源：http://rk.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://zl.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://qp.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ym.shtwfgs.cn

[Q54] 清空表
来源：http://kr.521024.cn

TRUNCATE TABLE logs;
来源：http://at.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://iz.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fq.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://uz.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://js.yuexingan06.cn

[Q57] 行号
来源：http://jc.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jb.9csxet.cn

[Q58] 累计求和
来源：http://jd.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zn.asd995.cn

[Q59] 分组内累计
来源：http://qu.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dg.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://rw.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tc.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ci.lnxyls.cn

[Q61] 移动平均
来源：http://wv.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cb.asd995.cn

[Q62] 分组占比
来源：http://ne.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nd.panjiajie.cn

[Q63] 开启事务
来源：http://gf.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bh.shxzukj.cn

[Q64] 提交事务
来源：http://bm.yuntaijiaju.cn

COMMIT;
来源：http://wa.asd995.cn

[Q65] 回滚事务
来源：http://lm.bjjhwx.cn

ROLLBACK;
来源：http://ox.shxzskj.cn

[Q66] 行锁查询
来源：http://uo.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bd.bookmarksfly.cn


<!-- 参考信息 -->