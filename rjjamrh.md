代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oh.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ge.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kb.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xi.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dk.szsharing.cn

[N10] 链表节点定义
来源：http://aa.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rx.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tp.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kd.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ye.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://jg.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fu.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hr.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ne.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://aq.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ie.9csxet.cn

PHP:  // 手写递归函数
来源：http://sm.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://it.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pl.szsharing.cn

Java: // 手写递归
来源：http://vw.huixinmuqiang.cn

Go:   // 手写递归
来源：http://lo.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ib.muxihuayi.cn

C#:   // 手写递归
来源：http://om.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ff.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yh.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xz.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ar.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fb.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://el.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ff.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mo.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pu.bjjhwx.cn

================================================================================
来源：http://ru.lnxyls.cn

O. 并发与异步
来源：http://cy.panjiajie.cn

================================================================================
来源：http://fb.nszjky.cn

[O01] 启动一个线程
来源：http://sm.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sa.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tr.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ug.wgjwhj.cn

TS:   // 同 JS
来源：http://gd.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://ab.hnjuh.cn

Go:   go f()
来源：http://wm.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://sb.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://gw.huanxung.cn

[O02] 使用线程池
来源：http://mb.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gj.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fn.huanxung.cn

JS:   // worker_threads 线程池
来源：http://uj.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://tk.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fb.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lp.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fs.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yn.nszjky.cn

[O03] 加锁保护共享数据
来源：http://ks.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://en.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://kr.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vx.jianghongdianzi.cn

TS:   // 同 JS
来源：http://jl.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://lj.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jh.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hl.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://ge.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://xe.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://fw.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cd.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://de.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ee.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eu.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oz.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://li.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://mk.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://se.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://ai.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dp.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://xq.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://ka.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cz.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://py.nicolike.cn

Ruby: threads.map(&:join)
来源：http://mp.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nb.huixinmuqiang.cn

[O06] 使用进程池
来源：http://df.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bl.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hy.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://jc.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://cn.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cl.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://je.9csxet.cn

Ruby: // fork 块
来源：http://bp.gzmigu.cn

C#:   Parallel.For
来源：http://wu.jianghongdianzi.cn

================================================================================
来源：http://yw.asd995.cn

P. 常用工具函数
来源：http://xm.chemitech.net.cn

================================================================================
来源：http://iq.szxytkj.cn

[P01] 生成 UUID
来源：http://ua.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://mr.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rk.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://os.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://vq.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://mb.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://ln.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://xp.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://zu.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://iz.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://in.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zx.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iv.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cs.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nf.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lu.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pn.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gt.hnjuh.cn

[P03] 生成短随机字符串
来源：http://qv.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rf.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ls.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kv.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lt.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ef.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://il.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jy.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gz.jctech888.com.cn

[P04] 求长度
来源：http://ie.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zf.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kr.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rx.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tj.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://qm.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://sd.9csxet.cn

Ruby: x.length;  x.size
来源：http://hb.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lh.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://fj.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tz.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mx.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://co.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gy.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yr.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://il.huanxung.cn

Ruby: a == b
来源：http://xc.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ge.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sc.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://db.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://ev.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://um.szsharing.cn

TS:   if (x == null) {}
来源：http://so.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zd.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://oq.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kp.panjiajie.cn

C#:   if (x is null) {}
来源：http://be.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://sd.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rg.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://ee.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yi.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gp.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tk.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xo.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tg.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://by.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://sr.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xx.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eu.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ef.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lp.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eq.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qz.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lq.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jt.colortex.cn

================================================================================
来源：http://lc.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qe.9csxet.cn

================================================================================
来源：http://cb.newstarts.cn

[Q01] 创建表
来源：http://qh.szsharing.cn

CREATE TABLE users (
来源：http://oy.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hc.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://ez.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://wj.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ek.muxihuayi.cn

);
来源：http://pv.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://uv.lnxyls.cn

CREATE TABLE orders (
来源：http://ry.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lm.jctech888.com.cn

user_id INT NOT NULL,
来源：http://yo.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://wd.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ys.asd995.cn

);
来源：http://sj.9csxet.cn

