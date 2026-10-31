代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://ml.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://vh.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://os.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://rn.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bl.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://ql.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oa.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yu.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dm.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vd.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://py.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://kh.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://un.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lg.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://np.asd995.cn

TS:   await Promise.all(tasks)
来源：http://sx.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qb.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ot.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://ca.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dg.hnjuh.cn

[O06] 使用进程池
来源：http://vv.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pt.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tj.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://ip.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://gg.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zn.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://om.jianghongdianzi.cn

Ruby: // fork 块
来源：http://ww.9csxet.cn

C#:   Parallel.For
来源：http://sc.szxytkj.cn

================================================================================
来源：http://lm.nicolike.cn

P. 常用工具函数
来源：http://oh.gzmigu.cn

================================================================================
来源：http://tf.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://vz.colortex.cn

Py:   str(uuid.uuid4())
来源：http://ag.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ev.szsharing.cn

JS:   crypto.randomUUID()
来源：http://de.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://iq.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://tb.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://hx.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://be.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ps.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://le.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xg.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fx.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oa.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mt.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://in.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ro.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zi.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zg.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://fp.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cv.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wm.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kc.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://st.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ux.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eq.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ie.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mm.hahajie.cn

[P04] 求长度
来源：http://uf.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ip.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jp.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hd.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pp.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://lj.newstarts.cn

Go:   len(arr);  len(m)
来源：http://jq.nicolike.cn

Ruby: x.length;  x.size
来源：http://nf.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bc.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://kn.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oh.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bg.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ux.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://je.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zg.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ry.colortex.cn

Ruby: a == b
来源：http://vr.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rf.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wy.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hd.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://my.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bl.szsharing.cn

TS:   if (x == null) {}
来源：http://ds.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ie.shxzskj.cn

Go:   if x == nil {}
来源：http://im.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fl.shxzukj.cn

C#:   if (x is null) {}
来源：http://qg.nszjky.cn

[P07] 防抖与节流
来源：http://vz.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tw.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://pd.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uq.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xo.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ur.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ep.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nq.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bh.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://zc.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qu.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zx.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ue.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ib.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://al.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sh.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xh.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xs.szsharing.cn

================================================================================
来源：http://hv.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gb.muxihuayi.cn

================================================================================
来源：http://fk.jianghongdianzi.cn

[Q01] 创建表
来源：http://xi.asd995.cn

CREATE TABLE users (
来源：http://rk.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://al.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://wf.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://ps.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rl.bookmarksfly.cn

);
来源：http://ds.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://bj.shxzskj.cn

CREATE TABLE orders (
来源：http://zb.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rx.nicolike.cn

user_id INT NOT NULL,
来源：http://bc.hahajie.cn

amount DECIMAL(10, 2),
来源：http://ew.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pq.bjjhwx.cn

);
来源：http://np.nicolike.cn

[Q03] 增加列
来源：http://ss.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ru.huanxung.cn

[Q04] 修改列类型
来源：http://ff.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qf.haigaiapp.cn

[Q05] 重命名列
来源：http://ct.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yh.panjiajie.cn

[Q06] 删除列
来源：http://ye.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://st.panjiajie.cn

[Q07] 删除表
来源：http://nq.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://xz.hnjuh.cn

[Q08] 创建普通索引
来源：http://cm.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oo.nszjky.cn

[Q09] 创建唯一索引
来源：http://lx.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rs.haigaiapp.cn

[Q10] 插入单行
来源：http://dh.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://nh.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://no.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://qu.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bj.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fw.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://zy.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rp.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://ab.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hv.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fo.jianghongdianzi.cn

[Q15] 查询全部
来源：http://if.521024.cn

SELECT * FROM users;
来源：http://or.nicolike.cn

[Q16] 查询指定列
来源：http://ea.panjiajie.cn

SELECT id, name FROM users;
来源：http://fa.huanxung.cn

[Q17] 条件查询
来源：http://pv.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xu.nicolike.cn

[Q18] 模糊匹配
来源：http://af.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bg.hahajie.cn

[Q19] 范围查询
来源：http://eq.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jn.chemitech.net.cn

[Q20] IN 列表
来源：http://ah.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ol.muxihuayi.cn

[Q21] 空值判断
来源：http://uq.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oe.yuexingan06.cn

[Q22] 排序
来源：http://qh.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jp.bookmarksfly.cn

[Q23] 分页
来源：http://yd.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ot.yuexingan06.cn

