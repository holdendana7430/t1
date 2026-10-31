代发 wailian999

PHP:  // 手写递归函数
来源：http://ke.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cf.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wj.colortex.cn

Java: // 手写递归
来源：http://yu.hahajie.cn

Go:   // 手写递归
来源：http://ek.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ue.shtwfgs.cn

C#:   // 手写递归
来源：http://mn.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sc.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pk.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yt.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oa.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lt.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uw.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kb.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tf.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://na.nicolike.cn

================================================================================
来源：http://vx.bookmarksfly.cn

O. 并发与异步
来源：http://cc.bjjhwx.cn

================================================================================
来源：http://vn.szsharing.cn

[O01] 启动一个线程
来源：http://yh.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mz.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sm.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yi.haigaiapp.cn

TS:   // 同 JS
来源：http://dl.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://am.jianghongdianzi.cn

Go:   go f()
来源：http://kz.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://bg.colortex.cn

C#:   Task.Run(() => F());
来源：http://iv.shtwfgs.cn

[O02] 使用线程池
来源：http://op.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wf.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dc.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://hl.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://za.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://di.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rr.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wx.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://az.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://cc.szxytkj.cn

Py:   with lock: shared += 1
来源：http://nb.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://ln.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zu.hahajie.cn

TS:   // 同 JS
来源：http://fh.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://ed.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://as.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xj.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://hv.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://vi.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://fh.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bf.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://dr.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sp.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://un.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ux.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gj.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://ea.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://sm.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ef.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qr.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://gw.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://ka.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ls.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ea.nicolike.cn

Ruby: threads.map(&:join)
来源：http://eo.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pm.shxzskj.cn

[O06] 使用进程池
来源：http://vo.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kb.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fy.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://yc.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://xj.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ad.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wr.szxytkj.cn

Ruby: // fork 块
来源：http://vc.szsharing.cn

C#:   Parallel.For
来源：http://rx.yuntaijiaju.cn

================================================================================
来源：http://dl.bookmarksfly.cn

P. 常用工具函数
来源：http://ia.colortex.cn

================================================================================
来源：http://ci.9csxet.cn

[P01] 生成 UUID
来源：http://ms.colortex.cn

Py:   str(uuid.uuid4())
来源：http://sc.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aw.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ud.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://ul.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://cu.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://an.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://ej.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://mk.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://tt.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ad.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://md.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gh.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bb.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yn.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dx.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yr.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ub.szxytkj.cn

[P03] 生成短随机字符串
来源：http://ot.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cb.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ah.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ap.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gm.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ok.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ro.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vh.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hq.shxzukj.cn

[P04] 求长度
来源：http://cz.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kw.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nu.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jr.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mn.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://sn.newstarts.cn

Go:   len(arr);  len(m)
来源：http://af.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://jn.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jc.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://lz.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hk.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sl.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://if.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vs.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tn.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uf.521024.cn

Ruby: a == b
来源：http://qi.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uv.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ax.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kv.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://aq.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fn.bjjhwx.cn

TS:   if (x == null) {}
来源：http://xv.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pj.wgjwhj.cn

Go:   if x == nil {}
来源：http://wk.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lh.colortex.cn

C#:   if (x is null) {}
来源：http://pp.lnxyls.cn

[P07] 防抖与节流
来源：http://sp.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xe.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://rn.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ci.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oe.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pw.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jv.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://en.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dk.9csxet.cn

[P08] 处理浮点精度问题
来源：http://px.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mj.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nv.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://it.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://el.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kf.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gu.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ko.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xf.yuexingan06.cn

================================================================================
来源：http://pe.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uo.9csxet.cn

================================================================================
来源：http://bg.hahajie.cn

[Q01] 创建表
来源：http://nx.lnxyls.cn

CREATE TABLE users (
来源：http://ah.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kj.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://hw.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://wq.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wn.yuexingan06.cn

);
来源：http://ar.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://nn.hnjuh.cn

CREATE TABLE orders (
来源：http://pw.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://st.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://bp.asd995.cn

amount DECIMAL(10, 2),
来源：http://kr.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vf.lnxyls.cn

);
来源：http://et.lnxyls.cn

[Q03] 增加列
来源：http://xi.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lj.colortex.cn

[Q04] 修改列类型
来源：http://mn.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eh.huanxung.cn

[Q05] 重命名列
来源：http://ad.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aq.huanxung.cn

[Q06] 删除列
来源：http://it.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tg.jianghongdianzi.cn

