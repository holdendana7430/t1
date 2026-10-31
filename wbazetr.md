代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rp.hahajie.cn

[O03] 加锁保护共享数据
来源：http://zx.hahajie.cn

Py:   with lock: shared += 1
来源：http://pk.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ur.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dl.colortex.cn

TS:   // 同 JS
来源：http://iy.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://bc.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gz.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xj.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://ty.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://ba.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://ud.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ta.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://so.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cp.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ao.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pi.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yj.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://ir.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://tm.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://cl.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ye.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://tw.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://ds.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zy.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ny.nicolike.cn

Ruby: threads.map(&:join)
来源：http://ca.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ud.shtwfgs.cn

[O06] 使用进程池
来源：http://hu.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bx.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nf.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://ec.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://wi.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cu.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bw.shxzukj.cn

Ruby: // fork 块
来源：http://qc.huixinmuqiang.cn

C#:   Parallel.For
来源：http://pq.jianghongdianzi.cn

================================================================================
来源：http://rs.asd995.cn

P. 常用工具函数
来源：http://bv.hahajie.cn

================================================================================
来源：http://os.521024.cn

[P01] 生成 UUID
来源：http://um.colortex.cn

Py:   str(uuid.uuid4())
来源：http://fk.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jc.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://yg.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://il.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://nw.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://gr.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://qf.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://kf.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://cf.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lv.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lx.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zi.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tl.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kr.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wx.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ye.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ct.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://mu.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tb.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ze.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dr.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aq.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kx.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ff.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xc.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://be.szsharing.cn

[P04] 求长度
来源：http://um.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bg.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yn.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cn.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rr.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://nm.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://md.shxzukj.cn

Ruby: x.length;  x.size
来源：http://us.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gk.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://ym.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iq.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ll.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dk.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://my.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kh.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cp.huixinmuqiang.cn

Ruby: a == b
来源：http://sl.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://er.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://an.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://po.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://rm.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pf.shtwfgs.cn

TS:   if (x == null) {}
来源：http://tq.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yu.haigaiapp.cn

Go:   if x == nil {}
来源：http://ve.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cn.gzmigu.cn

C#:   if (x is null) {}
来源：http://my.yuexingan06.cn

[P07] 防抖与节流
来源：http://js.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://om.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://fv.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kz.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kw.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cd.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aa.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://st.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ja.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://vo.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ux.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gt.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tg.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qv.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zo.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hw.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rc.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jn.huanxung.cn

================================================================================
来源：http://tj.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bn.panjiajie.cn

================================================================================
来源：http://ot.jianghongdianzi.cn

[Q01] 创建表
来源：http://qa.huixinmuqiang.cn

CREATE TABLE users (
来源：http://gr.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yn.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://yl.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://qk.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ey.hahajie.cn

);
来源：http://ba.newstarts.cn

[Q02] 创建带外键的表
来源：http://fu.huixiangedu.cn

CREATE TABLE orders (
来源：http://fm.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aw.nszjky.cn

user_id INT NOT NULL,
来源：http://hl.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://qr.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qd.haigaiapp.cn

);
来源：http://ii.hahajie.cn

[Q03] 增加列
来源：http://xn.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ce.wgjwhj.cn

[Q04] 修改列类型
来源：http://da.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kg.hahajie.cn

[Q05] 重命名列
来源：http://yi.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ju.szxytkj.cn

[Q06] 删除列
来源：http://jk.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ig.haigaiapp.cn

[Q07] 删除表
来源：http://vv.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://lu.shxzskj.cn

[Q08] 创建普通索引
来源：http://dw.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nl.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://bs.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ih.asd995.cn

[Q10] 插入单行
来源：http://ha.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cj.szxytkj.cn

[Q11] 一次插入多行
来源：http://nu.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ub.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://ew.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uq.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fs.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://ku.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hl.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://qf.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ec.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://da.huixiangedu.cn

[Q15] 查询全部
来源：http://qo.hahajie.cn

SELECT * FROM users;
来源：http://zj.shxzukj.cn

[Q16] 查询指定列
来源：http://sn.shxzukj.cn

SELECT id, name FROM users;
来源：http://va.szsharing.cn

[Q17] 条件查询
来源：http://lb.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tr.shxzskj.cn

[Q18] 模糊匹配
来源：http://ge.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bd.hahajie.cn

[Q19] 范围查询
来源：http://pj.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://md.panjiajie.cn

[Q20] IN 列表
来源：http://zh.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yq.yuntaijiaju.cn

[Q21] 空值判断
来源：http://jh.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wm.shxzukj.cn

