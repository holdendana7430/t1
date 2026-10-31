代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vy.chemitech.net.cn

TS:   // 同 JS
来源：http://jr.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://mn.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bp.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wv.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://ti.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://ww.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://tl.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ja.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://hx.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://al.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zd.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dj.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://lp.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://yw.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://lp.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://it.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://la.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://mc.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aa.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jd.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://ba.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eh.yuexingan06.cn

[O06] 使用进程池
来源：http://bg.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xo.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kl.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://cj.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://gg.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mv.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ph.shxzukj.cn

Ruby: // fork 块
来源：http://kl.jctech888.com.cn

C#:   Parallel.For
来源：http://xt.shxzukj.cn

================================================================================
来源：http://ir.yuntaijiaju.cn

P. 常用工具函数
来源：http://sl.muxihuayi.cn

================================================================================
来源：http://hr.huixiangedu.cn

[P01] 生成 UUID
来源：http://zj.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://vk.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xw.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://ue.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://la.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://nn.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://zq.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://mh.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://eq.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://nb.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yl.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uy.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bm.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ei.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ft.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ns.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://me.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://im.szsharing.cn

[P03] 生成短随机字符串
来源：http://vf.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cl.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hu.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://li.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eq.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vs.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gt.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nk.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qz.colortex.cn

[P04] 求长度
来源：http://tt.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ys.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ii.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hv.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://no.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://wg.nicolike.cn

Go:   len(arr);  len(m)
来源：http://nx.nszjky.cn

Ruby: x.length;  x.size
来源：http://tm.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bj.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://or.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wh.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ln.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ti.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rk.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ff.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xr.521024.cn

Ruby: a == b
来源：http://dx.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aq.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ld.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bt.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://sn.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bc.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://za.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rm.panjiajie.cn

Go:   if x == nil {}
来源：http://do.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zq.gzmigu.cn

C#:   if (x is null) {}
来源：http://gi.gzmigu.cn

[P07] 防抖与节流
来源：http://er.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mm.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://at.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tl.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eu.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xo.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://du.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pn.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://li.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://mg.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://te.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pc.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hw.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wi.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gg.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ky.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lp.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uf.szxytkj.cn

================================================================================
来源：http://sb.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xt.shtwfgs.cn

================================================================================
来源：http://oo.huixiangedu.cn

[Q01] 创建表
来源：http://kv.yuntaijiaju.cn

CREATE TABLE users (
来源：http://km.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://er.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://ls.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://eo.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mj.jianghongdianzi.cn

);
来源：http://mg.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://us.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://wl.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yz.huanxung.cn

user_id INT NOT NULL,
来源：http://mq.huanxung.cn

amount DECIMAL(10, 2),
来源：http://bs.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://md.wgjwhj.cn

);
来源：http://dx.panjiajie.cn

[Q03] 增加列
来源：http://io.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ub.gzmigu.cn

[Q04] 修改列类型
来源：http://uc.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ex.szsharing.cn

[Q05] 重命名列
来源：http://sy.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qo.shxzukj.cn

[Q06] 删除列
来源：http://ez.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vr.521024.cn

[Q07] 删除表
来源：http://vc.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://ua.jctech888.com.cn

[Q08] 创建普通索引
来源：http://qc.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lr.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://fn.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://es.colortex.cn

[Q10] 插入单行
来源：http://gj.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ep.gzmigu.cn

[Q11] 一次插入多行
来源：http://hp.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rf.colortex.cn

[Q12] 插入后取自增 ID
来源：http://hh.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kr.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://os.shxzskj.cn

[Q13] 忽略重复插入
来源：http://pi.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qo.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://kc.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ze.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wf.hahajie.cn

[Q15] 查询全部
来源：http://vp.huixinmuqiang.cn

SELECT * FROM users;
来源：http://kr.haigaiapp.cn

[Q16] 查询指定列
来源：http://xf.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://wg.newstarts.cn

[Q17] 条件查询
来源：http://lj.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wa.nicolike.cn

[Q18] 模糊匹配
来源：http://mg.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://io.nicolike.cn

[Q19] 范围查询
来源：http://xv.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tb.haigaiapp.cn

[Q20] IN 列表
来源：http://in.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://da.yuexingan06.cn

[Q21] 空值判断
来源：http://yz.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pr.9csxet.cn

[Q22] 排序
来源：http://kg.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rn.haigaiapp.cn

[Q23] 分页
来源：http://rz.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dt.yuntaijiaju.cn

[Q24] 去重
来源：http://wk.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://ck.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://un.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ho.bookmarksfly.cn

