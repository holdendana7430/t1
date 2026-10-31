代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hl.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hv.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dv.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zg.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tm.bookmarksfly.cn

[N10] 链表节点定义
来源：http://uc.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://to.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kr.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yr.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ad.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://wq.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fs.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fr.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rt.colortex.cn

[N11] 二叉树中序遍历
来源：http://ht.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mv.521024.cn

PHP:  // 手写递归函数
来源：http://sz.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ic.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kf.yuntaijiaju.cn

Java: // 手写递归
来源：http://dx.huanxung.cn

Go:   // 手写递归
来源：http://bz.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ed.shxzukj.cn

C#:   // 手写递归
来源：http://fs.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gw.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jv.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zb.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nz.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://if.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ai.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ai.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pm.szsharing.cn

================================================================================
来源：http://kj.nicolike.cn

O. 并发与异步
来源：http://ct.colortex.cn

================================================================================
来源：http://hr.hahajie.cn

[O01] 启动一个线程
来源：http://gv.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dr.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nd.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://im.yuntaijiaju.cn

TS:   // 同 JS
来源：http://iy.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ww.gzmigu.cn

Go:   go f()
来源：http://mz.521024.cn

Ruby: Thread.new { f }
来源：http://ud.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://ux.asd995.cn

[O02] 使用线程池
来源：http://hr.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rx.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://li.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://le.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://rp.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://le.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://za.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://op.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wz.9csxet.cn

[O03] 加锁保护共享数据
来源：http://us.colortex.cn

Py:   with lock: shared += 1
来源：http://ng.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://aj.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dy.huixiangedu.cn

TS:   // 同 JS
来源：http://ag.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://ou.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cc.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sg.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://ol.huanxung.cn

[O04] 定义异步函数并等待
来源：http://ya.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://rf.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bj.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://xc.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xq.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ab.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ts.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vb.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://cp.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://vo.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://mw.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://le.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://em.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://ty.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bi.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ie.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://zj.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ic.huixiangedu.cn

[O06] 使用进程池
来源：http://ai.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nj.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://aq.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://fa.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://xj.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ry.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://au.huixiangedu.cn

Ruby: // fork 块
来源：http://hp.bookmarksfly.cn

C#:   Parallel.For
来源：http://po.newstarts.cn

================================================================================
来源：http://ho.lnxyls.cn

P. 常用工具函数
来源：http://ua.shxzukj.cn

================================================================================
来源：http://pt.muxihuayi.cn

[P01] 生成 UUID
来源：http://ol.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://dm.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zc.nicolike.cn

JS:   crypto.randomUUID()
来源：http://im.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://iw.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://ec.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://ah.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://mz.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://bv.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://kc.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ty.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ia.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bs.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fe.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://br.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gm.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jx.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nh.shxzskj.cn

[P03] 生成短随机字符串
来源：http://xi.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kh.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ey.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eh.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mc.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mt.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://om.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mn.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nd.hnjuh.cn

[P04] 求长度
来源：http://eh.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uk.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tl.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ia.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ka.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://cb.nszjky.cn

Go:   len(arr);  len(m)
来源：http://qf.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://ze.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://id.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://ab.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tw.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nr.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nt.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kq.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xe.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ei.shxzskj.cn

Ruby: a == b
来源：http://ka.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dp.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ma.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ow.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://sx.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pv.muxihuayi.cn

TS:   if (x == null) {}
来源：http://lq.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ov.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://fu.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://as.gzmigu.cn

C#:   if (x is null) {}
来源：http://ps.521024.cn

[P07] 防抖与节流
来源：http://go.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nl.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://wn.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dn.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gs.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sy.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lm.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ra.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sb.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ex.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://de.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ep.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sr.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rr.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pc.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ug.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wo.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bw.shxzskj.cn

================================================================================
来源：http://yf.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://er.chemitech.net.cn

================================================================================
来源：http://fo.huixinmuqiang.cn

[Q01] 创建表
来源：http://ca.bookmarksfly.cn

CREATE TABLE users (
来源：http://qy.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ue.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://cj.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://dr.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ft.szxytkj.cn

);
来源：http://pe.9csxet.cn

[Q02] 创建带外键的表
来源：http://wb.nszjky.cn

CREATE TABLE orders (
来源：http://xt.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nq.nicolike.cn

user_id INT NOT NULL,
来源：http://dh.szsharing.cn

amount DECIMAL(10, 2),
来源：http://vk.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://te.shxzskj.cn

);
来源：http://ea.panjiajie.cn

