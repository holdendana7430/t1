代发 wailian999

Py:   itertools.permutations(arr)
来源：http://kw.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://je.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://aq.newstarts.cn

TS:   // 手写回溯递归
来源：http://ud.lnxyls.cn

Java: // 手写回溯递归
来源：http://kr.asd995.cn

Go:   // 手写回溯递归
来源：http://xu.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://yd.nicolike.cn

C#:   // 手写回溯递归
来源：http://kt.chemitech.net.cn

[N09] 栈与队列
来源：http://ck.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vq.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kt.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zx.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yi.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qa.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fb.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uh.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jt.panjiajie.cn

[N10] 链表节点定义
来源：http://jd.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qy.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://on.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ff.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lj.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://gp.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tc.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wf.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://xw.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jj.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://nu.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xk.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ly.szxytkj.cn

Java: // 手写递归
来源：http://yv.huixiangedu.cn

Go:   // 手写递归
来源：http://ow.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yw.shxzukj.cn

C#:   // 手写递归
来源：http://xt.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://br.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://en.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://te.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ti.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hi.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gz.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yr.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yp.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bg.gzmigu.cn

================================================================================
来源：http://vz.haigaiapp.cn

O. 并发与异步
来源：http://kk.yuexingan06.cn

================================================================================
来源：http://pe.panjiajie.cn

[O01] 启动一个线程
来源：http://dg.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gj.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jg.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rl.shxzukj.cn

TS:   // 同 JS
来源：http://ui.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://kg.szsharing.cn

Go:   go f()
来源：http://bu.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://sb.asd995.cn

C#:   Task.Run(() => F());
来源：http://rc.lnxyls.cn

[O02] 使用线程池
来源：http://mm.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sj.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ks.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://uu.huanxung.cn

TS:   // worker_threads 线程池
来源：http://wf.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eq.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wj.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pk.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qn.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://yu.hahajie.cn

Py:   with lock: shared += 1
来源：http://jq.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ry.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ak.chemitech.net.cn

TS:   // 同 JS
来源：http://by.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://lr.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wt.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wn.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://zx.521024.cn

[O04] 定义异步函数并等待
来源：http://at.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://uy.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ys.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://dr.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zl.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ur.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cx.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ki.521024.cn

C#:   async Task F() { await G(); }
来源：http://ol.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://ce.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://jo.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bb.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://dk.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://wg.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cf.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eu.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://xs.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pj.chemitech.net.cn

[O06] 使用进程池
来源：http://on.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jg.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lc.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://vm.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://cl.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oy.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://go.bjjhwx.cn

Ruby: // fork 块
来源：http://dj.shtwfgs.cn

C#:   Parallel.For
来源：http://hk.colortex.cn

================================================================================
来源：http://ae.colortex.cn

P. 常用工具函数
来源：http://pc.521024.cn

================================================================================
来源：http://tw.huanxung.cn

[P01] 生成 UUID
来源：http://nt.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://yl.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://li.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://kg.nszjky.cn

TS:   crypto.randomUUID()
来源：http://am.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://ob.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://ig.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://gw.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://jr.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://zq.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hn.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hr.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qv.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kx.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xa.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vd.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://di.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iu.newstarts.cn

[P03] 生成短随机字符串
来源：http://wd.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eu.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qu.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://te.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jv.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vr.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eb.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bk.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://af.huixiangedu.cn

[P04] 求长度
来源：http://ji.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ao.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bg.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lj.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vx.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://qj.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://fl.newstarts.cn

Ruby: x.length;  x.size
来源：http://ni.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://to.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://ih.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fy.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gp.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ou.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pi.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mi.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hf.lnxyls.cn

Ruby: a == b
来源：http://ee.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://es.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fc.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jm.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://bv.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lr.huanxung.cn

TS:   if (x == null) {}
来源：http://pw.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fb.bjjhwx.cn

Go:   if x == nil {}
来源：http://mt.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qd.muxihuayi.cn

C#:   if (x is null) {}
来源：http://tb.asd995.cn

[P07] 防抖与节流
来源：http://ac.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uu.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://ys.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sy.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rv.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ow.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wq.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ch.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jk.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://iw.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zr.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gp.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bu.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bq.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ms.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gp.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pk.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vv.gzmigu.cn

