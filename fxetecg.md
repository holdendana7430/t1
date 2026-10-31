代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://in.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://qh.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://pk.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://gd.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kk.szsharing.cn

TS:   // 同 JS
来源：http://uk.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://tz.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ov.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xh.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://wk.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://hn.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://st.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jp.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://sp.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zo.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gf.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ru.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rv.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://pw.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://gi.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://kv.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pl.asd995.cn

JS:   await Promise.all(tasks)
来源：http://lc.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://om.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gl.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lb.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://nj.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bw.9csxet.cn

[O06] 使用进程池
来源：http://ez.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://th.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ef.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://kr.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://rh.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yw.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fw.bjjhwx.cn

Ruby: // fork 块
来源：http://qv.szsharing.cn

C#:   Parallel.For
来源：http://yu.bjjhwx.cn

================================================================================
来源：http://sd.nicolike.cn

P. 常用工具函数
来源：http://rq.yuexingan06.cn

================================================================================
来源：http://xo.hnjuh.cn

[P01] 生成 UUID
来源：http://ym.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://vy.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ap.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://qn.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://vq.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://xy.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://cj.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://ws.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://fv.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://pc.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cz.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zk.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ck.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://us.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zu.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kw.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ty.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ok.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://dz.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zw.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tw.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bf.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://po.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qy.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ra.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hw.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kp.huixiangedu.cn

[P04] 求长度
来源：http://hj.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iq.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lp.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hs.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nv.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://xm.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://kl.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://wx.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zr.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://bq.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ur.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jw.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gw.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ns.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ey.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://db.lnxyls.cn

Ruby: a == b
来源：http://vz.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bw.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://du.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vm.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://nq.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nb.huanxung.cn

TS:   if (x == null) {}
来源：http://bz.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mk.521024.cn

Go:   if x == nil {}
来源：http://do.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nc.szsharing.cn

C#:   if (x is null) {}
来源：http://ez.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://bk.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ob.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://cu.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kh.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kg.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ef.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vu.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zv.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qe.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://tq.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wz.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zg.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sj.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qx.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dn.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nw.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ug.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lf.newstarts.cn

================================================================================
来源：http://um.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xj.nszjky.cn

================================================================================
来源：http://rp.panjiajie.cn

[Q01] 创建表
来源：http://xf.asd995.cn

CREATE TABLE users (
来源：http://uf.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://of.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://qa.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://nr.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://os.9csxet.cn

);
来源：http://bs.lnxyls.cn

[Q02] 创建带外键的表
来源：http://jl.colortex.cn

CREATE TABLE orders (
来源：http://ew.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dj.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://ue.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://vb.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hy.yuntaijiaju.cn

);
来源：http://ij.huixiangedu.cn

[Q03] 增加列
来源：http://qg.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://er.shtwfgs.cn

[Q04] 修改列类型
来源：http://my.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xn.jianghongdianzi.cn

[Q05] 重命名列
来源：http://wv.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ql.chemitech.net.cn

[Q06] 删除列
来源：http://ic.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ih.shtwfgs.cn

[Q07] 删除表
来源：http://ht.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://xw.newstarts.cn

[Q08] 创建普通索引
来源：http://dx.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ki.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://kg.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sm.panjiajie.cn

[Q10] 插入单行
来源：http://at.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://li.jctech888.com.cn

[Q11] 一次插入多行
来源：http://iw.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ui.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://zl.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fu.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jv.hahajie.cn

[Q13] 忽略重复插入
来源：http://ta.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wv.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://ww.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ii.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ju.szxytkj.cn

[Q15] 查询全部
来源：http://nf.jctech888.com.cn

SELECT * FROM users;
来源：http://ed.haigaiapp.cn

[Q16] 查询指定列
来源：http://kb.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://qw.newstarts.cn

[Q17] 条件查询
来源：http://mh.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tj.szxytkj.cn

[Q18] 模糊匹配
来源：http://ug.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nz.muxihuayi.cn

[Q19] 范围查询
来源：http://gj.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wn.bjjhwx.cn

[Q20] IN 列表
来源：http://la.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fa.hnjuh.cn

[Q21] 空值判断
来源：http://ku.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wg.nszjky.cn

[Q22] 排序
来源：http://za.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gh.panjiajie.cn

[Q23] 分页
来源：http://cs.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mh.colortex.cn

[Q24] 去重
来源：http://ze.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://cv.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://lb.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bo.chemitech.net.cn

