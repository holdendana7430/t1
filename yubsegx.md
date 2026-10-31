代发 wailian999

[O02] 使用线程池
来源：http://an.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wy.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xq.9csxet.cn

JS:   // worker_threads 线程池
来源：http://gk.nicolike.cn

TS:   // worker_threads 线程池
来源：http://do.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sb.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cx.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hq.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sa.szsharing.cn

[O03] 加锁保护共享数据
来源：http://mh.nicolike.cn

Py:   with lock: shared += 1
来源：http://oc.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://eg.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dh.9csxet.cn

TS:   // 同 JS
来源：http://if.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://xr.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pi.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sg.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://of.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://vp.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://zk.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://js.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://lh.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wr.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mx.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kk.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://te.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://sg.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://av.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://vv.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dm.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://bx.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://qf.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pm.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jc.521024.cn

Ruby: threads.map(&:join)
来源：http://ts.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://of.nszjky.cn

[O06] 使用进程池
来源：http://lz.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bm.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bd.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://sn.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://oy.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://su.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mp.huixinmuqiang.cn

Ruby: // fork 块
来源：http://pe.nszjky.cn

C#:   Parallel.For
来源：http://ku.bookmarksfly.cn

================================================================================
来源：http://ze.wgjwhj.cn

P. 常用工具函数
来源：http://wn.chemitech.net.cn

================================================================================
来源：http://dn.yuexingan06.cn

[P01] 生成 UUID
来源：http://ww.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://tv.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ta.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ir.szsharing.cn

TS:   crypto.randomUUID()
来源：http://ck.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://dp.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://ot.521024.cn

Ruby: SecureRandom.uuid
来源：http://iy.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://is.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://gz.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://re.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hr.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ss.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cy.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vd.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://az.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://od.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xg.9csxet.cn

[P03] 生成短随机字符串
来源：http://fr.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ic.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vo.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vc.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gh.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hi.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://if.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://em.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rw.huixinmuqiang.cn

[P04] 求长度
来源：http://wj.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cg.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ek.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ts.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lf.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://br.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://ea.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://qr.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://aa.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://dq.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cv.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wr.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gd.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vw.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ka.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cp.huanxung.cn

Ruby: a == b
来源：http://kl.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ze.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wk.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gm.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://ok.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://df.szxytkj.cn

TS:   if (x == null) {}
来源：http://wf.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gs.asd995.cn

Go:   if x == nil {}
来源：http://yz.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pe.muxihuayi.cn

C#:   if (x is null) {}
来源：http://sf.wgjwhj.cn

[P07] 防抖与节流
来源：http://ma.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lh.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://oa.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eo.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qd.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://an.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uz.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ro.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://in.hahajie.cn

[P08] 处理浮点精度问题
来源：http://nb.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mr.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ga.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ul.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sa.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iw.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nf.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cl.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ld.asd995.cn

================================================================================
来源：http://ed.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tt.hahajie.cn

================================================================================
来源：http://es.lnxyls.cn

[Q01] 创建表
来源：http://yc.szxytkj.cn

CREATE TABLE users (
来源：http://ym.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yq.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ou.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://gu.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zt.shtwfgs.cn

);
来源：http://kz.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://if.shxzskj.cn

CREATE TABLE orders (
来源：http://ek.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rv.haigaiapp.cn

user_id INT NOT NULL,
来源：http://yr.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://ue.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cz.gzmigu.cn

);
来源：http://eg.panjiajie.cn

[Q03] 增加列
来源：http://wi.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jm.9csxet.cn

[Q04] 修改列类型
来源：http://th.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hg.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ze.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://px.hnjuh.cn

[Q06] 删除列
来源：http://dn.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ix.bookmarksfly.cn

[Q07] 删除表
来源：http://vs.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://gi.shxzukj.cn

[Q08] 创建普通索引
来源：http://tg.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rm.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://fi.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dk.nszjky.cn

[Q10] 插入单行
来源：http://gq.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fi.szsharing.cn

[Q11] 一次插入多行
来源：http://lw.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://th.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://qa.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xf.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dk.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://fo.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rb.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://la.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ki.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gx.asd995.cn

[Q15] 查询全部
来源：http://ij.huixiangedu.cn

SELECT * FROM users;
来源：http://yt.szsharing.cn

[Q16] 查询指定列
来源：http://yw.haigaiapp.cn

SELECT id, name FROM users;
来源：http://vo.hahajie.cn

[Q17] 条件查询
来源：http://io.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ya.hnjuh.cn

[Q18] 模糊匹配
来源：http://bw.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ym.szsharing.cn

