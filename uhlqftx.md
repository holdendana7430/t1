代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ib.newstarts.cn

TS:   // 同 JS
来源：http://wx.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://vk.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ww.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zj.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://uz.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://dd.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://up.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fq.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://wj.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sc.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://on.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://de.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fg.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://nj.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://xv.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://qv.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rk.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://ud.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://fq.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ox.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hl.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://ks.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yd.shxzukj.cn

[O06] 使用进程池
来源：http://pi.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nx.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qd.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://sx.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://dm.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ez.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ao.9csxet.cn

Ruby: // fork 块
来源：http://ni.jianghongdianzi.cn

C#:   Parallel.For
来源：http://gc.bookmarksfly.cn

================================================================================
来源：http://sn.yuexingan06.cn

P. 常用工具函数
来源：http://bk.gzmigu.cn

================================================================================
来源：http://ci.shtwfgs.cn

[P01] 生成 UUID
来源：http://wq.asd995.cn

Py:   str(uuid.uuid4())
来源：http://px.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mm.521024.cn

JS:   crypto.randomUUID()
来源：http://zj.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://jf.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://ai.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://gt.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://xm.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://mp.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://fu.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sl.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ia.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pp.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wv.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://si.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tc.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rk.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://vo.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vm.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ft.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://is.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ti.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xf.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nz.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gv.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ch.nszjky.cn

[P04] 求长度
来源：http://gd.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mj.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pr.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bu.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kq.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://ll.521024.cn

Go:   len(arr);  len(m)
来源：http://zh.gzmigu.cn

Ruby: x.length;  x.size
来源：http://yc.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ur.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://kb.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wu.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fr.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ny.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qn.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ie.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ey.huixiangedu.cn

Ruby: a == b
来源：http://zl.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pt.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jm.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bg.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://az.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xe.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://bd.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jt.szsharing.cn

Go:   if x == nil {}
来源：http://wz.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hx.hahajie.cn

C#:   if (x is null) {}
来源：http://ay.bjjhwx.cn

[P07] 防抖与节流
来源：http://ba.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wb.521024.cn

PHP:  // 手写时间戳比较
来源：http://re.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uk.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://td.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zo.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xc.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qd.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gh.asd995.cn

[P08] 处理浮点精度问题
来源：http://kj.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://as.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yb.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gr.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ci.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ar.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cy.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wp.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tu.lnxyls.cn

================================================================================
来源：http://te.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jb.chemitech.net.cn

================================================================================
来源：http://rh.gzmigu.cn

[Q01] 创建表
来源：http://uh.shxzukj.cn

CREATE TABLE users (
来源：http://zr.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://za.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://pb.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://mm.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lr.jianghongdianzi.cn

);
来源：http://iu.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://wp.wgjwhj.cn

CREATE TABLE orders (
来源：http://mw.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jh.gzmigu.cn

user_id INT NOT NULL,
来源：http://ib.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://uu.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mx.huanxung.cn

);
来源：http://do.jianghongdianzi.cn

[Q03] 增加列
来源：http://ua.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oh.szxytkj.cn

[Q04] 修改列类型
来源：http://mv.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://od.bjjhwx.cn

[Q05] 重命名列
来源：http://qn.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ev.newstarts.cn

[Q06] 删除列
来源：http://rq.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gf.bjjhwx.cn

[Q07] 删除表
来源：http://zj.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://jn.newstarts.cn

[Q08] 创建普通索引
来源：http://no.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gh.shxzukj.cn

[Q09] 创建唯一索引
来源：http://aq.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ra.9csxet.cn

[Q10] 插入单行
来源：http://uz.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ur.9csxet.cn

[Q11] 一次插入多行
来源：http://pq.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qh.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://kb.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ei.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://as.9csxet.cn

[Q13] 忽略重复插入
来源：http://dw.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aa.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://wv.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hc.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eo.panjiajie.cn

[Q15] 查询全部
来源：http://zh.colortex.cn

SELECT * FROM users;
来源：http://ft.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://pg.huixiangedu.cn

SELECT id, name FROM users;
来源：http://nu.chemitech.net.cn

[Q17] 条件查询
来源：http://ol.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nm.wgjwhj.cn

[Q18] 模糊匹配
来源：http://kr.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jk.nicolike.cn

[Q19] 范围查询
来源：http://tp.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tb.gzmigu.cn

[Q20] IN 列表
来源：http://ao.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ts.huixinmuqiang.cn

[Q21] 空值判断
来源：http://ki.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sy.panjiajie.cn

[Q22] 排序
来源：http://qx.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://th.bjjhwx.cn