[Q03] 增加列
来源：http://ek.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pi.huanxung.cn

[Q04] 修改列类型
来源：http://ed.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rz.jianghongdianzi.cn

[Q05] 重命名列
来源：http://ol.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rq.jianghongdianzi.cn

[Q06] 删除列
来源：http://rb.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mm.521024.cn

[Q07] 删除表
来源：http://cg.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://nw.szsharing.cn

[Q08] 创建普通索引
来源：http://jh.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ac.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://hb.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tg.chemitech.net.cn

[Q10] 插入单行
来源：http://lt.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zl.szxytkj.cn

[Q11] 一次插入多行
来源：http://tm.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ot.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://nq.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rh.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ih.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://ta.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bl.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://jz.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ts.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ro.szxytkj.cn

[Q15] 查询全部
来源：http://en.muxihuayi.cn

SELECT * FROM users;
来源：http://oe.9csxet.cn

[Q16] 查询指定列
来源：http://yn.wgjwhj.cn

SELECT id, name FROM users;
来源：http://eh.chemitech.net.cn

[Q17] 条件查询
来源：http://aq.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hp.shxzskj.cn

[Q18] 模糊匹配
来源：http://zz.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uo.asd995.cn

[Q19] 范围查询
来源：http://dq.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://er.yuntaijiaju.cn

[Q20] IN 列表
来源：http://gu.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sw.lnxyls.cn

[Q21] 空值判断
来源：http://ez.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wn.lnxyls.cn

[Q22] 排序
来源：http://ii.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aa.jianghongdianzi.cn

[Q23] 分页
来源：http://vg.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vd.shtwfgs.cn

[Q24] 去重
来源：http://ek.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://tl.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://di.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ul.chemitech.net.cn

[Q26] 计数
来源：http://sj.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://bf.jctech888.com.cn

[Q27] 条件计数
来源：http://nd.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zd.bjjhwx.cn

[Q28] 求和与平均
来源：http://cw.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vc.bjjhwx.cn

[Q29] 最大最小值
来源：http://gl.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ta.bookmarksfly.cn

[Q30] 分组统计
来源：http://vk.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vt.nszjky.cn

[Q31] 分组后过滤
来源：http://jm.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yu.huanxung.cn

[Q32] 分组拼接字符串
来源：http://ab.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cq.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rp.panjiajie.cn

[Q33] 多列分组
来源：http://dc.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qe.shxzskj.cn

[Q34] 每组取第一条
来源：http://tm.huanxung.cn

SELECT * FROM (
来源：http://ob.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ba.521024.cn

) t WHERE rn = 1;
来源：http://au.gzmigu.cn

[Q35] 内连接
来源：http://us.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tk.asd995.cn

[Q36] 左连接
来源：http://gf.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zg.muxihuayi.cn

[Q37] 右连接
来源：http://dn.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jc.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xd.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qs.colortex.cn

[Q39] 自连接（查上下级）
来源：http://qk.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cn.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mg.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zw.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://en.yuntaijiaju.cn

[Q41] 多表连接
来源：http://ko.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nf.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://qv.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://hb.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://tq.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://qi.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dk.szxytkj.cn

[Q43] 标量子查询
来源：http://gw.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bw.haigaiapp.cn

[Q44] IN 子查询
来源：http://ym.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hs.521024.cn

[Q45] EXISTS 判断存在
来源：http://rp.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kx.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dz.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lz.asd995.cn

[Q47] 与平均值比较
来源：http://qn.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pb.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://zr.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qz.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://rq.shxzukj.cn

[Q49] 更新单行
来源：http://mq.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xx.shxzskj.cn

[Q50] 批量更新
来源：http://sy.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xe.gzmigu.cn

[Q51] 用子查询更新
来源：http://rt.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uf.nszjky.cn

[Q52] 删除指定行
来源：http://sr.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://kf.muxihuayi.cn

[Q53] 按条件删除
来源：http://ym.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://at.shxzskj.cn

[Q54] 清空表
来源：http://mj.9csxet.cn

TRUNCATE TABLE logs;
来源：http://wd.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://jz.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qa.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://uk.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cv.szxytkj.cn

[Q57] 行号
来源：http://zt.chemitech.net.cn


<!-- 参考信息 -->