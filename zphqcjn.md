代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ln.szsharing.cn

[N11] 二叉树中序遍历
来源：http://pd.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vi.huanxung.cn

PHP:  // 手写递归函数
来源：http://vy.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sn.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ro.szxytkj.cn

Java: // 手写递归
来源：http://if.muxihuayi.cn

Go:   // 手写递归
来源：http://lf.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qa.shtwfgs.cn

C#:   // 手写递归
来源：http://za.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gs.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://th.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rr.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pz.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pr.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ug.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gh.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nw.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bw.gzmigu.cn

================================================================================
来源：http://wi.wgjwhj.cn

O. 并发与异步
来源：http://xw.haigaiapp.cn

================================================================================
来源：http://aq.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://xg.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sg.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pu.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ub.haigaiapp.cn

TS:   // 同 JS
来源：http://kw.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://yv.jianghongdianzi.cn

Go:   go f()
来源：http://eh.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ou.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://ng.asd995.cn

[O02] 使用线程池
来源：http://si.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ar.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mp.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://kx.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://tl.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ft.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ar.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vx.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xs.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://lz.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://pc.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://kq.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ij.nszjky.cn

TS:   // 同 JS
来源：http://kj.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://dz.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rp.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ti.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://ef.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://jl.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://ck.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zt.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://lv.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jy.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://di.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ua.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ed.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://kv.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://pa.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://cv.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ew.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://ax.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://cd.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ul.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yb.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://gs.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://an.szsharing.cn

[O06] 使用进程池
来源：http://sy.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wu.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yz.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://me.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://dd.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iv.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ok.nicolike.cn

Ruby: // fork 块
来源：http://jh.newstarts.cn

C#:   Parallel.For
来源：http://dn.nszjky.cn

================================================================================
来源：http://od.nszjky.cn

P. 常用工具函数
来源：http://gb.yuntaijiaju.cn

================================================================================
来源：http://iw.chemitech.net.cn

[P01] 生成 UUID
来源：http://cc.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://zx.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dt.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://cw.colortex.cn

TS:   crypto.randomUUID()
来源：http://qh.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://mk.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://dv.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://kz.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://dj.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://bc.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ve.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xs.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aa.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://br.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://re.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vo.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://do.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ab.newstarts.cn

[P03] 生成短随机字符串
来源：http://yj.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://du.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mv.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wh.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bp.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://it.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bh.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dz.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qf.colortex.cn

[P04] 求长度
来源：http://gn.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cx.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ip.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pp.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ae.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ze.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://fg.hnjuh.cn

Ruby: x.length;  x.size
来源：http://ml.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ai.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://xl.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ig.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nn.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hu.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kc.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://th.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gm.chemitech.net.cn

Ruby: a == b
来源：http://qe.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ue.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ud.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pt.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://ht.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://td.szsharing.cn

TS:   if (x == null) {}
来源：http://vb.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://og.521024.cn

Go:   if x == nil {}
来源：http://ms.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ig.lnxyls.cn

C#:   if (x is null) {}
来源：http://gf.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://zn.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wd.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://nh.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://up.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fn.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xq.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dv.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bh.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zc.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://kw.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bg.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wf.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ig.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qy.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kj.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fs.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fd.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bf.jianghongdianzi.cn

================================================================================
来源：http://xu.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wl.panjiajie.cn

================================================================================
来源：http://cw.huixiangedu.cn

[Q01] 创建表
来源：http://bc.huixiangedu.cn

CREATE TABLE users (
来源：http://se.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gs.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://nm.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://jz.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lj.gzmigu.cn

);
来源：http://di.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://ae.wgjwhj.cn

CREATE TABLE orders (
来源：http://om.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uk.muxihuayi.cn

user_id INT NOT NULL,
来源：http://xx.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://ob.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pp.lnxyls.cn

);
来源：http://ii.521024.cn

[Q03] 增加列
来源：http://fo.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fg.colortex.cn

[Q04] 修改列类型
来源：http://tv.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nm.asd995.cn

[Q05] 重命名列
来源：http://us.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qt.yuexingan06.cn

