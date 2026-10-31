代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cl.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mh.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hw.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tv.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sx.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jk.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zc.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qi.521024.cn

================================================================================
来源：http://oh.gzmigu.cn

O. 并发与异步
来源：http://ms.colortex.cn

================================================================================
来源：http://dp.hahajie.cn

[O01] 启动一个线程
来源：http://tt.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://by.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sf.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rf.521024.cn

TS:   // 同 JS
来源：http://et.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://dm.lnxyls.cn

Go:   go f()
来源：http://dr.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://bo.nszjky.cn

C#:   Task.Run(() => F());
来源：http://bb.nszjky.cn

[O02] 使用线程池
来源：http://jk.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wh.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://af.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ms.newstarts.cn

TS:   // worker_threads 线程池
来源：http://zn.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://st.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://we.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uz.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cc.asd995.cn

[O03] 加锁保护共享数据
来源：http://qb.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://hm.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://se.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zd.521024.cn

TS:   // 同 JS
来源：http://zg.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://iv.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zi.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zv.521024.cn

C#:   lock (gate) { shared++; }
来源：http://gq.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://to.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://ub.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bq.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://lu.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uv.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dm.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ts.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://em.asd995.cn

C#:   async Task F() { await G(); }
来源：http://jd.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://pa.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://rp.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rz.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://zk.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://yd.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rg.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ut.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://xz.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ko.huixiangedu.cn

[O06] 使用进程池
来源：http://xi.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ps.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mx.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://lb.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://sg.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vp.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gd.bookmarksfly.cn

Ruby: // fork 块
来源：http://ff.muxihuayi.cn

C#:   Parallel.For
来源：http://sd.lnxyls.cn

================================================================================
来源：http://hx.bookmarksfly.cn

P. 常用工具函数
来源：http://hq.shtwfgs.cn

================================================================================
来源：http://ug.521024.cn

[P01] 生成 UUID
来源：http://bk.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://kx.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xr.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://qo.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://ax.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://iz.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://in.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://og.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://sv.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://sj.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wc.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nf.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sf.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cg.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ez.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qi.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oa.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zv.panjiajie.cn

[P03] 生成短随机字符串
来源：http://de.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sr.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://to.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xi.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gy.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hr.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jw.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qs.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vw.jianghongdianzi.cn

[P04] 求长度
来源：http://kc.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lk.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wm.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rs.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uj.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://qq.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://ln.9csxet.cn

Ruby: x.length;  x.size
来源：http://ng.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oc.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://ww.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qm.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://od.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wv.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pb.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://js.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jj.muxihuayi.cn

Ruby: a == b
来源：http://gh.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ht.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bv.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kf.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://vw.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ux.nicolike.cn

TS:   if (x == null) {}
来源：http://mw.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://by.bjjhwx.cn

Go:   if x == nil {}
来源：http://ox.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ox.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://su.hnjuh.cn

[P07] 防抖与节流
来源：http://kw.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bz.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://hz.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ey.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wr.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pc.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://es.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://am.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vm.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://kj.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://id.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pm.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fn.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jt.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://is.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ec.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qo.gzmigu.cn

================================================================================
来源：http://ru.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dk.colortex.cn

================================================================================
来源：http://vj.hnjuh.cn

[Q01] 创建表
来源：http://yx.huixinmuqiang.cn

CREATE TABLE users (
来源：http://lv.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vg.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://dy.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://lk.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sx.shxzskj.cn

);
来源：http://wx.huanxung.cn

[Q02] 创建带外键的表
来源：http://gp.huixiangedu.cn

CREATE TABLE orders (
来源：http://lk.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ge.chemitech.net.cn

user_id INT NOT NULL,
来源：http://et.newstarts.cn

amount DECIMAL(10, 2),
来源：http://am.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sx.szxytkj.cn

);
来源：http://xp.bjjhwx.cn

[Q03] 增加列
来源：http://ee.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dx.panjiajie.cn

[Q04] 修改列类型
来源：http://od.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ld.yuexingan06.cn

[Q05] 重命名列
来源：http://ki.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zy.yuexingan06.cn

[Q06] 删除列
来源：http://ma.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fg.muxihuayi.cn

[Q07] 删除表
来源：http://bc.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://us.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://de.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nb.colortex.cn

[Q09] 创建唯一索引
来源：http://dj.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yh.yuntaijiaju.cn