[Q03] 增加列
来源：http://dz.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uy.szxytkj.cn

[Q04] 修改列类型
来源：http://ff.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xm.huixinmuqiang.cn

[Q05] 重命名列
来源：http://al.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gw.hnjuh.cn

[Q06] 删除列
来源：http://co.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tw.shxzukj.cn

[Q07] 删除表
来源：http://wf.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://qq.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://xi.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bo.shxzskj.cn

[Q09] 创建唯一索引
来源：http://yb.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wr.yuexingan06.cn

[Q10] 插入单行
来源：http://cb.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cd.lnxyls.cn

[Q11] 一次插入多行
来源：http://hn.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lv.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://yu.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zt.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gq.nicolike.cn

[Q13] 忽略重复插入
来源：http://pn.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wy.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://nz.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mq.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wb.nszjky.cn

[Q15] 查询全部
来源：http://vv.chemitech.net.cn

SELECT * FROM users;
来源：http://pp.yuexingan06.cn

[Q16] 查询指定列
来源：http://dz.newstarts.cn

SELECT id, name FROM users;
来源：http://bb.bookmarksfly.cn

[Q17] 条件查询
来源：http://jy.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uv.gzmigu.cn

[Q18] 模糊匹配
来源：http://id.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bd.szsharing.cn

[Q19] 范围查询
来源：http://ql.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zz.colortex.cn

[Q20] IN 列表
来源：http://ha.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hw.huixiangedu.cn

[Q21] 空值判断
来源：http://ha.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vr.szsharing.cn

[Q22] 排序
来源：http://pu.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tt.9csxet.cn

[Q23] 分页
来源：http://sf.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qy.panjiajie.cn

[Q24] 去重
来源：http://lb.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://pl.newstarts.cn

[Q25] 只取前 N 条
来源：http://uw.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ws.bookmarksfly.cn

[Q26] 计数
来源：http://ei.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://nx.huanxung.cn

[Q27] 条件计数
来源：http://uu.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dw.huixiangedu.cn

[Q28] 求和与平均
来源：http://al.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wc.shtwfgs.cn

[Q29] 最大最小值
来源：http://ad.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sb.9csxet.cn

[Q30] 分组统计
来源：http://lg.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rq.panjiajie.cn

[Q31] 分组后过滤
来源：http://oq.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fk.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://hc.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://of.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rk.gzmigu.cn

[Q33] 多列分组
来源：http://cg.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qa.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://gm.wgjwhj.cn

SELECT * FROM (
来源：http://em.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uu.lnxyls.cn

) t WHERE rn = 1;
来源：http://cz.huixinmuqiang.cn

[Q35] 内连接
来源：http://uc.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nj.yuntaijiaju.cn

[Q36] 左连接
来源：http://yr.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ur.chemitech.net.cn

[Q37] 右连接
来源：http://rw.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wc.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ku.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yv.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://pl.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://up.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yl.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://md.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://or.bookmarksfly.cn

[Q41] 多表连接
来源：http://uf.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://up.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://fs.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://cm.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://nt.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://kn.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://he.huanxung.cn

[Q43] 标量子查询
来源：http://ik.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zz.huanxung.cn

[Q44] IN 子查询
来源：http://vp.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lu.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://ce.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://br.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fz.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cv.jctech888.com.cn

[Q47] 与平均值比较
来源：http://ng.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://th.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://tc.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ea.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://eo.shtwfgs.cn

[Q49] 更新单行
来源：http://bx.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ps.huanxung.cn

[Q50] 批量更新
来源：http://ck.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://td.newstarts.cn

[Q51] 用子查询更新
来源：http://bl.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pu.panjiajie.cn

[Q52] 删除指定行
来源：http://td.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://xh.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://xu.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ta.wgjwhj.cn

[Q54] 清空表
来源：http://mj.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://lt.newstarts.cn

[Q55] 排名（并列占位）
来源：http://pl.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bt.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://cq.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ce.colortex.cn

[Q57] 行号
来源：http://bg.szsharing.cn


<!-- 参考信息 -->