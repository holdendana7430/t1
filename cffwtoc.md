代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://je.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qc.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gi.muxihuayi.cn

TS:   // 同 JS
来源：http://ad.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://gr.521024.cn

Go:   go f()
来源：http://gb.huanxung.cn

Ruby: Thread.new { f }
来源：http://hb.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://wa.szxytkj.cn

[O02] 使用线程池
来源：http://iv.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zf.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yo.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://nd.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://bh.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jg.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xk.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xr.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ou.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://bo.lnxyls.cn

Py:   with lock: shared += 1
来源：http://pj.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://cj.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vj.shtwfgs.cn

TS:   // 同 JS
来源：http://lc.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://hh.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fa.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://np.521024.cn

C#:   lock (gate) { shared++; }
来源：http://mg.hahajie.cn

[O04] 定义异步函数并等待
来源：http://ko.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://xs.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ym.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://vw.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ci.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cv.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zn.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ri.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://ts.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://pm.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://sd.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ng.asd995.cn

JS:   await Promise.all(tasks)
来源：http://ny.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://nr.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fv.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bz.521024.cn

Ruby: threads.map(&:join)
来源：http://mv.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tf.shtwfgs.cn

[O06] 使用进程池
来源：http://ce.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lk.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mi.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://ee.asd995.cn

TS:   // child_process / cluster 模块
来源：http://wj.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://um.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://el.bjjhwx.cn

Ruby: // fork 块
来源：http://no.shxzskj.cn

C#:   Parallel.For
来源：http://nj.newstarts.cn

================================================================================
来源：http://ai.newstarts.cn

P. 常用工具函数
来源：http://ek.panjiajie.cn

================================================================================
来源：http://th.jctech888.com.cn

[P01] 生成 UUID
来源：http://kq.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://zs.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cl.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://jw.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://ls.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://yj.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://sa.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://pd.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://tb.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://ij.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eg.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fs.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yr.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oz.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rc.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qp.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wr.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zd.asd995.cn

[P03] 生成短随机字符串
来源：http://qa.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vk.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cb.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qx.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ay.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ra.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kz.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iz.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://df.hnjuh.cn

[P04] 求长度
来源：http://ax.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sn.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tu.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rm.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cd.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://yi.9csxet.cn

Go:   len(arr);  len(m)
来源：http://uq.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://ju.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yd.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://bb.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sa.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://no.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mk.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hm.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rc.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lv.szsharing.cn

Ruby: a == b
来源：http://ex.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yc.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ll.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ow.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://mk.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://km.yuexingan06.cn

TS:   if (x == null) {}
来源：http://mk.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hh.9csxet.cn

Go:   if x == nil {}
来源：http://xo.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ug.lnxyls.cn

C#:   if (x is null) {}
来源：http://qp.asd995.cn

[P07] 防抖与节流
来源：http://ao.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jk.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://wy.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ls.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://me.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mj.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ej.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hf.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cd.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://tp.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oa.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qn.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yh.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wi.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pv.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tv.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dh.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dr.gzmigu.cn

================================================================================
来源：http://fd.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mw.lnxyls.cn

================================================================================
来源：http://ug.shxzskj.cn

[Q01] 创建表
来源：http://nd.jctech888.com.cn

CREATE TABLE users (
来源：http://ex.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ap.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://qc.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://yu.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ik.jianghongdianzi.cn

);
来源：http://re.9csxet.cn

[Q02] 创建带外键的表
来源：http://mo.bookmarksfly.cn

CREATE TABLE orders (
来源：http://hd.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wr.shxzukj.cn

user_id INT NOT NULL,
来源：http://ww.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://ke.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mh.huixiangedu.cn

);
来源：http://qe.bjjhwx.cn

[Q03] 增加列
来源：http://ks.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xv.newstarts.cn

[Q04] 修改列类型
来源：http://zc.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vm.521024.cn

[Q05] 重命名列
来源：http://wp.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pj.521024.cn

[Q06] 删除列
来源：http://rc.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jt.newstarts.cn

[Q07] 删除表
来源：http://sb.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://bs.gzmigu.cn

[Q08] 创建普通索引
来源：http://ad.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xf.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://cn.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wr.yuntaijiaju.cn

[Q10] 插入单行
来源：http://vu.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cy.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://ym.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mj.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://ji.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jw.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vc.nicolike.cn

[Q13] 忽略重复插入
来源：http://zc.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ys.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://ot.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bg.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://id.huixiangedu.cn

[Q15] 查询全部
来源：http://pp.nicolike.cn