[Q22] 排序
来源：http://ag.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uq.hnjuh.cn

[Q23] 分页
来源：http://wr.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bj.bookmarksfly.cn

[Q24] 去重
来源：http://cx.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://bc.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://vm.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lx.huixiangedu.cn

[Q26] 计数
来源：http://hc.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://mq.jianghongdianzi.cn

[Q27] 条件计数
来源：http://gr.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ub.shxzskj.cn

[Q28] 求和与平均
来源：http://zc.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://na.panjiajie.cn

[Q29] 最大最小值
来源：http://zy.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hi.colortex.cn

[Q30] 分组统计
来源：http://mv.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ny.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://jz.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ge.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://cb.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dz.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iq.hnjuh.cn

[Q33] 多列分组
来源：http://hr.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ex.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://xz.nicolike.cn

SELECT * FROM (
来源：http://aj.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kx.nszjky.cn

) t WHERE rn = 1;
来源：http://oh.gzmigu.cn

[Q35] 内连接
来源：http://fi.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pr.nicolike.cn

[Q36] 左连接
来源：http://bd.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kf.shxzukj.cn

[Q37] 右连接
来源：http://dr.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pa.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yc.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ih.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://zj.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kk.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://na.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vf.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xw.bookmarksfly.cn

[Q41] 多表连接
来源：http://pp.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tv.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://nj.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://bk.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://kg.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://rz.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mr.shtwfgs.cn

[Q43] 标量子查询
来源：http://hd.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dj.colortex.cn

[Q44] IN 子查询
来源：http://rm.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vy.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ww.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zq.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dl.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qy.hahajie.cn

[Q47] 与平均值比较
来源：http://sh.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oy.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://wr.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hl.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://li.newstarts.cn

[Q49] 更新单行
来源：http://bx.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xu.huixinmuqiang.cn

[Q50] 批量更新
来源：http://hu.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mk.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://yi.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wn.muxihuayi.cn

[Q52] 删除指定行
来源：http://df.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://wf.yuexingan06.cn

[Q53] 按条件删除
来源：http://by.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yd.huanxung.cn

[Q54] 清空表
来源：http://fk.nicolike.cn

TRUNCATE TABLE logs;
来源：http://zc.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://xi.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dj.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://ug.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ov.huanxung.cn

[Q57] 行号
来源：http://go.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://du.szxytkj.cn

[Q58] 累计求和
来源：http://lp.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gf.newstarts.cn

[Q59] 分组内累计
来源：http://sq.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bn.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://nk.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ax.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ik.panjiajie.cn

[Q61] 移动平均
来源：http://wf.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kl.hnjuh.cn

[Q62] 分组占比
来源：http://og.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://in.nszjky.cn

[Q63] 开启事务
来源：http://pp.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mb.asd995.cn

[Q64] 提交事务
来源：http://db.shxzukj.cn

COMMIT;
来源：http://cq.nicolike.cn

[Q65] 回滚事务
来源：http://at.szsharing.cn

ROLLBACK;
来源：http://ut.panjiajie.cn

[Q66] 行锁查询
来源：http://th.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jf.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://sa.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fi.newstarts.cn

[Q68] 保存点
来源：http://qi.yuexingan06.cn

SAVEPOINT sp1;
来源：http://jr.521024.cn

ROLLBACK TO sp1;
来源：http://yn.szsharing.cn

[Q69] 查看执行计划
来源：http://dg.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://le.chemitech.net.cn

[Q70] 更新统计信息
来源：http://pt.9csxet.cn

ANALYZE TABLE users;
来源：http://pd.jctech888.com.cn

[Q71] 查看建表语句
来源：http://zv.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qj.asd995.cn

[Q72] 查看索引
来源：http://rx.hahajie.cn

SHOW INDEX FROM users;
来源：http://kp.szxytkj.cn

[Q73] 查看表状态
来源：http://mc.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ve.wgjwhj.cn

[Q74] 强制使用索引
来源：http://qq.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ct.bjjhwx.cn

[Q75] 日期格式化
来源：http://lu.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kq.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eu.bjjhwx.cn

[Q76] 按天统计
来源：http://tm.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://av.huixinmuqiang.cn

[Q77] 时间加减
来源：http://vo.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ed.bjjhwx.cn

[Q78] 当前时间
来源：http://yw.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://be.haigaiapp.cn

[Q79] 字符串拼接
来源：http://bm.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yx.panjiajie.cn

[Q80] 字符串截取
来源：http://pe.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tp.bookmarksfly.cn

[Q81] 字符串替换
来源：http://ta.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rn.szsharing.cn


<!-- 参考信息 -->