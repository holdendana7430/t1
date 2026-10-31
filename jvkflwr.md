代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rh.chemitech.net.cn

TS:   // 同 JS
来源：http://jh.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://mf.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kv.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pu.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://am.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://fa.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://wa.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ew.asd995.cn

JS:   async function f() { await g(); }
来源：http://hz.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yc.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dl.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qc.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sg.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://kr.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://qd.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://ki.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qg.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://uy.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://da.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cg.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gj.szsharing.cn

Ruby: threads.map(&:join)
来源：http://ri.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vd.panjiajie.cn

[O06] 使用进程池
来源：http://yf.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pl.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mm.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://el.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://kl.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ky.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tl.bjjhwx.cn

Ruby: // fork 块
来源：http://br.asd995.cn

C#:   Parallel.For
来源：http://go.jctech888.com.cn

================================================================================
来源：http://vk.huixinmuqiang.cn

P. 常用工具函数
来源：http://on.nicolike.cn

================================================================================
来源：http://dv.panjiajie.cn

[P01] 生成 UUID
来源：http://pr.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://ts.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bg.colortex.cn

JS:   crypto.randomUUID()
来源：http://zy.nicolike.cn

TS:   crypto.randomUUID()
来源：http://cw.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://vm.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://zv.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://cz.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://uz.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://de.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pc.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oq.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wj.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qv.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tf.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ky.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rx.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tq.hnjuh.cn

[P03] 生成短随机字符串
来源：http://mn.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wu.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fd.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qn.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yj.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://by.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cd.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wa.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gs.9csxet.cn

[P04] 求长度
来源：http://ug.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jk.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://je.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eo.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://al.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://rc.nszjky.cn

Go:   len(arr);  len(m)
来源：http://js.szxytkj.cn

Ruby: x.length;  x.size
来源：http://kl.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xy.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://vx.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yy.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qv.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uf.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zn.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://is.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://el.nicolike.cn

Ruby: a == b
来源：http://to.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yu.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ju.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://et.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://tl.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xc.gzmigu.cn

TS:   if (x == null) {}
来源：http://az.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cy.shxzukj.cn

Go:   if x == nil {}
来源：http://uk.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pf.wgjwhj.cn

C#:   if (x is null) {}
来源：http://ii.shtwfgs.cn

[P07] 防抖与节流
来源：http://vy.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ou.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://oe.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pz.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ua.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vd.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ca.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://re.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fd.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://li.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rp.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ia.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gt.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nf.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://je.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tn.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tb.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ek.newstarts.cn

================================================================================
来源：http://um.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uk.nszjky.cn

================================================================================
来源：http://rt.hahajie.cn

[Q01] 创建表
来源：http://or.jctech888.com.cn

CREATE TABLE users (
来源：http://ma.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kh.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://zw.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://fb.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fk.nszjky.cn

);
来源：http://yu.shxzukj.cn

[Q02] 创建带外键的表
来源：http://qr.newstarts.cn

CREATE TABLE orders (
来源：http://cg.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bv.wgjwhj.cn

user_id INT NOT NULL,
来源：http://gr.szsharing.cn

amount DECIMAL(10, 2),
来源：http://sa.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oe.szxytkj.cn

);
来源：http://si.yuntaijiaju.cn

[Q03] 增加列
来源：http://tb.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pv.shxzukj.cn

[Q04] 修改列类型
来源：http://wn.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zz.szxytkj.cn

[Q05] 重命名列
来源：http://yz.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://io.chemitech.net.cn

[Q06] 删除列
来源：http://cd.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wa.hnjuh.cn

[Q07] 删除表
来源：http://ja.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://nz.yuexingan06.cn

[Q08] 创建普通索引
来源：http://id.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ha.9csxet.cn

[Q09] 创建唯一索引
来源：http://ej.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kd.nicolike.cn

[Q10] 插入单行
来源：http://bx.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ko.shxzukj.cn

[Q11] 一次插入多行
来源：http://bp.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kd.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://ug.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oj.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qb.hahajie.cn

[Q13] 忽略重复插入
来源：http://hy.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ca.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://tg.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pa.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ag.huanxung.cn

[Q15] 查询全部
来源：http://xx.nszjky.cn

SELECT * FROM users;
来源：http://rd.szxytkj.cn

[Q16] 查询指定列
来源：http://uq.szsharing.cn

SELECT id, name FROM users;
来源：http://pf.szsharing.cn

[Q17] 条件查询
来源：http://yx.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://da.jctech888.com.cn

[Q18] 模糊匹配
来源：http://ki.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tq.bookmarksfly.cn

[Q19] 范围查询
来源：http://ij.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eu.colortex.cn

[Q20] IN 列表
来源：http://cl.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ku.szsharing.cn

[Q21] 空值判断
来源：http://dh.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gr.asd995.cn

[Q22] 排序
来源：http://cm.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gi.bookmarksfly.cn

