代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xw.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fo.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ki.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gh.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ll.colortex.cn

[N10] 链表节点定义
来源：http://ic.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jv.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aa.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lo.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lf.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://yz.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sz.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ej.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://le.colortex.cn

[N11] 二叉树中序遍历
来源：http://uz.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xa.9csxet.cn

PHP:  // 手写递归函数
来源：http://xf.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://il.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eu.hahajie.cn

Java: // 手写递归
来源：http://cr.asd995.cn

Go:   // 手写递归
来源：http://wi.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vq.shtwfgs.cn

C#:   // 手写递归
来源：http://bc.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uo.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bf.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gm.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zu.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ih.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lv.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ia.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qo.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mc.hnjuh.cn

================================================================================
来源：http://vk.chemitech.net.cn

O. 并发与异步
来源：http://vt.shxzukj.cn

================================================================================
来源：http://kx.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://jk.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mk.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://to.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qw.nszjky.cn

TS:   // 同 JS
来源：http://cj.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://ms.lnxyls.cn

Go:   go f()
来源：http://zo.nicolike.cn

Ruby: Thread.new { f }
来源：http://qr.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://cz.521024.cn

[O02] 使用线程池
来源：http://iw.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mu.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ep.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://fe.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://sv.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hf.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ty.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tv.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pk.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://zo.521024.cn

Py:   with lock: shared += 1
来源：http://vc.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://gs.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tg.yuexingan06.cn

TS:   // 同 JS
来源：http://ur.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://vh.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ou.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gq.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://sn.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://yx.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://mt.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ts.asd995.cn

JS:   async function f() { await g(); }
来源：http://rf.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yf.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cy.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qr.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tw.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://wx.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://gs.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://qy.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yj.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://iz.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://py.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qk.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pu.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://jq.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oe.yuntaijiaju.cn

[O06] 使用进程池
来源：http://bk.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mk.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ay.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://us.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://bx.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pq.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rm.shxzskj.cn

Ruby: // fork 块
来源：http://cb.shxzskj.cn

C#:   Parallel.For
来源：http://dg.gzmigu.cn

================================================================================
来源：http://sv.521024.cn

P. 常用工具函数
来源：http://zh.muxihuayi.cn

================================================================================
来源：http://jx.chemitech.net.cn

[P01] 生成 UUID
来源：http://kg.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://wj.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xf.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://zj.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://rz.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://bq.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://wc.asd995.cn

Ruby: SecureRandom.uuid
来源：http://ko.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://yq.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://ta.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bv.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jp.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ex.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fb.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tu.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://de.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ae.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://em.panjiajie.cn

[P03] 生成短随机字符串
来源：http://sb.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://go.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sa.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ys.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lf.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oe.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pt.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://et.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hl.huanxung.cn

[P04] 求长度
来源：http://sk.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ph.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bj.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://je.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zg.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://ef.nszjky.cn

Go:   len(arr);  len(m)
来源：http://wu.521024.cn

Ruby: x.length;  x.size
来源：http://pz.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://up.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://tw.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hf.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cn.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ad.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hb.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tp.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://md.wgjwhj.cn

Ruby: a == b
来源：http://zr.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wx.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zr.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gc.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://vt.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://it.szsharing.cn

TS:   if (x == null) {}
来源：http://bd.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wt.nicolike.cn

Go:   if x == nil {}
来源：http://ok.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fk.lnxyls.cn

C#:   if (x is null) {}
来源：http://qi.bjjhwx.cn

[P07] 防抖与节流
来源：http://jm.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dw.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://gn.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wr.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rt.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ok.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nv.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zl.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yo.nszjky.cn

[P08] 处理浮点精度问题
来源：http://fl.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://on.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mx.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fu.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://in.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fw.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://av.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://da.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://al.hnjuh.cn

================================================================================
来源：http://wu.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oq.521024.cn

================================================================================
来源：http://xv.wgjwhj.cn

[Q01] 创建表
来源：http://ju.haigaiapp.cn

CREATE TABLE users (
来源：http://ai.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tg.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://to.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://pj.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://is.chemitech.net.cn

);
来源：http://vg.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://nx.huanxung.cn

CREATE TABLE orders (
来源：http://rr.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xx.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://hm.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://uw.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jk.lnxyls.cn

);
来源：http://zn.lnxyls.cn

