代发 wailian999

Go:   // 手写 map[int]int
来源：http://nr.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://yh.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lr.haigaiapp.cn

[N08] 生成全排列
来源：http://bz.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://oa.nszjky.cn

PHP:  // 手写递归交换
来源：http://hj.huanxung.cn

JS:   // 手写回溯递归
来源：http://hk.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://xn.bjjhwx.cn

Java: // 手写回溯递归
来源：http://jt.hahajie.cn

Go:   // 手写回溯递归
来源：http://xq.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://ay.hahajie.cn

C#:   // 手写回溯递归
来源：http://hf.bjjhwx.cn

[N09] 栈与队列
来源：http://px.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wj.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nm.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jc.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jr.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yv.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ql.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uy.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fd.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://bi.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gk.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pd.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kp.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://av.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://rm.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://er.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yq.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hx.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://mw.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ew.huanxung.cn

PHP:  // 手写递归函数
来源：http://wo.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sf.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mu.bjjhwx.cn

Java: // 手写递归
来源：http://ao.hahajie.cn

Go:   // 手写递归
来源：http://tb.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pt.shtwfgs.cn

C#:   // 手写递归
来源：http://tl.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yf.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ky.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rd.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yq.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uj.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yz.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wb.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sm.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ij.yuntaijiaju.cn

================================================================================
来源：http://uh.panjiajie.cn

O. 并发与异步
来源：http://oc.yuntaijiaju.cn

================================================================================
来源：http://ks.nszjky.cn

[O01] 启动一个线程
来源：http://ux.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ir.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xo.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://if.521024.cn

TS:   // 同 JS
来源：http://tz.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://vy.shxzskj.cn

Go:   go f()
来源：http://om.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://dm.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://tu.shtwfgs.cn

[O02] 使用线程池
来源：http://vo.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bv.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fs.asd995.cn

JS:   // worker_threads 线程池
来源：http://xo.521024.cn

TS:   // worker_threads 线程池
来源：http://jq.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qm.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uj.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hd.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jl.521024.cn

[O03] 加锁保护共享数据
来源：http://iy.asd995.cn

Py:   with lock: shared += 1
来源：http://hr.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://em.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tj.shtwfgs.cn

TS:   // 同 JS
来源：http://cn.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://cn.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qd.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://we.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://do.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://qu.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://zm.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hd.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ca.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://da.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bd.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fz.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hd.colortex.cn

C#:   async Task F() { await G(); }
来源：http://jp.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://qb.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://gr.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iv.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://vi.521024.cn

TS:   await Promise.all(tasks)
来源：http://io.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bl.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bp.nszjky.cn

Ruby: threads.map(&:join)
来源：http://zl.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://su.bjjhwx.cn

[O06] 使用进程池
来源：http://pn.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kk.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qg.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://ow.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://uf.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jd.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lg.muxihuayi.cn

Ruby: // fork 块
来源：http://oz.9csxet.cn

C#:   Parallel.For
来源：http://ey.wgjwhj.cn

================================================================================
来源：http://gl.muxihuayi.cn

P. 常用工具函数
来源：http://uw.hahajie.cn

================================================================================
来源：http://xk.huixiangedu.cn

[P01] 生成 UUID
来源：http://ax.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://rx.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ka.521024.cn

JS:   crypto.randomUUID()
来源：http://qh.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://rc.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://al.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://sc.colortex.cn

Ruby: SecureRandom.uuid
来源：http://on.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://sy.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://cw.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gp.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ym.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bm.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://es.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nf.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hv.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ad.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yl.nicolike.cn

[P03] 生成短随机字符串
来源：http://tf.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yq.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kv.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fw.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zs.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kl.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rp.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tj.muxihuayi.cn

[P04] 求长度
来源：http://qo.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zi.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ig.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kc.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wa.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://xo.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://ai.shxzukj.cn

Ruby: x.length;  x.size
来源：http://ei.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cq.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://ef.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ah.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ie.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://te.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dm.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mw.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yw.panjiajie.cn

Ruby: a == b
来源：http://fq.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pn.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wk.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zs.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://jd.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uo.jctech888.com.cn

TS:   if (x == null) {}
来源：http://gv.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jl.huixiangedu.cn

Go:   if x == nil {}
来源：http://pk.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ex.szsharing.cn

C#:   if (x is null) {}
来源：http://ck.shxzskj.cn

