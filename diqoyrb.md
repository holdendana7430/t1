代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gf.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zu.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kg.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vm.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lv.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xq.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wj.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kt.huanxung.cn

================================================================================
来源：http://zj.9csxet.cn

O. 并发与异步
来源：http://ff.asd995.cn

================================================================================
来源：http://vv.nszjky.cn

[O01] 启动一个线程
来源：http://sh.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kg.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hl.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uf.521024.cn

TS:   // 同 JS
来源：http://cs.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://gx.jianghongdianzi.cn

Go:   go f()
来源：http://gd.shxzukj.cn

Ruby: Thread.new { f }
来源：http://dw.huanxung.cn

C#:   Task.Run(() => F());
来源：http://yd.9csxet.cn

[O02] 使用线程池
来源：http://db.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://of.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yb.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://cz.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://gh.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jv.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fj.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rl.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vy.nicolike.cn

[O03] 加锁保护共享数据
来源：http://vb.lnxyls.cn

Py:   with lock: shared += 1
来源：http://ro.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://gg.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ba.jianghongdianzi.cn

TS:   // 同 JS
来源：http://hq.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://zt.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://on.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cv.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://xp.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://uc.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://io.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dy.521024.cn

JS:   async function f() { await g(); }
来源：http://qc.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hu.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://in.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mu.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dn.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://qd.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://xj.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://bh.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rf.asd995.cn

JS:   await Promise.all(tasks)
来源：http://pd.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://sv.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tf.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fn.asd995.cn

Ruby: threads.map(&:join)
来源：http://ew.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mv.bookmarksfly.cn

[O06] 使用进程池
来源：http://rc.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gz.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tj.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://yb.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://sl.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zh.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iq.9csxet.cn

Ruby: // fork 块
来源：http://zw.nszjky.cn

C#:   Parallel.For
来源：http://fg.521024.cn

================================================================================
来源：http://ls.bjjhwx.cn

P. 常用工具函数
来源：http://tu.newstarts.cn

================================================================================
来源：http://at.szxytkj.cn

[P01] 生成 UUID
来源：http://hv.521024.cn

Py:   str(uuid.uuid4())
来源：http://td.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xt.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://ro.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://ya.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://ky.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://ai.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://rr.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://gf.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://mm.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cf.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tv.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ym.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iv.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://il.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cd.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qe.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cv.hahajie.cn

[P03] 生成短随机字符串
来源：http://cn.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://da.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lr.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nm.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jy.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sp.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ik.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dg.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cj.hnjuh.cn

[P04] 求长度
来源：http://oo.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hi.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sc.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ck.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vq.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://ek.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://be.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://ai.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yh.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://gk.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pm.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mr.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://px.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ys.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gq.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yh.hnjuh.cn

Ruby: a == b
来源：http://sy.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nc.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fn.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pz.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://di.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xg.huixiangedu.cn

TS:   if (x == null) {}
来源：http://ri.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xn.asd995.cn

Go:   if x == nil {}
来源：http://ff.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://um.wgjwhj.cn

C#:   if (x is null) {}
来源：http://lt.shxzukj.cn

[P07] 防抖与节流
来源：http://qp.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xx.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://kw.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://da.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ic.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oj.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hx.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oz.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://en.9csxet.cn

[P08] 处理浮点精度问题
来源：http://fm.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hq.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://se.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://se.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ef.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tt.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://in.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wm.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ka.nicolike.cn

================================================================================
来源：http://zt.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cd.yuexingan06.cn

================================================================================
来源：http://wj.wgjwhj.cn

[Q01] 创建表
来源：http://sn.jctech888.com.cn

CREATE TABLE users (
来源：http://rb.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://re.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://rv.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://xd.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://au.nicolike.cn

);
来源：http://ch.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://ez.521024.cn

CREATE TABLE orders (
来源：http://za.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://id.panjiajie.cn

user_id INT NOT NULL,
来源：http://dr.nszjky.cn

amount DECIMAL(10, 2),
来源：http://to.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://og.hahajie.cn

);
来源：http://ax.shtwfgs.cn

[Q03] 增加列
来源：http://cm.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zs.newstarts.cn

[Q04] 修改列类型
来源：http://ip.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gb.muxihuayi.cn

[Q05] 重命名列
来源：http://jj.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://le.yuntaijiaju.cn

[Q06] 删除列
来源：http://cq.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ma.asd995.cn

[Q07] 删除表
来源：http://et.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://sc.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://yd.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ns.szxytkj.cn

