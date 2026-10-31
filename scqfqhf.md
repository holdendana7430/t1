代发 wailian999

[O02] 使用线程池
来源：http://xz.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sy.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ys.huanxung.cn

JS:   // worker_threads 线程池
来源：http://dm.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://zp.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mn.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qy.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ah.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jm.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://kt.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://dg.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://vq.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://en.huixiangedu.cn

TS:   // 同 JS
来源：http://zw.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://du.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fh.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oc.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://zq.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://gw.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://vl.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aw.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://zf.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://er.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qh.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zw.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kl.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://ax.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://mp.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://xo.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uj.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://gi.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://on.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fx.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oa.colortex.cn

Ruby: threads.map(&:join)
来源：http://mc.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zq.newstarts.cn

[O06] 使用进程池
来源：http://pw.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oh.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://if.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://jl.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://lh.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ei.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cu.nszjky.cn

Ruby: // fork 块
来源：http://zw.newstarts.cn

C#:   Parallel.For
来源：http://sk.muxihuayi.cn

================================================================================
来源：http://bg.yuntaijiaju.cn

P. 常用工具函数
来源：http://jo.haigaiapp.cn

================================================================================
来源：http://sh.huanxung.cn

[P01] 生成 UUID
来源：http://rb.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://gp.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hb.hahajie.cn

JS:   crypto.randomUUID()
来源：http://ja.szsharing.cn

TS:   crypto.randomUUID()
来源：http://rp.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://zc.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://jz.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://yo.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://hy.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://ig.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uy.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gm.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sv.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uk.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lx.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vz.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lm.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pc.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://ta.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rl.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sn.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ru.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ex.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sx.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ns.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tv.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lq.wgjwhj.cn

[P04] 求长度
来源：http://ig.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ac.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ye.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ki.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aw.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://cv.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://oz.panjiajie.cn

Ruby: x.length;  x.size
来源：http://pf.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hr.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://su.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iq.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pz.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zr.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bi.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://io.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lv.shxzukj.cn

Ruby: a == b
来源：http://ic.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wf.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jw.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dg.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://nc.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://os.szxytkj.cn

TS:   if (x == null) {}
来源：http://kc.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ed.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://lb.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pm.521024.cn

C#:   if (x is null) {}
来源：http://kn.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://fz.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rj.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://qh.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oj.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vu.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://li.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cg.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sr.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uc.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://hd.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wh.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tb.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gt.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fm.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hn.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sa.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jj.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ez.bjjhwx.cn

================================================================================
来源：http://ca.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tn.szxytkj.cn

================================================================================
来源：http://fu.shxzskj.cn

[Q01] 创建表
来源：http://kl.jianghongdianzi.cn

CREATE TABLE users (
来源：http://tz.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ht.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://ap.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://fs.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gs.9csxet.cn

);
来源：http://wc.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://td.wgjwhj.cn

CREATE TABLE orders (
来源：http://fg.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lq.shxzukj.cn

user_id INT NOT NULL,
来源：http://ke.asd995.cn

amount DECIMAL(10, 2),
来源：http://uk.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rg.panjiajie.cn

);
来源：http://nr.szxytkj.cn

[Q03] 增加列
来源：http://xe.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pe.shtwfgs.cn

[Q04] 修改列类型
来源：http://lo.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jy.yuexingan06.cn

[Q05] 重命名列
来源：http://yt.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rg.panjiajie.cn

[Q06] 删除列
来源：http://ue.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://po.lnxyls.cn

[Q07] 删除表
来源：http://iw.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://ha.nszjky.cn

[Q08] 创建普通索引
来源：http://xv.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aa.521024.cn

[Q09] 创建唯一索引
来源：http://mf.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ur.lnxyls.cn

[Q10] 插入单行
来源：http://if.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xc.shxzukj.cn

[Q11] 一次插入多行
来源：http://dg.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://am.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://yn.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pz.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fz.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://qs.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lc.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://kt.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hf.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vh.szxytkj.cn

[Q15] 查询全部
来源：http://jg.521024.cn

SELECT * FROM users;
来源：http://ay.bookmarksfly.cn

[Q16] 查询指定列
来源：http://sz.chemitech.net.cn

SELECT id, name FROM users;
来源：http://sj.bookmarksfly.cn

[Q17] 条件查询
来源：http://kz.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yn.huixiangedu.cn

[Q18] 模糊匹配
来源：http://xz.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mb.chemitech.net.cn

[Q19] 范围查询
来源：http://tr.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dm.newstarts.cn

