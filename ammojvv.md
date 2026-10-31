代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yl.shtwfgs.cn

[N10] 链表节点定义
来源：http://zv.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ig.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uc.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sx.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eu.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://qv.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zy.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cs.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://em.huanxung.cn

[N11] 二叉树中序遍历
来源：http://ud.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://st.hnjuh.cn

PHP:  // 手写递归函数
来源：http://qi.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ee.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kt.colortex.cn

Java: // 手写递归
来源：http://do.hahajie.cn

Go:   // 手写递归
来源：http://qr.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ty.huanxung.cn

C#:   // 手写递归
来源：http://rq.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ow.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ih.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bp.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tz.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vc.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://up.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://th.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jv.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wl.newstarts.cn

================================================================================
来源：http://db.huixinmuqiang.cn

O. 并发与异步
来源：http://rr.szxytkj.cn

================================================================================
来源：http://pj.yuexingan06.cn

[O01] 启动一个线程
来源：http://gl.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lp.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fl.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pj.hahajie.cn

TS:   // 同 JS
来源：http://ii.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://gi.huixiangedu.cn

Go:   go f()
来源：http://ht.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://mh.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://yd.huanxung.cn

[O02] 使用线程池
来源：http://ac.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sh.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ou.newstarts.cn

JS:   // worker_threads 线程池
来源：http://of.szsharing.cn

TS:   // worker_threads 线程池
来源：http://sf.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bo.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zi.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vg.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://by.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://yq.nszjky.cn

Py:   with lock: shared += 1
来源：http://xn.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://cb.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pc.gzmigu.cn

TS:   // 同 JS
来源：http://sh.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://gy.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://te.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sg.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://wh.newstarts.cn

[O04] 定义异步函数并等待
来源：http://fp.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://mi.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tl.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://jv.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uu.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fc.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lq.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ut.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://py.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://fx.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://gv.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hh.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://wg.colortex.cn

TS:   await Promise.all(tasks)
来源：http://of.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ic.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fp.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://rm.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jk.nszjky.cn

[O06] 使用进程池
来源：http://eo.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ny.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ga.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://hi.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://uk.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gc.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ft.9csxet.cn

Ruby: // fork 块
来源：http://cb.panjiajie.cn

C#:   Parallel.For
来源：http://tx.hahajie.cn

================================================================================
来源：http://wb.yuntaijiaju.cn

P. 常用工具函数
来源：http://kl.huanxung.cn

================================================================================
来源：http://am.shtwfgs.cn

[P01] 生成 UUID
来源：http://um.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://tm.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hx.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://pu.newstarts.cn

TS:   crypto.randomUUID()
来源：http://ju.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://wz.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://vi.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://tb.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://eu.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://cu.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aj.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vf.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lh.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xh.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gb.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hr.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bh.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fk.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://fq.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rp.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pa.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qk.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iv.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ea.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jt.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ki.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sf.szxytkj.cn

[P04] 求长度
来源：http://tw.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ry.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vq.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gl.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vk.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://zg.szsharing.cn

Go:   len(arr);  len(m)
来源：http://dd.szxytkj.cn

Ruby: x.length;  x.size
来源：http://dq.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vg.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://en.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jc.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xn.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wc.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zi.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cm.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ap.yuexingan06.cn

Ruby: a == b
来源：http://bp.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sv.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://az.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://av.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://up.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hn.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://kh.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gn.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://nn.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pk.newstarts.cn

C#:   if (x is null) {}
来源：http://iz.wgjwhj.cn

[P07] 防抖与节流
来源：http://hm.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uy.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://wk.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sn.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ef.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nj.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iy.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qh.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uu.nszjky.cn

[P08] 处理浮点精度问题
来源：http://qg.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ck.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wz.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mu.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bc.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wl.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pm.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nl.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gv.nszjky.cn

================================================================================
来源：http://sx.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mq.huanxung.cn

================================================================================
来源：http://ex.shxzskj.cn

[Q01] 创建表
来源：http://pb.newstarts.cn

CREATE TABLE users (
来源：http://mm.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qj.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://zj.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://ue.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uf.hahajie.cn

);
来源：http://kz.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://tr.newstarts.cn

