代发 wailian999

Py:   itertools.permutations(arr)
来源：http://sz.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://jg.9csxet.cn

JS:   // 手写回溯递归
来源：http://gg.szxytkj.cn

TS:   // 手写回溯递归
来源：http://yo.haigaiapp.cn

Java: // 手写回溯递归
来源：http://dg.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ci.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://az.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://qy.jianghongdianzi.cn

[N09] 栈与队列
来源：http://qd.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://im.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://me.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fq.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jg.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fg.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pa.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bj.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bi.colortex.cn

[N10] 链表节点定义
来源：http://bs.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sn.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ab.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mb.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kr.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://yu.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sm.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ye.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xc.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://xj.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ve.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://gs.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://la.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qm.9csxet.cn

Java: // 手写递归
来源：http://uy.gzmigu.cn

Go:   // 手写递归
来源：http://xo.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vi.jianghongdianzi.cn

C#:   // 手写递归
来源：http://qn.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yo.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lf.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fz.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cq.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ee.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rx.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vc.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cm.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mt.bookmarksfly.cn

================================================================================
来源：http://wc.nszjky.cn

O. 并发与异步
来源：http://cg.bjjhwx.cn

================================================================================
来源：http://vy.szxytkj.cn

[O01] 启动一个线程
来源：http://it.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jz.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ld.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mq.muxihuayi.cn

TS:   // 同 JS
来源：http://rp.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://nq.hahajie.cn

Go:   go f()
来源：http://cn.hnjuh.cn

Ruby: Thread.new { f }
来源：http://np.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://el.yuntaijiaju.cn

[O02] 使用线程池
来源：http://fg.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vk.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://of.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://di.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://az.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hk.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xb.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hr.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wg.nicolike.cn

[O03] 加锁保护共享数据
来源：http://kj.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://kc.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://gr.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://it.521024.cn

TS:   // 同 JS
来源：http://dg.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://zp.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://th.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ej.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://bs.asd995.cn

[O04] 定义异步函数并等待
来源：http://qu.asd995.cn

Py:   async def f():⏎    await g()
来源：http://rs.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://az.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ts.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ut.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vv.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yd.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://us.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://or.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://jh.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://uf.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gu.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://tj.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://me.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zl.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lz.huanxung.cn

Ruby: threads.map(&:join)
来源：http://wf.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uk.lnxyls.cn

[O06] 使用进程池
来源：http://se.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zd.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cn.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://gp.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://et.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lu.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cq.huixiangedu.cn

Ruby: // fork 块
来源：http://pq.hnjuh.cn

C#:   Parallel.For
来源：http://co.wgjwhj.cn

================================================================================
来源：http://yo.jctech888.com.cn

P. 常用工具函数
来源：http://vn.panjiajie.cn

================================================================================
来源：http://ux.hahajie.cn

[P01] 生成 UUID
来源：http://jv.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://rw.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://me.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://mx.colortex.cn

TS:   crypto.randomUUID()
来源：http://mg.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://tt.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://ii.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://ht.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://be.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://zz.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sw.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oj.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yw.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tw.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fr.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lc.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tx.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ob.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://gy.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pr.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xo.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mj.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rh.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dk.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fi.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pp.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ao.jctech888.com.cn

[P04] 求长度
来源：http://cq.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bn.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yo.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gc.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sy.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://wm.szsharing.cn

Go:   len(arr);  len(m)
来源：http://qv.521024.cn

Ruby: x.length;  x.size
来源：http://sm.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zo.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://bf.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jj.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vy.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://df.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jw.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ux.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yy.shxzskj.cn

Ruby: a == b
来源：http://ji.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gc.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zz.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lx.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://rl.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oo.nicolike.cn

TS:   if (x == null) {}
来源：http://mb.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mx.huixiangedu.cn

Go:   if x == nil {}
来源：http://ka.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ux.asd995.cn

C#:   if (x is null) {}
来源：http://lq.gzmigu.cn

[P07] 防抖与节流
来源：http://dr.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pp.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://af.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cn.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://op.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pm.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bz.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zw.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fl.colortex.cn

[P08] 处理浮点精度问题
来源：http://vq.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wp.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://au.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://is.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fr.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hj.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cw.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ia.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dc.yuexingan06.cn