[Q24] 去重
来源：http://hl.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://zy.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://cx.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://td.jctech888.com.cn

[Q26] 计数
来源：http://to.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://cw.muxihuayi.cn

[Q27] 条件计数
来源：http://jg.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pq.newstarts.cn

[Q28] 求和与平均
来源：http://mv.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://la.newstarts.cn

[Q29] 最大最小值
来源：http://pz.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qs.muxihuayi.cn

[Q30] 分组统计
来源：http://ry.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vx.jctech888.com.cn

[Q31] 分组后过滤
来源：http://rm.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pd.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://ti.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fn.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mv.shxzskj.cn

[Q33] 多列分组
来源：http://zr.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xv.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ft.gzmigu.cn

SELECT * FROM (
来源：http://zc.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jm.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://ru.newstarts.cn

[Q35] 内连接
来源：http://ye.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gt.bjjhwx.cn

[Q36] 左连接
来源：http://dt.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mk.521024.cn

[Q37] 右连接
来源：http://fb.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qe.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://en.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://on.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://dp.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ax.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ei.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ue.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pt.muxihuayi.cn

[Q41] 多表连接
来源：http://dc.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gu.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://tq.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://jf.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://zm.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://ff.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mo.panjiajie.cn

[Q43] 标量子查询
来源：http://ve.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ud.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://ne.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jh.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://to.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://du.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mq.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rw.newstarts.cn

[Q47] 与平均值比较
来源：http://ze.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rn.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://sl.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uc.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://ye.hnjuh.cn

[Q49] 更新单行
来源：http://mf.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vn.hahajie.cn

[Q50] 批量更新
来源：http://iw.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://my.shxzskj.cn

[Q51] 用子查询更新
来源：http://db.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lt.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://rg.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://zv.bookmarksfly.cn

[Q53] 按条件删除
来源：http://gb.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uc.huixiangedu.cn

[Q54] 清空表
来源：http://bh.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://wi.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://br.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hf.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://kk.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zd.newstarts.cn

[Q57] 行号
来源：http://dy.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mr.szsharing.cn

[Q58] 累计求和
来源：http://ky.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vn.9csxet.cn

[Q59] 分组内累计
来源：http://mj.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://if.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://du.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vh.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hb.shxzukj.cn

[Q61] 移动平均
来源：http://tv.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xo.shxzukj.cn

[Q62] 分组占比
来源：http://xo.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lg.muxihuayi.cn

[Q63] 开启事务
来源：http://eh.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fi.yuexingan06.cn

[Q64] 提交事务
来源：http://gm.yuntaijiaju.cn

COMMIT;
来源：http://nm.jctech888.com.cn

[Q65] 回滚事务
来源：http://mt.shxzskj.cn

ROLLBACK;
来源：http://oe.gzmigu.cn

[Q66] 行锁查询
来源：http://vn.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iv.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://ty.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aq.bjjhwx.cn

[Q68] 保存点
来源：http://ol.nicolike.cn

SAVEPOINT sp1;
来源：http://rl.szxytkj.cn

ROLLBACK TO sp1;
来源：http://ek.huixiangedu.cn

[Q69] 查看执行计划
来源：http://xm.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sp.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://ir.hahajie.cn

ANALYZE TABLE users;
来源：http://bb.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://tq.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jx.huixiangedu.cn

[Q72] 查看索引
来源：http://ff.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://lm.jctech888.com.cn

[Q73] 查看表状态
来源：http://xu.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ep.panjiajie.cn

[Q74] 强制使用索引
来源：http://qi.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bu.shxzukj.cn

[Q75] 日期格式化
来源：http://rt.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fq.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ly.hahajie.cn

[Q76] 按天统计
来源：http://sa.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qb.muxihuayi.cn

[Q77] 时间加减
来源：http://kj.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://go.chemitech.net.cn

[Q78] 当前时间
来源：http://jd.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bn.521024.cn

[Q79] 字符串拼接
来源：http://tq.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hl.yuexingan06.cn

[Q80] 字符串截取
来源：http://vv.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bn.szsharing.cn

[Q81] 字符串替换
来源：http://yi.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ro.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://zv.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gv.szsharing.cn

[Q83] 大小写转换
来源：http://gh.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oj.huanxung.cn

[Q84] 去除首尾空格
来源：http://bt.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://eh.panjiajie.cn

[Q85] 数值取整
来源：http://nm.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rf.gzmigu.cn


<!-- 参考信息 -->