================================================================================
来源：http://tn.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rv.nszjky.cn

================================================================================
来源：http://cf.haigaiapp.cn

[Q01] 创建表
来源：http://cg.bjjhwx.cn

CREATE TABLE users (
来源：http://ef.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pf.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://yd.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://th.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rs.nszjky.cn

);
来源：http://mf.9csxet.cn

[Q02] 创建带外键的表
来源：http://ha.9csxet.cn

CREATE TABLE orders (
来源：http://en.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://io.hahajie.cn

user_id INT NOT NULL,
来源：http://kp.asd995.cn

amount DECIMAL(10, 2),
来源：http://yi.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bf.hnjuh.cn

);
来源：http://lx.yuexingan06.cn

[Q03] 增加列
来源：http://oe.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vf.bjjhwx.cn

[Q04] 修改列类型
来源：http://sy.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bw.chemitech.net.cn

[Q05] 重命名列
来源：http://wx.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ra.huixiangedu.cn

[Q06] 删除列
来源：http://zh.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uy.jctech888.com.cn

[Q07] 删除表
来源：http://wz.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://rc.panjiajie.cn

[Q08] 创建普通索引
来源：http://xm.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bb.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://hz.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ca.9csxet.cn

[Q10] 插入单行
来源：http://ve.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ds.huanxung.cn

[Q11] 一次插入多行
来源：http://ov.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://to.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://jg.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kg.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://en.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://kz.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://os.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://dt.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jk.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://av.hahajie.cn

[Q15] 查询全部
来源：http://zk.9csxet.cn

SELECT * FROM users;
来源：http://th.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://uk.panjiajie.cn

SELECT id, name FROM users;
来源：http://ro.hnjuh.cn

[Q17] 条件查询
来源：http://xn.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zo.jctech888.com.cn

[Q18] 模糊匹配
来源：http://vk.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wg.szxytkj.cn

[Q19] 范围查询
来源：http://eq.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zh.huixiangedu.cn

[Q20] IN 列表
来源：http://ns.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://el.nicolike.cn

[Q21] 空值判断
来源：http://bc.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ho.shxzskj.cn

[Q22] 排序
来源：http://xd.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bd.huixiangedu.cn

[Q23] 分页
来源：http://jx.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lt.bjjhwx.cn

[Q24] 去重
来源：http://th.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://mm.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://le.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wg.shxzskj.cn

[Q26] 计数
来源：http://df.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://cy.asd995.cn

[Q27] 条件计数
来源：http://ny.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zp.shxzskj.cn

[Q28] 求和与平均
来源：http://dk.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zm.szxytkj.cn

[Q29] 最大最小值
来源：http://az.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://te.newstarts.cn

[Q30] 分组统计
来源：http://vk.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yg.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://ip.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rp.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://ie.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qu.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yj.9csxet.cn

[Q33] 多列分组
来源：http://us.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ye.muxihuayi.cn

[Q34] 每组取第一条
来源：http://zd.bookmarksfly.cn

SELECT * FROM (
来源：http://ml.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eu.shtwfgs.cn

) t WHERE rn = 1;
来源：http://sp.yuexingan06.cn

[Q35] 内连接
来源：http://bx.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bl.chemitech.net.cn

[Q36] 左连接
来源：http://ih.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://be.huixinmuqiang.cn

[Q37] 右连接
来源：http://pv.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mg.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iz.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://to.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://nq.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pv.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wt.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mq.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iw.9csxet.cn

[Q41] 多表连接
来源：http://uc.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pa.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ha.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://yg.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://yw.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://fe.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dc.szsharing.cn

[Q43] 标量子查询
来源：http://ll.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fs.shtwfgs.cn

[Q44] IN 子查询
来源：http://fn.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aw.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://ll.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hg.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uw.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sr.yuexingan06.cn

[Q47] 与平均值比较
来源：http://dq.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ra.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://pq.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wo.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://gl.shxzukj.cn

[Q49] 更新单行
来源：http://ht.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pa.szxytkj.cn

[Q50] 批量更新
来源：http://so.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ct.shtwfgs.cn

[Q51] 用子查询更新
来源：http://ik.newstarts.cn


<!-- 参考信息 -->