[Q26] 计数
来源：http://wd.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://zl.huixiangedu.cn

[Q27] 条件计数
来源：http://jt.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dt.chemitech.net.cn

[Q28] 求和与平均
来源：http://vj.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://za.newstarts.cn

[Q29] 最大最小值
来源：http://cc.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pm.huixiangedu.cn

[Q30] 分组统计
来源：http://or.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sl.haigaiapp.cn

[Q31] 分组后过滤
来源：http://uk.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ii.9csxet.cn

[Q32] 分组拼接字符串
来源：http://vt.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ub.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ae.newstarts.cn

[Q33] 多列分组
来源：http://rp.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ex.nicolike.cn

[Q34] 每组取第一条
来源：http://px.yuexingan06.cn

SELECT * FROM (
来源：http://sn.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yz.shtwfgs.cn

) t WHERE rn = 1;
来源：http://nm.gzmigu.cn

[Q35] 内连接
来源：http://wz.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ql.jctech888.com.cn

[Q36] 左连接
来源：http://px.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pa.shxzukj.cn

[Q37] 右连接
来源：http://vm.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ms.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qy.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sz.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://aq.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lv.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dz.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fb.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cx.bjjhwx.cn

[Q41] 多表连接
来源：http://au.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fh.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://xq.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://no.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://fa.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://hg.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ow.jctech888.com.cn

[Q43] 标量子查询
来源：http://pe.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rz.newstarts.cn

[Q44] IN 子查询
来源：http://ql.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ui.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://qt.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sp.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wd.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://po.521024.cn

[Q47] 与平均值比较
来源：http://en.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ny.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://eu.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ga.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://qh.9csxet.cn

[Q49] 更新单行
来源：http://xs.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qm.jianghongdianzi.cn

[Q50] 批量更新
来源：http://dt.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gc.huixiangedu.cn

[Q51] 用子查询更新
来源：http://sl.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://he.bookmarksfly.cn

[Q52] 删除指定行
来源：http://ku.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://ix.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://vb.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eo.asd995.cn

[Q54] 清空表
来源：http://ag.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://sz.szsharing.cn

[Q55] 排名（并列占位）
来源：http://pc.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cq.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://lm.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fj.hnjuh.cn

[Q57] 行号
来源：http://yy.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://am.nszjky.cn

[Q58] 累计求和
来源：http://bq.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yv.huixiangedu.cn

[Q59] 分组内累计
来源：http://aw.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aw.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://rz.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kv.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iz.bookmarksfly.cn

[Q61] 移动平均
来源：http://hd.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pm.asd995.cn

[Q62] 分组占比
来源：http://rv.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nf.shxzukj.cn

[Q63] 开启事务
来源：http://bf.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mg.lnxyls.cn

[Q64] 提交事务
来源：http://bf.shtwfgs.cn

COMMIT;
来源：http://zz.nicolike.cn

[Q65] 回滚事务
来源：http://me.muxihuayi.cn

ROLLBACK;
来源：http://on.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://vc.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ps.shxzukj.cn

[Q67] 设置隔离级别
来源：http://ya.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dy.huanxung.cn

[Q68] 保存点
来源：http://xc.lnxyls.cn

SAVEPOINT sp1;
来源：http://vy.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://ls.huanxung.cn

[Q69] 查看执行计划
来源：http://ae.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xb.nicolike.cn

[Q70] 更新统计信息
来源：http://sv.asd995.cn

ANALYZE TABLE users;
来源：http://tu.hnjuh.cn

[Q71] 查看建表语句
来源：http://iy.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rv.szxytkj.cn

[Q72] 查看索引
来源：http://lr.521024.cn

SHOW INDEX FROM users;
来源：http://bv.9csxet.cn

[Q73] 查看表状态
来源：http://rn.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hy.chemitech.net.cn

[Q74] 强制使用索引
来源：http://cj.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xo.shxzukj.cn

[Q75] 日期格式化
来源：http://hr.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ea.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oj.nszjky.cn

[Q76] 按天统计
来源：http://ka.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bz.wgjwhj.cn

[Q77] 时间加减
来源：http://cr.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wq.huanxung.cn

[Q78] 当前时间
来源：http://so.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bs.9csxet.cn

[Q79] 字符串拼接
来源：http://ni.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://il.shxzukj.cn

[Q80] 字符串截取
来源：http://pj.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ty.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://ix.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iy.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://mc.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ie.lnxyls.cn

[Q83] 大小写转换
来源：http://yw.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jt.jctech888.com.cn


<!-- 参考信息 -->