[Q26] 计数
来源：http://zp.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://ap.gzmigu.cn

[Q27] 条件计数
来源：http://ns.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wn.asd995.cn

[Q28] 求和与平均
来源：http://af.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ql.szsharing.cn

[Q29] 最大最小值
来源：http://an.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vu.chemitech.net.cn

[Q30] 分组统计
来源：http://vu.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jx.hnjuh.cn

[Q31] 分组后过滤
来源：http://wt.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xx.asd995.cn

[Q32] 分组拼接字符串
来源：http://wj.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ek.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vf.haigaiapp.cn

[Q33] 多列分组
来源：http://sg.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sy.haigaiapp.cn

[Q34] 每组取第一条
来源：http://nu.shxzskj.cn

SELECT * FROM (
来源：http://el.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gt.lnxyls.cn

) t WHERE rn = 1;
来源：http://vw.521024.cn

[Q35] 内连接
来源：http://ug.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://px.wgjwhj.cn

[Q36] 左连接
来源：http://dd.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tg.szxytkj.cn

[Q37] 右连接
来源：http://rn.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qa.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qf.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nl.521024.cn

[Q39] 自连接（查上下级）
来源：http://ke.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pl.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cu.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bq.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gj.yuntaijiaju.cn

[Q41] 多表连接
来源：http://yb.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gw.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://xb.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://rb.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://kr.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://li.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wv.chemitech.net.cn

[Q43] 标量子查询
来源：http://ih.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wv.jctech888.com.cn

[Q44] IN 子查询
来源：http://iw.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tx.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://rk.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ff.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sz.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vy.wgjwhj.cn

[Q47] 与平均值比较
来源：http://gb.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qw.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://zt.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sa.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://zr.szxytkj.cn

[Q49] 更新单行
来源：http://ti.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ov.jctech888.com.cn

[Q50] 批量更新
来源：http://hy.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bt.huanxung.cn

[Q51] 用子查询更新
来源：http://nu.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aa.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://rj.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://pn.shxzukj.cn

[Q53] 按条件删除
来源：http://hi.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fz.panjiajie.cn

[Q54] 清空表
来源：http://jk.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://ov.9csxet.cn

[Q55] 排名（并列占位）
来源：http://vs.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vq.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://vn.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pl.jianghongdianzi.cn

[Q57] 行号
来源：http://jo.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://es.jctech888.com.cn

[Q58] 累计求和
来源：http://dj.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gu.shxzukj.cn

[Q59] 分组内累计
来源：http://ao.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nt.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://bb.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gw.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eo.jctech888.com.cn

[Q61] 移动平均
来源：http://xg.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bu.asd995.cn

[Q62] 分组占比
来源：http://ak.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fd.wgjwhj.cn

[Q63] 开启事务
来源：http://wk.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ho.huanxung.cn

[Q64] 提交事务
来源：http://ph.asd995.cn

COMMIT;
来源：http://zo.bookmarksfly.cn

[Q65] 回滚事务
来源：http://bv.bjjhwx.cn

ROLLBACK;
来源：http://kh.chemitech.net.cn

[Q66] 行锁查询
来源：http://ln.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tl.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://qk.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://im.shxzskj.cn

[Q68] 保存点
来源：http://uy.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://ld.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://ei.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://oj.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hs.chemitech.net.cn

[Q70] 更新统计信息
来源：http://lz.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://zz.lnxyls.cn

[Q71] 查看建表语句
来源：http://xn.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fq.colortex.cn

[Q72] 查看索引
来源：http://ea.lnxyls.cn

SHOW INDEX FROM users;
来源：http://pf.chemitech.net.cn

[Q73] 查看表状态
来源：http://zu.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ma.shtwfgs.cn

[Q74] 强制使用索引
来源：http://wu.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cl.muxihuayi.cn

[Q75] 日期格式化
来源：http://sj.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dt.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ia.newstarts.cn

[Q76] 按天统计
来源：http://kd.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gp.huixiangedu.cn

[Q77] 时间加减
来源：http://dq.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rq.yuntaijiaju.cn

[Q78] 当前时间
来源：http://gq.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nq.shtwfgs.cn

[Q79] 字符串拼接
来源：http://bp.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tu.asd995.cn

[Q80] 字符串截取
来源：http://wo.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jc.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://cn.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dz.shtwfgs.cn


<!-- 参考信息 -->