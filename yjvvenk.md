代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://az.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://od.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bk.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xz.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ms.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://tx.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zs.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ea.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vu.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vf.521024.cn

Java: class Node { int v; Node next; }
来源：http://qn.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lj.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jr.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xu.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://yt.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fv.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://xb.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yg.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mz.jctech888.com.cn

Java: // 手写递归
来源：http://rg.wgjwhj.cn

Go:   // 手写递归
来源：http://sl.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gh.hahajie.cn

C#:   // 手写递归
来源：http://hy.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nq.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jp.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xs.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wd.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rz.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ij.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ca.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xa.muxihuayi.cn

================================================================================
来源：http://th.shxzukj.cn

O. 并发与异步
来源：http://wo.yuexingan06.cn

================================================================================
来源：http://ox.szxytkj.cn

[O01] 启动一个线程
来源：http://rm.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dz.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ur.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ac.hnjuh.cn

TS:   // 同 JS
来源：http://kk.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://jw.bjjhwx.cn

Go:   go f()
来源：http://ng.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://hg.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://dg.jctech888.com.cn

[O02] 使用线程池
来源：http://bu.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ho.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lp.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://ep.asd995.cn

TS:   // worker_threads 线程池
来源：http://tk.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yj.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zy.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xi.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://zu.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://ae.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ix.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gj.shtwfgs.cn

TS:   // 同 JS
来源：http://ja.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://sh.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sl.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rb.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://iv.szsharing.cn

[O04] 定义异步函数并等待
来源：http://nu.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://gb.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xz.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://yw.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ll.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ik.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ez.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eu.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://sa.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://wj.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ms.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://en.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://io.asd995.cn

TS:   await Promise.all(tasks)
来源：http://gg.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xi.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lq.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://gl.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xe.jctech888.com.cn

[O06] 使用进程池
来源：http://tv.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kw.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://so.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://rh.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://yk.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qz.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tp.jianghongdianzi.cn

Ruby: // fork 块
来源：http://vr.hnjuh.cn

C#:   Parallel.For
来源：http://lp.chemitech.net.cn

================================================================================
来源：http://vk.521024.cn

P. 常用工具函数
来源：http://fb.yuexingan06.cn

================================================================================
来源：http://fh.newstarts.cn

[P01] 生成 UUID
来源：http://uu.asd995.cn

Py:   str(uuid.uuid4())
来源：http://jt.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gq.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://ay.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://bu.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://he.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://on.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://we.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://dp.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://ue.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nu.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nw.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zb.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ze.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yr.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nl.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sh.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ih.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://oq.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gp.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yh.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gv.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sp.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qq.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gb.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xf.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ad.huixiangedu.cn

[P04] 求长度
来源：http://qj.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hx.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ls.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yv.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uf.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://rh.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://gw.newstarts.cn

Ruby: x.length;  x.size
来源：http://qv.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ao.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://al.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uy.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ju.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jd.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hi.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rz.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zs.asd995.cn

Ruby: a == b
来源：http://wc.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vd.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pn.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rj.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://lr.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vw.szxytkj.cn

TS:   if (x == null) {}
来源：http://fy.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ic.hnjuh.cn

Go:   if x == nil {}
来源：http://ee.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ob.haigaiapp.cn

C#:   if (x is null) {}
来源：http://er.chemitech.net.cn

[P07] 防抖与节流
来源：http://qq.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rn.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://nl.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rv.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kg.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hn.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rb.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cb.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://th.hahajie.cn

[P08] 处理浮点精度问题
来源：http://ir.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sr.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ff.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qv.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ab.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://or.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rm.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://po.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gx.yuntaijiaju.cn

================================================================================
来源：http://dw.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ck.hahajie.cn

================================================================================
来源：http://mh.bookmarksfly.cn

[Q01] 创建表
来源：http://zo.yuntaijiaju.cn

CREATE TABLE users (
来源：http://ko.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wd.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://uk.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://ry.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vl.colortex.cn

);
来源：http://jz.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://yf.szsharing.cn

CREATE TABLE orders (
来源：http://jr.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vj.9csxet.cn

user_id INT NOT NULL,
来源：http://tg.colortex.cn

amount DECIMAL(10, 2),
来源：http://gk.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qi.bjjhwx.cn

);
来源：http://zc.chemitech.net.cn

[Q03] 增加列
来源：http://hm.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://db.hahajie.cn