[Q10] 插入单行
来源：http://nx.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aw.huanxung.cn

[Q11] 一次插入多行
来源：http://vu.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qz.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://ko.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uq.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rf.9csxet.cn

[Q13] 忽略重复插入
来源：http://oe.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fi.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://ep.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uo.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ka.shxzukj.cn

[Q15] 查询全部
来源：http://du.jctech888.com.cn

SELECT * FROM users;
来源：http://pk.huixiangedu.cn

[Q16] 查询指定列
来源：http://nk.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://sr.muxihuayi.cn

[Q17] 条件查询
来源：http://yu.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kr.haigaiapp.cn

[Q18] 模糊匹配
来源：http://he.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ii.shxzukj.cn

[Q19] 范围查询
来源：http://yb.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yb.bjjhwx.cn

[Q20] IN 列表
来源：http://fb.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fl.shxzskj.cn

[Q21] 空值判断
来源：http://im.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jw.bjjhwx.cn

[Q22] 排序
来源：http://re.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bc.nszjky.cn

[Q23] 分页
来源：http://vh.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dz.jctech888.com.cn

[Q24] 去重
来源：http://qw.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://zr.nszjky.cn

[Q25] 只取前 N 条
来源：http://wv.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tq.szxytkj.cn

[Q26] 计数
来源：http://pt.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://ia.asd995.cn

[Q27] 条件计数
来源：http://rr.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pq.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://bo.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bw.colortex.cn

[Q29] 最大最小值
来源：http://kr.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ut.shtwfgs.cn

[Q30] 分组统计
来源：http://or.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://px.shtwfgs.cn

[Q31] 分组后过滤
来源：http://ff.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fk.szsharing.cn

[Q32] 分组拼接字符串
来源：http://df.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zd.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fm.yuntaijiaju.cn

[Q33] 多列分组
来源：http://jx.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ty.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://bs.hnjuh.cn

SELECT * FROM (
来源：http://nh.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cy.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://so.colortex.cn

[Q35] 内连接
来源：http://sh.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nd.gzmigu.cn

[Q36] 左连接
来源：http://fk.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nl.lnxyls.cn

[Q37] 右连接
来源：http://nv.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ye.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qb.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qt.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://oe.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://st.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hk.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ji.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wu.hnjuh.cn

[Q41] 多表连接
来源：http://xs.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ar.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://oj.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://wx.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://os.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://vk.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xf.gzmigu.cn

[Q43] 标量子查询
来源：http://ur.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oe.9csxet.cn

[Q44] IN 子查询
来源：http://jg.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bp.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://il.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lz.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cc.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.lnxyls.cn

[Q47] 与平均值比较
来源：http://bu.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lp.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://fv.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ei.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://xt.haigaiapp.cn

[Q49] 更新单行
来源：http://mk.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tl.gzmigu.cn

[Q50] 批量更新
来源：http://to.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ph.9csxet.cn

[Q51] 用子查询更新
来源：http://jo.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vl.bookmarksfly.cn

[Q52] 删除指定行
来源：http://nz.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://xz.nicolike.cn

[Q53] 按条件删除
来源：http://mp.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gx.hahajie.cn

[Q54] 清空表
来源：http://bj.huanxung.cn

TRUNCATE TABLE logs;
来源：http://mq.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://hn.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eo.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://li.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mv.jctech888.com.cn

[Q57] 行号
来源：http://pf.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ec.shtwfgs.cn

[Q58] 累计求和
来源：http://ie.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fp.colortex.cn

[Q59] 分组内累计
来源：http://kd.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ux.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://qc.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dg.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nu.chemitech.net.cn

[Q61] 移动平均
来源：http://up.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pi.bjjhwx.cn

[Q62] 分组占比
来源：http://pq.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wu.colortex.cn

[Q63] 开启事务
来源：http://fv.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rw.jianghongdianzi.cn

[Q64] 提交事务
来源：http://ob.gzmigu.cn

COMMIT;
来源：http://zg.hnjuh.cn

[Q65] 回滚事务
来源：http://zn.jianghongdianzi.cn

ROLLBACK;
来源：http://iu.muxihuayi.cn

[Q66] 行锁查询
来源：http://pv.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jo.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://np.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hh.chemitech.net.cn

[Q68] 保存点
来源：http://qs.nszjky.cn

SAVEPOINT sp1;
来源：http://nz.szxytkj.cn


<!-- 参考信息 -->