CREATE TABLE orders (
来源：http://yt.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ud.wgjwhj.cn

user_id INT NOT NULL,
来源：http://jy.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://xc.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zn.jianghongdianzi.cn

);
来源：http://we.szsharing.cn

[Q03] 增加列
来源：http://hi.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vg.9csxet.cn

[Q04] 修改列类型
来源：http://py.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sx.panjiajie.cn

[Q05] 重命名列
来源：http://fw.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zs.szxytkj.cn

[Q06] 删除列
来源：http://hm.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ko.colortex.cn

[Q07] 删除表
来源：http://dl.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://xd.gzmigu.cn

[Q08] 创建普通索引
来源：http://vf.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jl.nszjky.cn

[Q09] 创建唯一索引
来源：http://cp.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kl.colortex.cn

[Q10] 插入单行
来源：http://di.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mv.huixiangedu.cn

[Q11] 一次插入多行
来源：http://ih.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wb.521024.cn

[Q12] 插入后取自增 ID
来源：http://le.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uw.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://au.521024.cn

[Q13] 忽略重复插入
来源：http://vm.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uy.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://xw.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hg.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qu.wgjwhj.cn

[Q15] 查询全部
来源：http://mk.jianghongdianzi.cn

SELECT * FROM users;
来源：http://eu.newstarts.cn

[Q16] 查询指定列
来源：http://nx.huanxung.cn

SELECT id, name FROM users;
来源：http://qn.lnxyls.cn

[Q17] 条件查询
来源：http://cl.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kb.bjjhwx.cn

[Q18] 模糊匹配
来源：http://co.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pg.nszjky.cn

[Q19] 范围查询
来源：http://dr.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oz.jianghongdianzi.cn

[Q20] IN 列表
来源：http://rv.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jy.huixinmuqiang.cn

[Q21] 空值判断
来源：http://gg.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dp.muxihuayi.cn

[Q22] 排序
来源：http://na.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dg.hnjuh.cn

[Q23] 分页
来源：http://po.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gj.szsharing.cn

[Q24] 去重
来源：http://lq.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://ic.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://hg.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eu.jctech888.com.cn

[Q26] 计数
来源：http://ic.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://qn.huanxung.cn

[Q27] 条件计数
来源：http://at.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://br.nicolike.cn

[Q28] 求和与平均
来源：http://uo.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ti.gzmigu.cn

[Q29] 最大最小值
来源：http://hs.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kz.panjiajie.cn

[Q30] 分组统计
来源：http://th.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nn.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://df.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uk.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://nb.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wi.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yx.colortex.cn

[Q33] 多列分组
来源：http://tt.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vk.shtwfgs.cn

[Q34] 每组取第一条
来源：http://rm.jctech888.com.cn

SELECT * FROM (
来源：http://sg.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jp.haigaiapp.cn

) t WHERE rn = 1;
来源：http://zz.9csxet.cn

[Q35] 内连接
来源：http://as.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dz.shxzskj.cn

[Q36] 左连接
来源：http://tj.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tt.shxzukj.cn

[Q37] 右连接
来源：http://sd.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pf.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://re.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sq.521024.cn

[Q39] 自连接（查上下级）
来源：http://ee.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ro.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xl.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yz.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hy.asd995.cn

[Q41] 多表连接
来源：http://hp.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dt.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://vo.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://em.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://ip.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://ph.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wq.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://bm.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gx.muxihuayi.cn

[Q44] IN 子查询
来源：http://ln.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wv.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://ac.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ec.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sh.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gs.colortex.cn

[Q47] 与平均值比较
来源：http://ws.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gg.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://rz.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cm.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://po.521024.cn

[Q49] 更新单行
来源：http://xb.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eo.chemitech.net.cn

[Q50] 批量更新
来源：http://ta.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tu.hahajie.cn

[Q51] 用子查询更新
来源：http://gp.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://am.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://xs.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://dv.yuexingan06.cn

[Q53] 按条件删除
来源：http://cl.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zj.lnxyls.cn

[Q54] 清空表
来源：http://nr.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://pp.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://sm.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uq.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://nl.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ew.colortex.cn

[Q57] 行号
来源：http://je.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ty.chemitech.net.cn

[Q58] 累计求和
来源：http://af.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ka.yuexingan06.cn

[Q59] 分组内累计
来源：http://zw.huanxung.cn


<!-- 参考信息 -->