[Q07] 删除表
来源：http://ha.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://fv.hahajie.cn

[Q08] 创建普通索引
来源：http://la.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ry.nszjky.cn

[Q09] 创建唯一索引
来源：http://hq.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://je.shxzskj.cn

[Q10] 插入单行
来源：http://dk.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ky.newstarts.cn

[Q11] 一次插入多行
来源：http://hq.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pr.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://ex.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qk.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wu.asd995.cn

[Q13] 忽略重复插入
来源：http://eo.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vw.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://ip.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lf.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gg.jianghongdianzi.cn

[Q15] 查询全部
来源：http://do.newstarts.cn

SELECT * FROM users;
来源：http://hp.chemitech.net.cn

[Q16] 查询指定列
来源：http://fe.szxytkj.cn

SELECT id, name FROM users;
来源：http://tr.shtwfgs.cn

[Q17] 条件查询
来源：http://ll.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tv.yuexingan06.cn

[Q18] 模糊匹配
来源：http://id.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xw.huanxung.cn

[Q19] 范围查询
来源：http://hx.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gr.jianghongdianzi.cn

[Q20] IN 列表
来源：http://xa.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://af.szxytkj.cn

[Q21] 空值判断
来源：http://ov.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vq.jianghongdianzi.cn

[Q22] 排序
来源：http://dk.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yo.huixiangedu.cn

[Q23] 分页
来源：http://pp.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ca.shtwfgs.cn

[Q24] 去重
来源：http://kf.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://vl.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://xg.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gk.shxzukj.cn

[Q26] 计数
来源：http://rv.521024.cn

SELECT COUNT(*) FROM users;
来源：http://xr.nicolike.cn

[Q27] 条件计数
来源：http://br.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xk.haigaiapp.cn

[Q28] 求和与平均
来源：http://bs.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wy.panjiajie.cn

[Q29] 最大最小值
来源：http://dg.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dw.wgjwhj.cn

[Q30] 分组统计
来源：http://co.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://re.szsharing.cn

[Q31] 分组后过滤
来源：http://rl.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ae.huanxung.cn

[Q32] 分组拼接字符串
来源：http://ry.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xk.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lj.521024.cn

[Q33] 多列分组
来源：http://sg.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kn.wgjwhj.cn

[Q34] 每组取第一条
来源：http://wo.bookmarksfly.cn

SELECT * FROM (
来源：http://in.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://un.huanxung.cn

) t WHERE rn = 1;
来源：http://fa.szsharing.cn

[Q35] 内连接
来源：http://so.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qq.wgjwhj.cn

[Q36] 左连接
来源：http://cc.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://na.szsharing.cn

[Q37] 右连接
来源：http://sq.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ng.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ww.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ap.521024.cn

[Q39] 自连接（查上下级）
来源：http://xf.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://go.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oy.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kw.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tw.huixiangedu.cn

[Q41] 多表连接
来源：http://ee.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nb.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://uw.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://fw.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://ks.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://dd.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nb.huanxung.cn

[Q43] 标量子查询
来源：http://ur.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://en.chemitech.net.cn

[Q44] IN 子查询
来源：http://zd.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hn.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://gl.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rl.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vd.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gz.wgjwhj.cn

[Q47] 与平均值比较
来源：http://bu.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pv.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://qa.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lq.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://bm.shxzukj.cn

[Q49] 更新单行
来源：http://ke.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cv.hahajie.cn

[Q50] 批量更新
来源：http://zq.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qa.wgjwhj.cn

[Q51] 用子查询更新
来源：http://if.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gj.shxzukj.cn

[Q52] 删除指定行
来源：http://vd.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://ak.nszjky.cn

[Q53] 按条件删除
来源：http://jw.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ji.gzmigu.cn

[Q54] 清空表
来源：http://yk.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://pm.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://uy.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ih.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://lm.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hi.hahajie.cn

[Q57] 行号
来源：http://gq.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://af.bjjhwx.cn

[Q58] 累计求和
来源：http://hw.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yd.chemitech.net.cn

[Q59] 分组内累计
来源：http://mj.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yw.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://go.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xu.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ob.szxytkj.cn

[Q61] 移动平均
来源：http://kk.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fh.gzmigu.cn

[Q62] 分组占比
来源：http://gj.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yj.9csxet.cn

[Q63] 开启事务
来源：http://cx.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://op.chemitech.net.cn

[Q64] 提交事务
来源：http://dh.bookmarksfly.cn

COMMIT;
来源：http://ao.9csxet.cn


<!-- 参考信息 -->