[Q03] 增加列
来源：http://pu.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fu.szsharing.cn

[Q04] 修改列类型
来源：http://vs.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ag.hnjuh.cn

[Q05] 重命名列
来源：http://xm.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rs.huanxung.cn

[Q06] 删除列
来源：http://sg.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ll.szxytkj.cn

[Q07] 删除表
来源：http://zz.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://ru.bjjhwx.cn

[Q08] 创建普通索引
来源：http://ql.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gl.nicolike.cn

[Q09] 创建唯一索引
来源：http://wl.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lu.szxytkj.cn

[Q10] 插入单行
来源：http://wm.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hm.huanxung.cn

[Q11] 一次插入多行
来源：http://dx.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lc.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://ua.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bz.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hd.szsharing.cn

[Q13] 忽略重复插入
来源：http://fo.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yi.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://hm.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ti.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cp.huixinmuqiang.cn

[Q15] 查询全部
来源：http://iu.yuexingan06.cn

SELECT * FROM users;
来源：http://hr.chemitech.net.cn

[Q16] 查询指定列
来源：http://qr.shxzskj.cn

SELECT id, name FROM users;
来源：http://ab.nszjky.cn

[Q17] 条件查询
来源：http://cu.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iw.hahajie.cn

[Q18] 模糊匹配
来源：http://uw.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ci.521024.cn

[Q19] 范围查询
来源：http://ua.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vo.haigaiapp.cn

[Q20] IN 列表
来源：http://tm.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yv.wgjwhj.cn

[Q21] 空值判断
来源：http://lj.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yj.shxzukj.cn

[Q22] 排序
来源：http://kj.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ox.shxzskj.cn

[Q23] 分页
来源：http://nm.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gq.bookmarksfly.cn

[Q24] 去重
来源：http://yv.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ai.gzmigu.cn

[Q25] 只取前 N 条
来源：http://dh.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kf.muxihuayi.cn

[Q26] 计数
来源：http://vg.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ge.bjjhwx.cn

[Q27] 条件计数
来源：http://vi.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rf.newstarts.cn

[Q28] 求和与平均
来源：http://dq.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zk.shxzskj.cn

[Q29] 最大最小值
来源：http://dy.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nr.hnjuh.cn

[Q30] 分组统计
来源：http://ah.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jm.panjiajie.cn

[Q31] 分组后过滤
来源：http://ay.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jb.nszjky.cn

[Q32] 分组拼接字符串
来源：http://lh.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oq.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yp.newstarts.cn

[Q33] 多列分组
来源：http://ef.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bc.panjiajie.cn

[Q34] 每组取第一条
来源：http://cg.bjjhwx.cn

SELECT * FROM (
来源：http://qq.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iz.nicolike.cn

) t WHERE rn = 1;
来源：http://jc.asd995.cn

[Q35] 内连接
来源：http://qe.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sp.haigaiapp.cn

[Q36] 左连接
来源：http://zz.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tl.huixiangedu.cn

[Q37] 右连接
来源：http://ao.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gk.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pc.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lo.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://ki.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rn.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cv.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kw.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ez.shxzskj.cn

[Q41] 多表连接
来源：http://kv.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ft.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://xo.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://iq.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://rq.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://vd.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sv.shxzskj.cn

[Q43] 标量子查询
来源：http://xl.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qs.bjjhwx.cn

[Q44] IN 子查询
来源：http://is.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qi.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://ws.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sh.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kq.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nd.newstarts.cn

[Q47] 与平均值比较
来源：http://hp.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ym.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://co.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://va.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://zd.huanxung.cn

[Q49] 更新单行
来源：http://bs.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pj.yuexingan06.cn

[Q50] 批量更新
来源：http://jm.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ah.newstarts.cn

[Q51] 用子查询更新
来源：http://pw.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gr.szxytkj.cn

[Q52] 删除指定行
来源：http://al.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://ip.bjjhwx.cn

[Q53] 按条件删除
来源：http://yf.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ow.9csxet.cn

[Q54] 清空表
来源：http://jw.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://vf.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://cs.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://un.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://ho.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xr.yuntaijiaju.cn

[Q57] 行号
来源：http://sp.521024.cn


<!-- 参考信息 -->