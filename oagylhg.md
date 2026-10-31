代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://jr.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://zl.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://kc.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://hp.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ql.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://uv.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zi.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lv.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sf.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ld.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://ae.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://am.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://uo.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zv.colortex.cn

JS:   await Promise.all(tasks)
来源：http://aw.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://zd.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qy.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yw.colortex.cn

Ruby: threads.map(&:join)
来源：http://ra.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yv.colortex.cn

[O06] 使用进程池
来源：http://ng.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sx.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iv.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://pj.colortex.cn

TS:   // child_process / cluster 模块
来源：http://qd.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://du.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ym.haigaiapp.cn

Ruby: // fork 块
来源：http://wh.colortex.cn

C#:   Parallel.For
来源：http://su.lnxyls.cn

================================================================================
来源：http://ps.newstarts.cn

P. 常用工具函数
来源：http://nb.nszjky.cn

================================================================================
来源：http://vx.wgjwhj.cn

[P01] 生成 UUID
来源：http://oy.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://ud.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bw.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://wd.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://ix.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://oh.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://pj.asd995.cn

Ruby: SecureRandom.uuid
来源：http://je.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://jr.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://dw.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bf.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gq.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qk.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jb.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ur.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zk.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wz.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tb.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://ah.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kg.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eh.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dz.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xe.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wp.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bw.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xf.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ys.panjiajie.cn

[P04] 求长度
来源：http://yg.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tk.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://si.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rd.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yl.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://ii.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://xs.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://zn.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ir.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://qj.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ck.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ga.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ep.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sw.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kf.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hg.szsharing.cn

Ruby: a == b
来源：http://gz.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ca.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xh.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kq.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://ns.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cx.asd995.cn

TS:   if (x == null) {}
来源：http://yy.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fa.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://do.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lr.9csxet.cn

C#:   if (x is null) {}
来源：http://dk.muxihuayi.cn

[P07] 防抖与节流
来源：http://gt.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dt.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://po.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wy.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jb.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kp.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://os.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gy.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tl.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://vb.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xm.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wq.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kw.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rb.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yt.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pk.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rg.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qs.huixinmuqiang.cn

================================================================================
来源：http://rp.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xs.nszjky.cn

================================================================================
来源：http://ma.shtwfgs.cn

[Q01] 创建表
来源：http://bc.newstarts.cn

CREATE TABLE users (
来源：http://ag.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qh.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://ei.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://cb.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xx.huixiangedu.cn

);
来源：http://ud.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://sw.yuexingan06.cn

CREATE TABLE orders (
来源：http://jd.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yy.lnxyls.cn

user_id INT NOT NULL,
来源：http://ce.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://ec.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ou.jianghongdianzi.cn

);
来源：http://hp.nicolike.cn

[Q03] 增加列
来源：http://rm.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bz.huixiangedu.cn

[Q04] 修改列类型
来源：http://re.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gx.asd995.cn

[Q05] 重命名列
来源：http://ff.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ag.huanxung.cn

[Q06] 删除列
来源：http://dt.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zn.hahajie.cn

[Q07] 删除表
来源：http://lx.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://iy.haigaiapp.cn

[Q08] 创建普通索引
来源：http://dl.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://od.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://cw.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://em.bookmarksfly.cn

[Q10] 插入单行
来源：http://ro.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wt.huanxung.cn

[Q11] 一次插入多行
来源：http://wg.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cf.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://am.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://io.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pk.hnjuh.cn

[Q13] 忽略重复插入
来源：http://bw.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pm.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://es.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cd.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ae.newstarts.cn

[Q15] 查询全部
来源：http://bg.huixiangedu.cn

SELECT * FROM users;
来源：http://kc.bjjhwx.cn

[Q16] 查询指定列
来源：http://ez.szsharing.cn

SELECT id, name FROM users;
来源：http://hw.hahajie.cn

[Q17] 条件查询
来源：http://sp.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fb.huixiangedu.cn

[Q18] 模糊匹配
来源：http://hv.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://or.szxytkj.cn

[Q19] 范围查询
来源：http://yn.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rd.nicolike.cn

[Q20] IN 列表
来源：http://fx.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qy.shtwfgs.cn

[Q21] 空值判断
来源：http://nt.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yl.huixiangedu.cn

[Q22] 排序
来源：http://px.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://we.shxzskj.cn

[Q23] 分页
来源：http://gs.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ds.huixiangedu.cn

[Q24] 去重
来源：http://jd.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://nr.lnxyls.cn

[Q25] 只取前 N 条
来源：http://pk.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cm.wgjwhj.cn

[Q26] 计数
来源：http://hn.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://xo.shxzukj.cn