================================================================================
来源：http://tr.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tu.szxytkj.cn

================================================================================
来源：http://zc.lnxyls.cn

[Q01] 创建表
来源：http://ih.haigaiapp.cn

CREATE TABLE users (
来源：http://xr.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pr.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://en.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://ue.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vk.chemitech.net.cn

);
来源：http://lt.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://ip.nicolike.cn

CREATE TABLE orders (
来源：http://do.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kx.shxzskj.cn

user_id INT NOT NULL,
来源：http://yg.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://jp.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zd.szxytkj.cn

);
来源：http://tl.lnxyls.cn

[Q03] 增加列
来源：http://cc.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hk.nicolike.cn

[Q04] 修改列类型
来源：http://nx.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uj.huixiangedu.cn

[Q05] 重命名列
来源：http://fc.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ml.9csxet.cn

[Q06] 删除列
来源：http://lt.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bz.haigaiapp.cn

[Q07] 删除表
来源：http://jt.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://hx.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://lm.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qj.nszjky.cn

[Q09] 创建唯一索引
来源：http://yx.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mf.lnxyls.cn

[Q10] 插入单行
来源：http://uz.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ui.newstarts.cn

[Q11] 一次插入多行
来源：http://hu.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ik.asd995.cn

[Q12] 插入后取自增 ID
来源：http://dr.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xz.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shxzukj.cn

[Q13] 忽略重复插入
来源：http://ty.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vi.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://lz.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vx.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sk.asd995.cn

[Q15] 查询全部
来源：http://pg.bjjhwx.cn

SELECT * FROM users;
来源：http://vt.asd995.cn

[Q16] 查询指定列
来源：http://cm.muxihuayi.cn

SELECT id, name FROM users;
来源：http://fi.nicolike.cn

[Q17] 条件查询
来源：http://iw.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fc.hahajie.cn

[Q18] 模糊匹配
来源：http://lh.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tk.szxytkj.cn

[Q19] 范围查询
来源：http://jh.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wj.szxytkj.cn

[Q20] IN 列表
来源：http://ui.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rm.shtwfgs.cn

[Q21] 空值判断
来源：http://uq.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cu.hahajie.cn

[Q22] 排序
来源：http://ij.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fr.newstarts.cn

[Q23] 分页
来源：http://hi.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ru.shxzukj.cn

[Q24] 去重
来源：http://yt.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://at.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://gr.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fm.hnjuh.cn

[Q26] 计数
来源：http://sg.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://tz.szxytkj.cn

[Q27] 条件计数
来源：http://et.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ff.nszjky.cn

[Q28] 求和与平均
来源：http://xl.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cl.huixiangedu.cn

[Q29] 最大最小值
来源：http://bo.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jb.szxytkj.cn

[Q30] 分组统计
来源：http://va.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://no.shxzskj.cn

[Q31] 分组后过滤
来源：http://hk.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mq.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://gq.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zf.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rg.yuexingan06.cn

[Q33] 多列分组
来源：http://rr.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wl.muxihuayi.cn

[Q34] 每组取第一条
来源：http://qz.colortex.cn

SELECT * FROM (
来源：http://wn.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lv.szsharing.cn

) t WHERE rn = 1;
来源：http://ct.huanxung.cn

[Q35] 内连接
来源：http://va.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nf.huanxung.cn

[Q36] 左连接
来源：http://ri.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://af.9csxet.cn

[Q37] 右连接
来源：http://vd.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mv.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gu.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qj.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://ay.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://em.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qb.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ch.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dv.muxihuayi.cn

[Q41] 多表连接
来源：http://dy.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ev.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://mj.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://wp.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://yb.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://xr.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tl.szsharing.cn

[Q43] 标量子查询
来源：http://ds.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lq.haigaiapp.cn

[Q44] IN 子查询
来源：http://dn.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ui.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://tr.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rr.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hr.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ho.9csxet.cn

[Q47] 与平均值比较
来源：http://ey.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tf.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://mq.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ca.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://jg.nszjky.cn

[Q49] 更新单行
来源：http://kv.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sz.szxytkj.cn

[Q50] 批量更新
来源：http://hk.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xw.9csxet.cn

[Q51] 用子查询更新
来源：http://rc.jctech888.com.cn


<!-- 参考信息 -->