[Q04] 修改列类型
来源：http://ad.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uq.yuntaijiaju.cn

[Q05] 重命名列
来源：http://xg.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sd.hahajie.cn

[Q06] 删除列
来源：http://mn.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gu.hahajie.cn

[Q07] 删除表
来源：http://bl.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://qp.521024.cn

[Q08] 创建普通索引
来源：http://ra.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://my.521024.cn

[Q09] 创建唯一索引
来源：http://zz.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://td.gzmigu.cn

[Q10] 插入单行
来源：http://ds.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://su.wgjwhj.cn

[Q11] 一次插入多行
来源：http://ai.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rq.521024.cn

[Q12] 插入后取自增 ID
来源：http://gb.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qy.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fi.nicolike.cn

[Q13] 忽略重复插入
来源：http://el.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gf.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://cq.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oh.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rh.wgjwhj.cn

[Q15] 查询全部
来源：http://px.muxihuayi.cn

SELECT * FROM users;
来源：http://mg.asd995.cn

[Q16] 查询指定列
来源：http://hw.huixiangedu.cn

SELECT id, name FROM users;
来源：http://hs.bookmarksfly.cn

[Q17] 条件查询
来源：http://xk.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fj.nszjky.cn

[Q18] 模糊匹配
来源：http://hy.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jv.gzmigu.cn

[Q19] 范围查询
来源：http://fv.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lg.hnjuh.cn

[Q20] IN 列表
来源：http://ct.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yc.nszjky.cn

[Q21] 空值判断
来源：http://yp.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kq.chemitech.net.cn

[Q22] 排序
来源：http://gn.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kb.yuntaijiaju.cn

[Q23] 分页
来源：http://lq.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vn.521024.cn

[Q24] 去重
来源：http://te.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://yj.hahajie.cn

[Q25] 只取前 N 条
来源：http://fr.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oa.nszjky.cn

[Q26] 计数
来源：http://nw.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://zf.shxzukj.cn

[Q27] 条件计数
来源：http://dt.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://es.panjiajie.cn

[Q28] 求和与平均
来源：http://kb.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lw.bookmarksfly.cn

[Q29] 最大最小值
来源：http://hm.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vi.szxytkj.cn

[Q30] 分组统计
来源：http://ch.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ux.newstarts.cn

[Q31] 分组后过滤
来源：http://qs.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ax.nszjky.cn

[Q32] 分组拼接字符串
来源：http://af.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xf.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uo.jianghongdianzi.cn

[Q33] 多列分组
来源：http://ce.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lb.huixiangedu.cn

[Q34] 每组取第一条
来源：http://xe.521024.cn

SELECT * FROM (
来源：http://ct.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xn.szsharing.cn

) t WHERE rn = 1;
来源：http://ht.szxytkj.cn

[Q35] 内连接
来源：http://fp.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dc.shxzukj.cn

[Q36] 左连接
来源：http://gi.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ba.yuexingan06.cn

[Q37] 右连接
来源：http://lz.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ld.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jo.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hj.colortex.cn

[Q39] 自连接（查上下级）
来源：http://hk.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aw.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ka.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dv.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gq.colortex.cn

[Q41] 多表连接
来源：http://dc.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://be.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://an.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://ju.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://lv.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://ed.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kp.shtwfgs.cn

[Q43] 标量子查询
来源：http://ic.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ip.bookmarksfly.cn

[Q44] IN 子查询
来源：http://jb.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pv.asd995.cn

[Q45] EXISTS 判断存在
来源：http://kx.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dr.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ta.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bu.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://gn.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://le.colortex.cn

[Q48] CTE 公用表表达式
来源：http://cc.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dj.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://oy.jianghongdianzi.cn

[Q49] 更新单行
来源：http://dk.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vt.haigaiapp.cn

[Q50] 批量更新
来源：http://vi.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jl.muxihuayi.cn

[Q51] 用子查询更新
来源：http://xf.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bi.colortex.cn

[Q52] 删除指定行
来源：http://vw.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://kz.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://kx.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xf.newstarts.cn

[Q54] 清空表
来源：http://jf.huanxung.cn

TRUNCATE TABLE logs;
来源：http://uk.nicolike.cn

[Q55] 排名（并列占位）
来源：http://da.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://os.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://nm.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fn.huixiangedu.cn

[Q57] 行号
来源：http://zb.shxzskj.cn


<!-- 参考信息 -->