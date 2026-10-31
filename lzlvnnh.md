代发 wailian999

[N09] 栈与队列
来源：http://cl.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ni.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sm.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yy.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qg.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tx.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bj.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://di.shxzukj.cn

[N10] 链表节点定义
来源：http://tf.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mn.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ty.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://px.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://be.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://vp.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zj.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hx.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wa.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://nd.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hd.lnxyls.cn

PHP:  // 手写递归函数
来源：http://jy.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nx.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ab.chemitech.net.cn

Java: // 手写递归
来源：http://ay.yuexingan06.cn

Go:   // 手写递归
来源：http://sb.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hd.huixinmuqiang.cn

C#:   // 手写递归
来源：http://sd.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lz.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oo.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://np.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oy.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xr.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xf.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jw.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iv.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kb.colortex.cn

================================================================================
来源：http://xk.9csxet.cn

O. 并发与异步
来源：http://wy.chemitech.net.cn

================================================================================
来源：http://kg.bjjhwx.cn

[O01] 启动一个线程
来源：http://yt.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qt.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iz.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cn.colortex.cn

TS:   // 同 JS
来源：http://pi.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://dd.yuexingan06.cn

Go:   go f()
来源：http://iu.szsharing.cn

Ruby: Thread.new { f }
来源：http://pk.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://hx.huanxung.cn

[O02] 使用线程池
来源：http://ax.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zd.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cn.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://pj.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://qw.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fo.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vy.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yz.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xv.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://or.shxzskj.cn

Py:   with lock: shared += 1
来源：http://nn.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://yh.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ru.jianghongdianzi.cn

TS:   // 同 JS
来源：http://us.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://to.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ya.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pr.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://vb.9csxet.cn

[O04] 定义异步函数并等待
来源：http://wd.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://ws.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pa.521024.cn

JS:   async function f() { await g(); }
来源：http://dx.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rn.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fq.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ut.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nn.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://ia.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://dh.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://wp.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jh.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://rf.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://uc.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://to.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ai.nszjky.cn

Ruby: threads.map(&:join)
来源：http://om.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sb.shxzskj.cn

[O06] 使用进程池
来源：http://xd.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sa.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sy.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://rp.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://zv.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sf.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sk.szxytkj.cn

Ruby: // fork 块
来源：http://lq.yuexingan06.cn

C#:   Parallel.For
来源：http://uj.szsharing.cn

================================================================================
来源：http://xm.asd995.cn

P. 常用工具函数
来源：http://ib.panjiajie.cn

================================================================================
来源：http://vq.wgjwhj.cn

[P01] 生成 UUID
来源：http://xi.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://sw.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ev.9csxet.cn

JS:   crypto.randomUUID()
来源：http://nv.asd995.cn

TS:   crypto.randomUUID()
来源：http://eq.521024.cn

Java: UUID.randomUUID().toString()
来源：http://cx.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://eb.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://uz.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://be.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://fs.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lk.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zt.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lr.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oc.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hi.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sv.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://le.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bh.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://xa.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mg.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fi.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://at.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kd.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qc.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kt.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ct.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ev.yuntaijiaju.cn

[P04] 求长度
来源：http://ct.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://al.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pr.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mi.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xf.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://td.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://wm.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://ke.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kz.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://xf.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vb.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sx.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gy.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ob.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bc.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ih.muxihuayi.cn

Ruby: a == b
来源：http://sy.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jk.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yi.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rb.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://uk.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cv.huanxung.cn

TS:   if (x == null) {}
来源：http://tn.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bw.newstarts.cn

Go:   if x == nil {}
来源：http://eq.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cp.shxzukj.cn

C#:   if (x is null) {}
来源：http://jr.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://qu.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cc.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://un.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eq.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pq.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kt.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jq.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gy.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jr.szsharing.cn

[P08] 处理浮点精度问题
来源：http://wt.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zx.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ep.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kj.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jn.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iw.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tf.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qn.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://si.szxytkj.cn

================================================================================
来源：http://hu.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xn.colortex.cn

================================================================================
来源：http://ab.panjiajie.cn

[Q01] 创建表
来源：http://cy.colortex.cn

CREATE TABLE users (
来源：http://qo.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sh.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://pu.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://mr.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cp.gzmigu.cn

);
来源：http://ez.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://ge.newstarts.cn