[Q27] 条件计数
来源：http://vp.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fr.muxihuayi.cn

[Q28] 求和与平均
来源：http://tl.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qy.panjiajie.cn

[Q29] 最大最小值
来源：http://ws.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xb.shxzskj.cn

[Q30] 分组统计
来源：http://uz.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ub.haigaiapp.cn

[Q31] 分组后过滤
来源：http://ip.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hh.szsharing.cn

[Q32] 分组拼接字符串
来源：http://yj.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fv.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fj.asd995.cn

[Q33] 多列分组
来源：http://tz.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qf.nszjky.cn

[Q34] 每组取第一条
来源：http://fn.panjiajie.cn

SELECT * FROM (
来源：http://hd.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dm.jctech888.com.cn

) t WHERE rn = 1;
来源：http://lj.jianghongdianzi.cn

[Q35] 内连接
来源：http://jy.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gd.shxzskj.cn

[Q36] 左连接
来源：http://mh.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ae.shxzukj.cn

[Q37] 右连接
来源：http://jl.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xe.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zr.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yw.asd995.cn

[Q39] 自连接（查上下级）
来源：http://rg.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fa.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oa.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rk.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gq.gzmigu.cn

[Q41] 多表连接
来源：http://xy.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yl.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://rc.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://cv.521024.cn

[Q42] 连接条件附加过滤
来源：http://lo.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://nm.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cf.9csxet.cn

[Q43] 标量子查询
来源：http://te.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bw.bjjhwx.cn

[Q44] IN 子查询
来源：http://aw.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ui.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://hg.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rl.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mp.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ps.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://kk.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cb.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://rn.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mf.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://se.colortex.cn

[Q49] 更新单行
来源：http://fh.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jq.szsharing.cn

[Q50] 批量更新
来源：http://ni.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vo.asd995.cn

[Q51] 用子查询更新
来源：http://rt.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eo.gzmigu.cn

[Q52] 删除指定行
来源：http://kq.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://xu.bookmarksfly.cn

[Q53] 按条件删除
来源：http://jg.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zd.haigaiapp.cn

[Q54] 清空表
来源：http://gv.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://ox.nszjky.cn

[Q55] 排名（并列占位）
来源：http://ph.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cg.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ce.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cw.huanxung.cn

[Q57] 行号
来源：http://mc.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gx.huixiangedu.cn

[Q58] 累计求和
来源：http://kw.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cd.yuexingan06.cn

[Q59] 分组内累计
来源：http://dz.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xf.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://bw.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kw.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fs.521024.cn

[Q61] 移动平均
来源：http://xj.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ye.jianghongdianzi.cn

[Q62] 分组占比
来源：http://wx.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gy.gzmigu.cn

[Q63] 开启事务
来源：http://gh.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oz.szxytkj.cn

[Q64] 提交事务
来源：http://vf.521024.cn

COMMIT;
来源：http://lz.colortex.cn

[Q65] 回滚事务
来源：http://gu.lnxyls.cn

ROLLBACK;
来源：http://lz.bookmarksfly.cn

[Q66] 行锁查询
来源：http://jq.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ye.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://td.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pm.yuexingan06.cn

[Q68] 保存点
来源：http://qf.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://vu.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://sm.hnjuh.cn

[Q69] 查看执行计划
来源：http://cr.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zv.shtwfgs.cn

[Q70] 更新统计信息
来源：http://ef.muxihuayi.cn

ANALYZE TABLE users;
来源：http://nd.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://mn.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://on.hahajie.cn

[Q72] 查看索引
来源：http://nf.shxzskj.cn

SHOW INDEX FROM users;
来源：http://mn.huixiangedu.cn

[Q73] 查看表状态
来源：http://mr.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://am.jctech888.com.cn

[Q74] 强制使用索引
来源：http://bg.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ra.muxihuayi.cn

[Q75] 日期格式化
来源：http://no.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://af.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://au.bookmarksfly.cn

[Q76] 按天统计
来源：http://ww.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://st.nicolike.cn

[Q77] 时间加减
来源：http://uh.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zr.wgjwhj.cn

[Q78] 当前时间
来源：http://ua.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pn.gzmigu.cn

[Q79] 字符串拼接
来源：http://qa.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rk.muxihuayi.cn

[Q80] 字符串截取
来源：http://yc.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uq.nicolike.cn

[Q81] 字符串替换
来源：http://kx.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qg.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://qq.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qj.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://gi.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nq.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://xy.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://iu.chemitech.net.cn

[Q85] 数值取整
来源：http://bo.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fu.haigaiapp.cn


<!-- 参考信息 -->