[Q09] 创建唯一索引
来源：http://oi.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://or.gzmigu.cn

[Q10] 插入单行
来源：http://mq.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dx.shtwfgs.cn

[Q11] 一次插入多行
来源：http://ny.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ov.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://fv.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://je.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fd.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://lw.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sn.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://nl.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lq.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qk.shxzukj.cn

[Q15] 查询全部
来源：http://ir.jctech888.com.cn

SELECT * FROM users;
来源：http://cm.colortex.cn

[Q16] 查询指定列
来源：http://tu.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://oa.shxzskj.cn

[Q17] 条件查询
来源：http://lz.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kn.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://ia.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rj.haigaiapp.cn

[Q19] 范围查询
来源：http://li.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hi.colortex.cn

[Q20] IN 列表
来源：http://ni.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vv.szsharing.cn

[Q21] 空值判断
来源：http://ct.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://at.bjjhwx.cn

[Q22] 排序
来源：http://cf.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bk.jianghongdianzi.cn

[Q23] 分页
来源：http://uc.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wr.hnjuh.cn

[Q24] 去重
来源：http://fa.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://sh.panjiajie.cn

[Q25] 只取前 N 条
来源：http://nu.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xp.shxzukj.cn

[Q26] 计数
来源：http://sp.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://za.huixiangedu.cn

[Q27] 条件计数
来源：http://oq.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ve.panjiajie.cn

[Q28] 求和与平均
来源：http://vs.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dl.colortex.cn

[Q29] 最大最小值
来源：http://no.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xr.shxzskj.cn

[Q30] 分组统计
来源：http://cg.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://by.panjiajie.cn

[Q31] 分组后过滤
来源：http://nk.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gr.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://xd.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ne.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fs.huixinmuqiang.cn

[Q33] 多列分组
来源：http://sx.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iv.521024.cn

[Q34] 每组取第一条
来源：http://eq.colortex.cn

SELECT * FROM (
来源：http://kn.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jg.jctech888.com.cn

) t WHERE rn = 1;
来源：http://ng.bjjhwx.cn

[Q35] 内连接
来源：http://ld.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sf.newstarts.cn

[Q36] 左连接
来源：http://xu.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zz.chemitech.net.cn

[Q37] 右连接
来源：http://rs.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lv.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ar.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ae.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://gb.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kq.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aa.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cx.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ic.bookmarksfly.cn

[Q41] 多表连接
来源：http://pt.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dr.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://wh.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://np.colortex.cn

[Q42] 连接条件附加过滤
来源：http://ne.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://nb.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://en.haigaiapp.cn

[Q43] 标量子查询
来源：http://zy.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mr.yuexingan06.cn

[Q44] IN 子查询
来源：http://at.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xk.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://uy.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dx.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kg.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ni.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://uv.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bv.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://hu.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gu.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://vb.hahajie.cn

[Q49] 更新单行
来源：http://oe.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ce.chemitech.net.cn

[Q50] 批量更新
来源：http://kp.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eu.hnjuh.cn

[Q51] 用子查询更新
来源：http://pn.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mb.chemitech.net.cn

[Q52] 删除指定行
来源：http://qa.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://rf.colortex.cn

[Q53] 按条件删除
来源：http://xa.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qq.hahajie.cn

[Q54] 清空表
来源：http://fw.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://iy.521024.cn

[Q55] 排名（并列占位）
来源：http://jz.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://io.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://hp.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dt.wgjwhj.cn

[Q57] 行号
来源：http://wq.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bb.newstarts.cn

[Q58] 累计求和
来源：http://lp.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nv.nicolike.cn

[Q59] 分组内累计
来源：http://ed.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ar.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://tw.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fw.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wd.muxihuayi.cn

[Q61] 移动平均
来源：http://hl.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dr.nszjky.cn

[Q62] 分组占比
来源：http://gm.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cn.newstarts.cn

[Q63] 开启事务
来源：http://lt.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uk.9csxet.cn

[Q64] 提交事务
来源：http://hc.jianghongdianzi.cn

COMMIT;
来源：http://gw.szxytkj.cn

[Q65] 回滚事务
来源：http://xa.9csxet.cn

ROLLBACK;
来源：http://yq.szsharing.cn

[Q66] 行锁查询
来源：http://ak.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hm.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://dz.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kf.huixinmuqiang.cn

[Q68] 保存点
来源：http://gh.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://mx.hnjuh.cn


<!-- 参考信息 -->