SELECT * FROM users;
来源：http://we.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://jr.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://pl.bjjhwx.cn

[Q17] 条件查询
来源：http://kr.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nk.shxzukj.cn

[Q18] 模糊匹配
来源：http://gd.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ky.asd995.cn

[Q19] 范围查询
来源：http://hl.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ix.szxytkj.cn

[Q20] IN 列表
来源：http://zw.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ag.shxzskj.cn

[Q21] 空值判断
来源：http://yr.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ks.yuexingan06.cn

[Q22] 排序
来源：http://bj.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kw.nszjky.cn

[Q23] 分页
来源：http://yl.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ek.wgjwhj.cn

[Q24] 去重
来源：http://cr.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://go.nszjky.cn

[Q25] 只取前 N 条
来源：http://jr.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uq.shxzukj.cn

[Q26] 计数
来源：http://pp.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://sv.521024.cn

[Q27] 条件计数
来源：http://lm.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ft.colortex.cn

[Q28] 求和与平均
来源：http://gc.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dn.gzmigu.cn

[Q29] 最大最小值
来源：http://wn.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bx.bjjhwx.cn

[Q30] 分组统计
来源：http://bw.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bt.panjiajie.cn

[Q31] 分组后过滤
来源：http://pt.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cq.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://hy.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rf.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rz.521024.cn

[Q33] 多列分组
来源：http://tx.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nj.nicolike.cn

[Q34] 每组取第一条
来源：http://ur.521024.cn

SELECT * FROM (
来源：http://lm.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lk.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://fo.colortex.cn

[Q35] 内连接
来源：http://vt.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vd.szxytkj.cn

[Q36] 左连接
来源：http://wf.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nt.yuntaijiaju.cn

[Q37] 右连接
来源：http://fn.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ps.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ek.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vk.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://oh.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://li.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oe.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qy.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ld.huixiangedu.cn

[Q41] 多表连接
来源：http://uk.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jl.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://ok.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://em.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://gx.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://xa.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://df.muxihuayi.cn

[Q43] 标量子查询
来源：http://jr.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hx.hnjuh.cn

[Q44] IN 子查询
来源：http://li.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ho.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://sp.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pd.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qw.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xv.jctech888.com.cn

[Q47] 与平均值比较
来源：http://co.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dg.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://xj.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lh.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://cg.gzmigu.cn

[Q49] 更新单行
来源：http://mw.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hr.haigaiapp.cn

[Q50] 批量更新
来源：http://ag.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kx.panjiajie.cn

[Q51] 用子查询更新
来源：http://aw.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ja.shtwfgs.cn

[Q52] 删除指定行
来源：http://uf.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://iu.bookmarksfly.cn

[Q53] 按条件删除
来源：http://sw.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qt.hnjuh.cn

[Q54] 清空表
来源：http://yk.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://kh.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://fp.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://js.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://is.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rv.wgjwhj.cn

[Q57] 行号
来源：http://kh.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xv.jctech888.com.cn

[Q58] 累计求和
来源：http://yd.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ai.yuexingan06.cn

[Q59] 分组内累计
来源：http://op.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gg.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://xw.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ry.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ze.huanxung.cn

[Q61] 移动平均
来源：http://vu.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pm.shxzukj.cn

[Q62] 分组占比
来源：http://rk.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fp.wgjwhj.cn

[Q63] 开启事务
来源：http://ih.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dd.chemitech.net.cn

[Q64] 提交事务
来源：http://lx.szxytkj.cn

COMMIT;
来源：http://up.shxzukj.cn

[Q65] 回滚事务
来源：http://nx.huixiangedu.cn

ROLLBACK;
来源：http://tj.huanxung.cn

[Q66] 行锁查询
来源：http://nj.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rj.nicolike.cn

[Q67] 设置隔离级别
来源：http://wr.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mn.bookmarksfly.cn

[Q68] 保存点
来源：http://hy.panjiajie.cn

SAVEPOINT sp1;
来源：http://gs.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://xs.gzmigu.cn

[Q69] 查看执行计划
来源：http://ix.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://za.shtwfgs.cn

[Q70] 更新统计信息
来源：http://vq.nszjky.cn

ANALYZE TABLE users;
来源：http://tw.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://cv.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xz.jctech888.com.cn

[Q72] 查看索引
来源：http://es.newstarts.cn

SHOW INDEX FROM users;
来源：http://ge.nicolike.cn

[Q73] 查看表状态
来源：http://jj.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uf.colortex.cn

[Q74] 强制使用索引
来源：http://fp.shxzskj.cn


<!-- 参考信息 -->