[Q23] 分页
来源：http://zt.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ql.huanxung.cn

[Q24] 去重
来源：http://zm.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://uz.521024.cn

[Q25] 只取前 N 条
来源：http://xm.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://en.9csxet.cn

[Q26] 计数
来源：http://ao.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://ux.yuntaijiaju.cn

[Q27] 条件计数
来源：http://ey.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vb.nszjky.cn

[Q28] 求和与平均
来源：http://yr.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vq.9csxet.cn

[Q29] 最大最小值
来源：http://vx.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ff.haigaiapp.cn

[Q30] 分组统计
来源：http://ao.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rb.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://qs.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vo.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://mg.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mz.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ak.huixinmuqiang.cn

[Q33] 多列分组
来源：http://rb.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vg.9csxet.cn

[Q34] 每组取第一条
来源：http://hh.jianghongdianzi.cn

SELECT * FROM (
来源：http://yi.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qo.nicolike.cn

) t WHERE rn = 1;
来源：http://re.jctech888.com.cn

[Q35] 内连接
来源：http://tw.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qu.bjjhwx.cn

[Q36] 左连接
来源：http://rr.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ds.shxzukj.cn

[Q37] 右连接
来源：http://kc.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ah.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xq.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://af.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://um.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cw.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rs.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ln.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nx.szxytkj.cn

[Q41] 多表连接
来源：http://jp.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ef.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://um.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://rx.521024.cn

[Q42] 连接条件附加过滤
来源：http://cg.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://mv.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xf.huixiangedu.cn

[Q43] 标量子查询
来源：http://zp.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qa.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://yf.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gy.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://ji.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://du.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hx.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ji.shtwfgs.cn

[Q47] 与平均值比较
来源：http://ru.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lq.521024.cn

[Q48] CTE 公用表表达式
来源：http://zi.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ax.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://bx.szsharing.cn

[Q49] 更新单行
来源：http://fo.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wl.shxzskj.cn

[Q50] 批量更新
来源：http://mg.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qp.shxzukj.cn

[Q51] 用子查询更新
来源：http://rh.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tb.nicolike.cn

[Q52] 删除指定行
来源：http://lm.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://ya.shxzskj.cn

[Q53] 按条件删除
来源：http://jq.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://um.gzmigu.cn

[Q54] 清空表
来源：http://ws.hahajie.cn

TRUNCATE TABLE logs;
来源：http://sv.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://tm.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gq.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://bh.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hg.gzmigu.cn

[Q57] 行号
来源：http://vu.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ps.gzmigu.cn

[Q58] 累计求和
来源：http://ma.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bn.huixiangedu.cn

[Q59] 分组内累计
来源：http://th.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://re.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://yy.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zw.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pn.bookmarksfly.cn

[Q61] 移动平均
来源：http://sw.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bl.huixiangedu.cn

[Q62] 分组占比
来源：http://qs.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jr.shxzukj.cn

[Q63] 开启事务
来源：http://uv.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oh.szsharing.cn

[Q64] 提交事务
来源：http://ts.wgjwhj.cn

COMMIT;
来源：http://vs.9csxet.cn

[Q65] 回滚事务
来源：http://rn.hahajie.cn

ROLLBACK;
来源：http://kt.shtwfgs.cn

[Q66] 行锁查询
来源：http://mh.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nc.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://wo.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pd.szxytkj.cn

[Q68] 保存点
来源：http://oj.colortex.cn

SAVEPOINT sp1;
来源：http://lh.szxytkj.cn

ROLLBACK TO sp1;
来源：http://yr.hahajie.cn

[Q69] 查看执行计划
来源：http://df.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sa.asd995.cn

[Q70] 更新统计信息
来源：http://ja.bjjhwx.cn

ANALYZE TABLE users;
来源：http://pq.colortex.cn

[Q71] 查看建表语句
来源：http://bc.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ff.9csxet.cn

[Q72] 查看索引
来源：http://xb.lnxyls.cn

SHOW INDEX FROM users;
来源：http://bt.muxihuayi.cn

[Q73] 查看表状态
来源：http://nq.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kw.shxzukj.cn

[Q74] 强制使用索引
来源：http://vn.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lt.huanxung.cn

[Q75] 日期格式化
来源：http://lw.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://om.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rf.panjiajie.cn

[Q76] 按天统计
来源：http://tf.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tg.nszjky.cn

[Q77] 时间加减
来源：http://tb.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vf.9csxet.cn

[Q78] 当前时间
来源：http://gl.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://al.lnxyls.cn

[Q79] 字符串拼接
来源：http://dm.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hw.gzmigu.cn

[Q80] 字符串截取
来源：http://jw.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ap.jctech888.com.cn

[Q81] 字符串替换
来源：http://fw.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bf.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://sp.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ja.9csxet.cn

[Q83] 大小写转换
来源：http://ue.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hp.shxzukj.cn


<!-- 参考信息 -->