[Q06] 删除列
来源：http://ac.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cz.jctech888.com.cn

[Q07] 删除表
来源：http://kr.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://cv.yuexingan06.cn

[Q08] 创建普通索引
来源：http://kr.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tm.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://zu.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://re.9csxet.cn

[Q10] 插入单行
来源：http://rd.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://io.nszjky.cn

[Q11] 一次插入多行
来源：http://ae.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ta.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://re.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rc.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pj.nicolike.cn

[Q13] 忽略重复插入
来源：http://ti.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ri.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://vg.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bv.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ws.szxytkj.cn

[Q15] 查询全部
来源：http://wk.bookmarksfly.cn

SELECT * FROM users;
来源：http://sy.szxytkj.cn

[Q16] 查询指定列
来源：http://fa.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://zz.huixinmuqiang.cn

[Q17] 条件查询
来源：http://vp.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tj.bjjhwx.cn

[Q18] 模糊匹配
来源：http://cj.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ge.huixinmuqiang.cn

[Q19] 范围查询
来源：http://cn.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ua.asd995.cn

[Q20] IN 列表
来源：http://ym.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yj.chemitech.net.cn

[Q21] 空值判断
来源：http://ex.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pb.haigaiapp.cn

[Q22] 排序
来源：http://sy.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ds.shtwfgs.cn

[Q23] 分页
来源：http://ep.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yu.colortex.cn

[Q24] 去重
来源：http://xw.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://fn.colortex.cn

[Q25] 只取前 N 条
来源：http://dq.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zr.shtwfgs.cn

[Q26] 计数
来源：http://kl.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://tj.newstarts.cn

[Q27] 条件计数
来源：http://th.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aq.colortex.cn

[Q28] 求和与平均
来源：http://xv.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kk.jctech888.com.cn

[Q29] 最大最小值
来源：http://zy.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wp.nszjky.cn

[Q30] 分组统计
来源：http://ls.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bj.shxzukj.cn

[Q31] 分组后过滤
来源：http://rn.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ip.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://un.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rh.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nc.szsharing.cn

[Q33] 多列分组
来源：http://vi.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oj.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://sv.colortex.cn

SELECT * FROM (
来源：http://xq.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lq.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://mw.chemitech.net.cn

[Q35] 内连接
来源：http://rl.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wx.lnxyls.cn

[Q36] 左连接
来源：http://gx.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ue.newstarts.cn

[Q37] 右连接
来源：http://cf.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mu.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ru.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gc.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://zx.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gt.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tl.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://os.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ku.chemitech.net.cn

[Q41] 多表连接
来源：http://ev.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sb.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://gc.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://kt.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://vz.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ee.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jv.hahajie.cn

[Q43] 标量子查询
来源：http://ko.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rp.haigaiapp.cn

[Q44] IN 子查询
来源：http://kc.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bx.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://el.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ge.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ij.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ex.jctech888.com.cn

[Q47] 与平均值比较
来源：http://qi.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qf.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://dx.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xd.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://km.szxytkj.cn

[Q49] 更新单行
来源：http://hk.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jh.szsharing.cn

[Q50] 批量更新
来源：http://em.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dz.asd995.cn

[Q51] 用子查询更新
来源：http://pg.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dm.hnjuh.cn

[Q52] 删除指定行
来源：http://mw.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://pe.nszjky.cn

[Q53] 按条件删除
来源：http://lx.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ys.jctech888.com.cn

[Q54] 清空表
来源：http://ae.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://zf.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://fm.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vy.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://mi.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tb.huanxung.cn

[Q57] 行号
来源：http://we.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://if.hnjuh.cn

[Q58] 累计求和
来源：http://io.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fo.gzmigu.cn

[Q59] 分组内累计
来源：http://jz.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dq.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://bl.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ba.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nz.hahajie.cn

[Q61] 移动平均
来源：http://ks.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wx.nicolike.cn

[Q62] 分组占比
来源：http://ea.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pu.bookmarksfly.cn


<!-- 参考信息 -->