[Q23] 分页
来源：http://pv.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ag.chemitech.net.cn

[Q24] 去重
来源：http://ku.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://zw.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://tx.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fg.chemitech.net.cn

[Q26] 计数
来源：http://fo.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://ck.hnjuh.cn

[Q27] 条件计数
来源：http://fl.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://by.nicolike.cn

[Q28] 求和与平均
来源：http://ds.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hx.panjiajie.cn

[Q29] 最大最小值
来源：http://xx.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xp.lnxyls.cn

[Q30] 分组统计
来源：http://uz.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qp.newstarts.cn

[Q31] 分组后过滤
来源：http://ue.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jg.521024.cn

[Q32] 分组拼接字符串
来源：http://xq.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://np.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oq.lnxyls.cn

[Q33] 多列分组
来源：http://zk.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gk.nszjky.cn

[Q34] 每组取第一条
来源：http://qt.shxzskj.cn

SELECT * FROM (
来源：http://ne.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://is.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://jv.colortex.cn

[Q35] 内连接
来源：http://du.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zq.shxzskj.cn

[Q36] 左连接
来源：http://ui.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jf.shxzskj.cn

[Q37] 右连接
来源：http://oy.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ou.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jx.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hf.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://ff.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rv.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ku.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ck.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ho.hahajie.cn

[Q41] 多表连接
来源：http://ae.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kq.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://dr.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://bf.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://fi.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://kd.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rf.szsharing.cn

[Q43] 标量子查询
来源：http://du.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gi.asd995.cn

[Q44] IN 子查询
来源：http://yv.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pi.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://ov.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rz.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sh.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uz.lnxyls.cn

[Q47] 与平均值比较
来源：http://wg.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://io.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://gh.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rd.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://nk.shtwfgs.cn

[Q49] 更新单行
来源：http://bm.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gy.wgjwhj.cn

[Q50] 批量更新
来源：http://mv.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ee.gzmigu.cn

[Q51] 用子查询更新
来源：http://qa.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://st.bjjhwx.cn

[Q52] 删除指定行
来源：http://xh.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://xz.nszjky.cn

[Q53] 按条件删除
来源：http://un.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wx.hahajie.cn

[Q54] 清空表
来源：http://ub.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://vk.521024.cn

[Q55] 排名（并列占位）
来源：http://wz.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zj.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ez.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cu.shtwfgs.cn

[Q57] 行号
来源：http://gr.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kb.muxihuayi.cn

[Q58] 累计求和
来源：http://lj.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hf.shtwfgs.cn

[Q59] 分组内累计
来源：http://ze.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zv.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://tk.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fb.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vu.hahajie.cn

[Q61] 移动平均
来源：http://el.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bm.huanxung.cn

[Q62] 分组占比
来源：http://ug.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nz.szxytkj.cn

[Q63] 开启事务
来源：http://ml.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ci.9csxet.cn

[Q64] 提交事务
来源：http://qa.jianghongdianzi.cn

COMMIT;
来源：http://wp.muxihuayi.cn

[Q65] 回滚事务
来源：http://yf.bjjhwx.cn

ROLLBACK;
来源：http://to.szsharing.cn

[Q66] 行锁查询
来源：http://gf.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fd.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://su.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://up.bookmarksfly.cn

[Q68] 保存点
来源：http://iy.shxzskj.cn

SAVEPOINT sp1;
来源：http://im.lnxyls.cn

ROLLBACK TO sp1;
来源：http://ne.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://ex.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xv.szsharing.cn

[Q70] 更新统计信息
来源：http://un.yuexingan06.cn

ANALYZE TABLE users;
来源：http://ok.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://wu.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mx.wgjwhj.cn

[Q72] 查看索引
来源：http://ls.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://hc.newstarts.cn

[Q73] 查看表状态
来源：http://aq.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://et.huixiangedu.cn

[Q74] 强制使用索引
来源：http://ox.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rd.hahajie.cn

[Q75] 日期格式化
来源：http://qy.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rg.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fr.colortex.cn

[Q76] 按天统计
来源：http://pa.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dl.szsharing.cn

[Q77] 时间加减
来源：http://el.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mr.huanxung.cn

[Q78] 当前时间
来源：http://jp.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://po.szxytkj.cn

[Q79] 字符串拼接
来源：http://uo.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wh.newstarts.cn

[Q80] 字符串截取
来源：http://lm.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ah.gzmigu.cn

[Q81] 字符串替换
来源：http://yf.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wi.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://wy.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yh.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://gp.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ol.colortex.cn


<!-- 参考信息 -->