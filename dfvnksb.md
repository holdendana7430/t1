代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://fw.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://jm.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://uv.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://ck.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wq.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://nd.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ed.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fb.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gn.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gm.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://qt.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://jc.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://dm.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jk.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://et.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://gs.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cn.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nc.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://jb.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pi.muxihuayi.cn

[O06] 使用进程池
来源：http://ey.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vt.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mz.521024.cn

JS:   // child_process / cluster 模块
来源：http://xb.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://bw.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zs.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fn.colortex.cn

Ruby: // fork 块
来源：http://ye.hahajie.cn

C#:   Parallel.For
来源：http://vz.szxytkj.cn

================================================================================
来源：http://ia.bookmarksfly.cn

P. 常用工具函数
来源：http://he.9csxet.cn

================================================================================
来源：http://bm.yuexingan06.cn

[P01] 生成 UUID
来源：http://vr.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://ts.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lz.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ha.hahajie.cn

TS:   crypto.randomUUID()
来源：http://uv.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://hw.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://th.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://up.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://lv.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://km.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eb.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fj.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gu.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://si.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mo.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zt.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zp.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jm.panjiajie.cn

[P03] 生成短随机字符串
来源：http://ul.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tu.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aa.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jk.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fb.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lk.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tu.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ks.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zz.jianghongdianzi.cn

[P04] 求长度
来源：http://qm.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fn.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ek.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pc.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gu.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://yg.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://wt.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://cm.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ps.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://qe.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sl.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hu.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://by.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://co.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fp.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ja.bookmarksfly.cn

Ruby: a == b
来源：http://zp.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hw.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iv.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://db.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://pd.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mb.hahajie.cn

TS:   if (x == null) {}
来源：http://no.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fd.shtwfgs.cn

Go:   if x == nil {}
来源：http://bt.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rp.huixiangedu.cn

C#:   if (x is null) {}
来源：http://xu.colortex.cn

[P07] 防抖与节流
来源：http://id.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ia.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://te.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sk.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vz.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zn.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sb.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hu.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ku.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://eh.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pr.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://de.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nm.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gh.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://so.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ek.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dp.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vd.szxytkj.cn

================================================================================
来源：http://pu.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ow.panjiajie.cn

================================================================================
来源：http://dn.nszjky.cn

[Q01] 创建表
来源：http://wh.huixiangedu.cn

CREATE TABLE users (
来源：http://wz.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ee.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://xx.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://vd.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iq.newstarts.cn

);
来源：http://dw.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://qt.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://co.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ux.colortex.cn

user_id INT NOT NULL,
来源：http://wo.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://rx.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sq.521024.cn

);
来源：http://ll.huixinmuqiang.cn

[Q03] 增加列
来源：http://sk.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mc.521024.cn

[Q04] 修改列类型
来源：http://oa.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lh.jianghongdianzi.cn

[Q05] 重命名列
来源：http://qz.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tc.huixiangedu.cn

[Q06] 删除列
来源：http://zm.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sy.gzmigu.cn

[Q07] 删除表
来源：http://zd.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://iz.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://sf.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vd.hnjuh.cn

[Q09] 创建唯一索引
来源：http://qt.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yb.colortex.cn

[Q10] 插入单行
来源：http://gc.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ld.haigaiapp.cn

[Q11] 一次插入多行
来源：http://vv.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ll.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://jg.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jj.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cm.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://ae.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wo.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://yu.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rm.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gg.shxzukj.cn

[Q15] 查询全部
来源：http://ds.yuexingan06.cn

SELECT * FROM users;
来源：http://gy.wgjwhj.cn

[Q16] 查询指定列
来源：http://uk.chemitech.net.cn

SELECT id, name FROM users;
来源：http://qs.huixinmuqiang.cn

[Q17] 条件查询
来源：http://wu.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ej.jctech888.com.cn

[Q18] 模糊匹配
来源：http://od.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rd.bookmarksfly.cn

[Q19] 范围查询
来源：http://wj.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gl.shxzskj.cn

[Q20] IN 列表
来源：http://kl.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ju.asd995.cn

[Q21] 空值判断
来源：http://ob.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zs.shtwfgs.cn

[Q22] 排序
来源：http://al.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sq.huixinmuqiang.cn

[Q23] 分页
来源：http://xh.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zq.szxytkj.cn

[Q24] 去重
来源：http://ru.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://kt.lnxyls.cn

[Q25] 只取前 N 条
来源：http://ns.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mt.chemitech.net.cn

[Q26] 计数
来源：http://ok.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://pr.lnxyls.cn

[Q27] 条件计数
来源：http://mj.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://je.521024.cn