[Q20] IN 列表
来源：http://vx.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pg.hahajie.cn

[Q21] 空值判断
来源：http://ko.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jo.panjiajie.cn

[Q22] 排序
来源：http://rd.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nr.huixiangedu.cn

[Q23] 分页
来源：http://px.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qv.huixinmuqiang.cn

[Q24] 去重
来源：http://lq.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://bl.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://vq.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fz.shtwfgs.cn

[Q26] 计数
来源：http://vm.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://nb.muxihuayi.cn

[Q27] 条件计数
来源：http://dj.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vu.nicolike.cn

[Q28] 求和与平均
来源：http://lt.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zu.lnxyls.cn

[Q29] 最大最小值
来源：http://ja.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://us.bjjhwx.cn

[Q30] 分组统计
来源：http://qm.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ij.huanxung.cn

[Q31] 分组后过滤
来源：http://hw.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tf.hahajie.cn

[Q32] 分组拼接字符串
来源：http://oj.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dq.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://us.jctech888.com.cn

[Q33] 多列分组
来源：http://jm.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yz.521024.cn

[Q34] 每组取第一条
来源：http://dk.521024.cn

SELECT * FROM (
来源：http://sg.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fo.bjjhwx.cn

) t WHERE rn = 1;
来源：http://cm.colortex.cn

[Q35] 内连接
来源：http://po.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pb.huanxung.cn

[Q36] 左连接
来源：http://jp.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wn.jctech888.com.cn

[Q37] 右连接
来源：http://hx.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ma.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qp.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fj.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://xg.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xv.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qf.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hj.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ht.bjjhwx.cn

[Q41] 多表连接
来源：http://wk.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fb.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://en.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://fn.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://ou.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://vt.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gb.huixiangedu.cn

[Q43] 标量子查询
来源：http://um.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pk.lnxyls.cn

[Q44] IN 子查询
来源：http://my.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ed.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://bc.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sl.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fc.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sn.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://tg.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ii.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://fc.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xd.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://bc.hnjuh.cn

[Q49] 更新单行
来源：http://vb.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zk.yuexingan06.cn

[Q50] 批量更新
来源：http://kx.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dp.colortex.cn

[Q51] 用子查询更新
来源：http://ct.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mo.huixiangedu.cn

[Q52] 删除指定行
来源：http://pc.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://lk.shxzskj.cn

[Q53] 按条件删除
来源：http://pe.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ct.wgjwhj.cn

[Q54] 清空表
来源：http://wp.newstarts.cn

TRUNCATE TABLE logs;
来源：http://sx.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://vo.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yq.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://lz.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tu.bjjhwx.cn

[Q57] 行号
来源：http://uv.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lr.chemitech.net.cn

[Q58] 累计求和
来源：http://ya.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jq.colortex.cn

[Q59] 分组内累计
来源：http://xc.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ic.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://je.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hn.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zq.huixiangedu.cn

[Q61] 移动平均
来源：http://nl.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yu.muxihuayi.cn

[Q62] 分组占比
来源：http://hy.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gj.nicolike.cn

[Q63] 开启事务
来源：http://sd.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qi.muxihuayi.cn

[Q64] 提交事务
来源：http://it.szxytkj.cn

COMMIT;
来源：http://fj.lnxyls.cn

[Q65] 回滚事务
来源：http://rc.nicolike.cn

ROLLBACK;
来源：http://wi.panjiajie.cn

[Q66] 行锁查询
来源：http://mu.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jh.lnxyls.cn

[Q67] 设置隔离级别
来源：http://aw.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nu.szsharing.cn

[Q68] 保存点
来源：http://he.shxzukj.cn

SAVEPOINT sp1;
来源：http://vw.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://ew.panjiajie.cn

[Q69] 查看执行计划
来源：http://th.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://id.huixiangedu.cn

[Q70] 更新统计信息
来源：http://yq.nszjky.cn

ANALYZE TABLE users;
来源：http://oh.muxihuayi.cn

[Q71] 查看建表语句
来源：http://zz.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cy.muxihuayi.cn

[Q72] 查看索引
来源：http://ng.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://id.panjiajie.cn

[Q73] 查看表状态
来源：http://wv.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ed.asd995.cn

[Q74] 强制使用索引
来源：http://zk.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xs.shxzskj.cn

[Q75] 日期格式化
来源：http://cz.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qr.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dz.wgjwhj.cn

[Q76] 按天统计
来源：http://kf.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qr.yuexingan06.cn

[Q77] 时间加减
来源：http://cm.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://za.nszjky.cn


<!-- 参考信息 -->