[P07] 防抖与节流
来源：http://yx.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ad.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://im.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nt.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dj.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gp.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://it.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://as.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xg.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://lm.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ye.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cx.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lr.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mt.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mx.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xm.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zx.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ym.yuntaijiaju.cn

================================================================================
来源：http://co.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gb.colortex.cn

================================================================================
来源：http://ve.shxzskj.cn

[Q01] 创建表
来源：http://no.asd995.cn

CREATE TABLE users (
来源：http://ed.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yp.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://ek.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://lz.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uk.asd995.cn

);
来源：http://lf.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://lb.panjiajie.cn

CREATE TABLE orders (
来源：http://fz.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ja.nszjky.cn

user_id INT NOT NULL,
来源：http://kl.szsharing.cn

amount DECIMAL(10, 2),
来源：http://pv.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bb.huanxung.cn

);
来源：http://iq.gzmigu.cn

[Q03] 增加列
来源：http://xi.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hr.haigaiapp.cn

[Q04] 修改列类型
来源：http://bn.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://do.huanxung.cn

[Q05] 重命名列
来源：http://cn.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xq.gzmigu.cn

[Q06] 删除列
来源：http://df.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uu.asd995.cn

[Q07] 删除表
来源：http://wt.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://zv.wgjwhj.cn

[Q08] 创建普通索引
来源：http://za.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lp.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://pc.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mg.colortex.cn

[Q10] 插入单行
来源：http://se.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cb.shtwfgs.cn

[Q11] 一次插入多行
来源：http://rw.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xm.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://jc.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cy.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mf.panjiajie.cn

[Q13] 忽略重复插入
来源：http://te.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://we.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://bo.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ci.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qm.colortex.cn

[Q15] 查询全部
来源：http://iw.panjiajie.cn

SELECT * FROM users;
来源：http://qr.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://ry.yuexingan06.cn

SELECT id, name FROM users;
来源：http://ql.wgjwhj.cn

[Q17] 条件查询
来源：http://ol.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vg.nszjky.cn

[Q18] 模糊匹配
来源：http://oj.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oe.haigaiapp.cn

[Q19] 范围查询
来源：http://lq.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hg.asd995.cn

[Q20] IN 列表
来源：http://xf.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fo.nicolike.cn

[Q21] 空值判断
来源：http://jz.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mw.colortex.cn

[Q22] 排序
来源：http://tg.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gr.nszjky.cn

[Q23] 分页
来源：http://cy.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sh.bjjhwx.cn

[Q24] 去重
来源：http://pm.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://pv.shxzukj.cn

[Q25] 只取前 N 条
来源：http://ae.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sn.huixinmuqiang.cn

[Q26] 计数
来源：http://vq.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://ol.jianghongdianzi.cn

[Q27] 条件计数
来源：http://vf.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pq.bjjhwx.cn

[Q28] 求和与平均
来源：http://zu.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mv.hahajie.cn

[Q29] 最大最小值
来源：http://yf.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pr.panjiajie.cn

[Q30] 分组统计
来源：http://wq.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yw.hnjuh.cn

[Q31] 分组后过滤
来源：http://ru.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hf.colortex.cn

[Q32] 分组拼接字符串
来源：http://yi.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://df.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xn.lnxyls.cn

[Q33] 多列分组
来源：http://sa.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nk.huanxung.cn

[Q34] 每组取第一条
来源：http://le.shxzskj.cn

SELECT * FROM (
来源：http://ri.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eo.9csxet.cn

) t WHERE rn = 1;
来源：http://rw.huanxung.cn

[Q35] 内连接
来源：http://lx.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dq.szxytkj.cn

[Q36] 左连接
来源：http://fc.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ut.nszjky.cn

[Q37] 右连接
来源：http://db.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://js.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jb.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://md.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://dr.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sx.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mz.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://si.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oj.yuexingan06.cn

[Q41] 多表连接
来源：http://mh.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uh.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://ub.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://zx.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://lw.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://sx.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ki.shtwfgs.cn

[Q43] 标量子查询
来源：http://fg.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zq.szsharing.cn

[Q44] IN 子查询
来源：http://pn.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bz.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://sq.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mt.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bz.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wk.colortex.cn

[Q47] 与平均值比较
来源：http://dx.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wi.521024.cn

[Q48] CTE 公用表表达式
来源：http://yk.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ak.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://mi.haigaiapp.cn

[Q49] 更新单行
来源：http://pb.nszjky.cn


<!-- 参考信息 -->