CREATE TABLE orders (
来源：http://po.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pe.hnjuh.cn

user_id INT NOT NULL,
来源：http://gr.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://hm.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ae.chemitech.net.cn

);
来源：http://mj.bookmarksfly.cn

[Q03] 增加列
来源：http://ys.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cw.shxzskj.cn

[Q04] 修改列类型
来源：http://ut.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sn.huixinmuqiang.cn

[Q05] 重命名列
来源：http://sx.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://el.chemitech.net.cn

[Q06] 删除列
来源：http://pe.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ua.shxzukj.cn

[Q07] 删除表
来源：http://nx.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ec.wgjwhj.cn

[Q08] 创建普通索引
来源：http://ak.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hd.newstarts.cn

[Q09] 创建唯一索引
来源：http://bk.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ad.shxzukj.cn

[Q10] 插入单行
来源：http://tv.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://do.szsharing.cn

[Q11] 一次插入多行
来源：http://sj.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ai.colortex.cn

[Q12] 插入后取自增 ID
来源：http://fg.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vc.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://at.lnxyls.cn

[Q13] 忽略重复插入
来源：http://yj.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ty.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://yw.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ox.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mh.nszjky.cn

[Q15] 查询全部
来源：http://im.nicolike.cn

SELECT * FROM users;
来源：http://bj.hnjuh.cn

[Q16] 查询指定列
来源：http://xm.szsharing.cn

SELECT id, name FROM users;
来源：http://ez.521024.cn

[Q17] 条件查询
来源：http://rn.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qw.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://fr.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qi.wgjwhj.cn

[Q19] 范围查询
来源：http://yu.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oy.chemitech.net.cn

[Q20] IN 列表
来源：http://ow.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wl.shxzskj.cn

[Q21] 空值判断
来源：http://se.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cz.jianghongdianzi.cn

[Q22] 排序
来源：http://cw.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gu.huanxung.cn

[Q23] 分页
来源：http://vj.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yw.chemitech.net.cn

[Q24] 去重
来源：http://aw.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://cj.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://px.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qe.chemitech.net.cn

[Q26] 计数
来源：http://vp.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://hd.huanxung.cn

[Q27] 条件计数
来源：http://zm.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pq.colortex.cn

[Q28] 求和与平均
来源：http://ky.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ue.haigaiapp.cn

[Q29] 最大最小值
来源：http://no.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nv.shxzukj.cn

[Q30] 分组统计
来源：http://ms.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ip.bjjhwx.cn

[Q31] 分组后过滤
来源：http://xg.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sx.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://pv.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gw.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ra.nicolike.cn

[Q33] 多列分组
来源：http://mb.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tg.asd995.cn

[Q34] 每组取第一条
来源：http://jd.shxzskj.cn

SELECT * FROM (
来源：http://fn.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vh.bjjhwx.cn

) t WHERE rn = 1;
来源：http://lx.hnjuh.cn

[Q35] 内连接
来源：http://kz.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sb.jianghongdianzi.cn

[Q36] 左连接
来源：http://nh.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://go.asd995.cn

[Q37] 右连接
来源：http://ga.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gi.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uq.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ri.colortex.cn

[Q39] 自连接（查上下级）
来源：http://io.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lq.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gr.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nf.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jv.yuexingan06.cn

[Q41] 多表连接
来源：http://xb.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kc.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://oo.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ki.asd995.cn

[Q42] 连接条件附加过滤
来源：http://dn.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://rz.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pt.nicolike.cn

[Q43] 标量子查询
来源：http://tm.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fi.yuexingan06.cn

[Q44] IN 子查询
来源：http://kw.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ex.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://um.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://to.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dk.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hx.gzmigu.cn

[Q47] 与平均值比较
来源：http://zm.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cd.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://io.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wl.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ok.lnxyls.cn

[Q49] 更新单行
来源：http://im.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oe.muxihuayi.cn

[Q50] 批量更新
来源：http://qq.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uq.asd995.cn

[Q51] 用子查询更新
来源：http://ps.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.panjiajie.cn

[Q52] 删除指定行
来源：http://ty.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://ks.szxytkj.cn

[Q53] 按条件删除
来源：http://qf.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kf.muxihuayi.cn

[Q54] 清空表
来源：http://qt.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://qt.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://wt.yuntaijiaju.cn


<!-- 参考信息 -->