[Q19] 范围查询
来源：http://yz.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zt.haigaiapp.cn

[Q20] IN 列表
来源：http://cy.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fk.shxzskj.cn

[Q21] 空值判断
来源：http://nj.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://la.9csxet.cn

[Q22] 排序
来源：http://bf.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zn.nicolike.cn

[Q23] 分页
来源：http://cm.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nl.nicolike.cn

[Q24] 去重
来源：http://cn.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://xe.lnxyls.cn

[Q25] 只取前 N 条
来源：http://yt.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rh.huixiangedu.cn

[Q26] 计数
来源：http://jo.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://rt.9csxet.cn

[Q27] 条件计数
来源：http://wt.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mq.newstarts.cn

[Q28] 求和与平均
来源：http://et.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://um.asd995.cn

[Q29] 最大最小值
来源：http://jk.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pr.yuntaijiaju.cn

[Q30] 分组统计
来源：http://vh.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ho.jctech888.com.cn

[Q31] 分组后过滤
来源：http://df.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wy.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://kn.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hr.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yp.szsharing.cn

[Q33] 多列分组
来源：http://el.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kk.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://ob.huixinmuqiang.cn

SELECT * FROM (
来源：http://pm.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wx.yuexingan06.cn

) t WHERE rn = 1;
来源：http://tp.nszjky.cn

[Q35] 内连接
来源：http://lv.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fj.bjjhwx.cn

[Q36] 左连接
来源：http://de.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bo.shxzukj.cn

[Q37] 右连接
来源：http://wg.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bo.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nv.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vt.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://wo.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hq.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tv.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xt.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qv.newstarts.cn

[Q41] 多表连接
来源：http://rs.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ie.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://pl.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://sc.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://hp.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://va.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oz.huanxung.cn

[Q43] 标量子查询
来源：http://zu.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vj.521024.cn

[Q44] IN 子查询
来源：http://th.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bq.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://sq.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eb.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bp.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jx.bjjhwx.cn

[Q47] 与平均值比较
来源：http://xo.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gd.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://dw.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lb.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://zn.colortex.cn

[Q49] 更新单行
来源：http://no.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xf.bookmarksfly.cn

[Q50] 批量更新
来源：http://bq.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rm.nicolike.cn

[Q51] 用子查询更新
来源：http://qi.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ay.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://bq.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://lk.huanxung.cn

[Q53] 按条件删除
来源：http://kc.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://da.yuexingan06.cn

[Q54] 清空表
来源：http://ux.szsharing.cn

TRUNCATE TABLE logs;
来源：http://xk.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://bt.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fy.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://ly.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ep.521024.cn

[Q57] 行号
来源：http://fe.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rd.wgjwhj.cn

[Q58] 累计求和
来源：http://xl.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qn.huixiangedu.cn

[Q59] 分组内累计
来源：http://xx.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fs.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://fd.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fl.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mt.yuexingan06.cn

[Q61] 移动平均
来源：http://fb.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://li.huixinmuqiang.cn

[Q62] 分组占比
来源：http://cp.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jk.wgjwhj.cn

[Q63] 开启事务
来源：http://ls.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xv.huixiangedu.cn

[Q64] 提交事务
来源：http://pe.wgjwhj.cn

COMMIT;
来源：http://nn.szxytkj.cn

[Q65] 回滚事务
来源：http://ws.bjjhwx.cn

ROLLBACK;
来源：http://lt.jctech888.com.cn

[Q66] 行锁查询
来源：http://yk.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jf.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://wq.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://el.yuntaijiaju.cn

[Q68] 保存点
来源：http://lq.nicolike.cn

SAVEPOINT sp1;
来源：http://jd.colortex.cn

ROLLBACK TO sp1;
来源：http://jp.shtwfgs.cn

[Q69] 查看执行计划
来源：http://qz.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cd.wgjwhj.cn

[Q70] 更新统计信息
来源：http://pu.szxytkj.cn

ANALYZE TABLE users;
来源：http://gq.nicolike.cn

[Q71] 查看建表语句
来源：http://bm.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tq.bjjhwx.cn

[Q72] 查看索引
来源：http://ep.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://if.wgjwhj.cn

[Q73] 查看表状态
来源：http://uy.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yx.wgjwhj.cn

[Q74] 强制使用索引
来源：http://fz.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://by.szsharing.cn

[Q75] 日期格式化
来源：http://bl.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mi.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tk.huixiangedu.cn

[Q76] 按天统计
来源：http://mg.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wr.nszjky.cn

[Q77] 时间加减
来源：http://my.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yy.521024.cn


<!-- 参考信息 -->