[Q28] 求和与平均
来源：http://qu.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eo.szsharing.cn

[Q29] 最大最小值
来源：http://xb.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://im.521024.cn

[Q30] 分组统计
来源：http://uk.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vp.asd995.cn

[Q31] 分组后过滤
来源：http://kq.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hn.nicolike.cn

[Q32] 分组拼接字符串
来源：http://jx.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fj.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vw.nicolike.cn

[Q33] 多列分组
来源：http://wh.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xj.hnjuh.cn

[Q34] 每组取第一条
来源：http://sj.huanxung.cn

SELECT * FROM (
来源：http://zi.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ui.chemitech.net.cn

) t WHERE rn = 1;
来源：http://rd.panjiajie.cn

[Q35] 内连接
来源：http://wg.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vj.gzmigu.cn

[Q36] 左连接
来源：http://gr.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fw.shtwfgs.cn

[Q37] 右连接
来源：http://lb.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://me.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xb.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vg.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://ar.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jn.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pt.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fg.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hu.nszjky.cn

[Q41] 多表连接
来源：http://mk.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lu.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://hu.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ko.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://jq.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://ql.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yo.muxihuayi.cn

[Q43] 标量子查询
来源：http://fw.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kv.colortex.cn

[Q44] IN 子查询
来源：http://al.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wb.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://cc.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ss.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://el.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jv.521024.cn

[Q47] 与平均值比较
来源：http://fw.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hq.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://av.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rp.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://mu.chemitech.net.cn

[Q49] 更新单行
来源：http://fv.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tb.colortex.cn

[Q50] 批量更新
来源：http://cb.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ca.shtwfgs.cn

[Q51] 用子查询更新
来源：http://tm.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lk.szsharing.cn

[Q52] 删除指定行
来源：http://pf.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://rj.huixiangedu.cn

[Q53] 按条件删除
来源：http://iv.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yu.nszjky.cn

[Q54] 清空表
来源：http://ma.9csxet.cn

TRUNCATE TABLE logs;
来源：http://ji.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://rb.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yt.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://mk.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://he.jianghongdianzi.cn

[Q57] 行号
来源：http://nw.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cj.yuexingan06.cn

[Q58] 累计求和
来源：http://sb.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ic.chemitech.net.cn

[Q59] 分组内累计
来源：http://ux.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rc.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://yp.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://do.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hv.bookmarksfly.cn

[Q61] 移动平均
来源：http://jy.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rm.haigaiapp.cn

[Q62] 分组占比
来源：http://ko.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://av.bjjhwx.cn

[Q63] 开启事务
来源：http://ry.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oc.jianghongdianzi.cn

[Q64] 提交事务
来源：http://iy.jctech888.com.cn

COMMIT;
来源：http://gu.muxihuayi.cn

[Q65] 回滚事务
来源：http://da.521024.cn

ROLLBACK;
来源：http://fz.yuexingan06.cn

[Q66] 行锁查询
来源：http://wj.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uh.gzmigu.cn

[Q67] 设置隔离级别
来源：http://ep.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wj.gzmigu.cn

[Q68] 保存点
来源：http://qi.colortex.cn

SAVEPOINT sp1;
来源：http://vu.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://wc.nszjky.cn

[Q69] 查看执行计划
来源：http://pd.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bj.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://nm.9csxet.cn

ANALYZE TABLE users;
来源：http://rz.lnxyls.cn

[Q71] 查看建表语句
来源：http://wd.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ie.szsharing.cn

[Q72] 查看索引
来源：http://pj.newstarts.cn

SHOW INDEX FROM users;
来源：http://kp.muxihuayi.cn

[Q73] 查看表状态
来源：http://hb.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jy.colortex.cn

[Q74] 强制使用索引
来源：http://po.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hd.hnjuh.cn

[Q75] 日期格式化
来源：http://rn.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://su.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sv.huanxung.cn

[Q76] 按天统计
来源：http://yk.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cc.hnjuh.cn

[Q77] 时间加减
来源：http://wo.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xf.huixiangedu.cn

[Q78] 当前时间
来源：http://vs.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gk.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://as.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://az.chemitech.net.cn

[Q80] 字符串截取
来源：http://sm.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oy.haigaiapp.cn

[Q81] 字符串替换
来源：http://hf.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yn.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://un.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hn.shxzskj.cn

[Q83] 大小写转换
来源：http://nn.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://np.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://fa.521024.cn

SELECT TRIM(name) FROM users;
来源：http://qr.jianghongdianzi.cn

[Q85] 数值取整
来源：http://kg.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wv.shtwfgs.cn


<!-- 参考信息 -->