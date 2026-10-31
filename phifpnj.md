代发 wailian999

Py:   itertools.permutations(arr)
来源：http://dq.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://la.nszjky.cn

JS:   // 手写回溯递归
来源：http://fw.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://tb.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://nj.lnxyls.cn

Go:   // 手写回溯递归
来源：http://fo.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://kc.panjiajie.cn

C#:   // 手写回溯递归
来源：http://uc.muxihuayi.cn

[N09] 栈与队列
来源：http://ou.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jt.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nc.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ky.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kj.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jb.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kd.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bm.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hg.huanxung.cn

[N10] 链表节点定义
来源：http://va.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qb.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kh.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xv.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rw.colortex.cn

Java: class Node { int v; Node next; }
来源：http://dk.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lv.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hv.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rq.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://yd.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vj.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://ou.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ii.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://md.huanxung.cn

Java: // 手写递归
来源：http://iu.shxzukj.cn

Go:   // 手写递归
来源：http://ks.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://it.hnjuh.cn

C#:   // 手写递归
来源：http://hi.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tj.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://li.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ed.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fv.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://og.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ze.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dc.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lc.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cr.jianghongdianzi.cn

================================================================================
来源：http://xh.nicolike.cn

O. 并发与异步
来源：http://bw.huanxung.cn

================================================================================
来源：http://ao.yuexingan06.cn

[O01] 启动一个线程
来源：http://dp.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yz.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lo.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://te.szsharing.cn

TS:   // 同 JS
来源：http://zv.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://wt.yuntaijiaju.cn

Go:   go f()
来源：http://ln.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://cf.9csxet.cn

C#:   Task.Run(() => F());
来源：http://ni.huixinmuqiang.cn

[O02] 使用线程池
来源：http://fm.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://no.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oe.521024.cn

JS:   // worker_threads 线程池
来源：http://xb.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://sk.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fv.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://im.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yf.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yr.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://lq.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://zf.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://bm.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ny.hahajie.cn

TS:   // 同 JS
来源：http://vn.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://ks.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bd.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oj.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://ol.szsharing.cn

[O04] 定义异步函数并等待
来源：http://hl.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://yx.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://im.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://pp.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jo.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kw.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jn.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ck.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://rk.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://kj.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://em.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ve.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://cb.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://fa.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://it.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mj.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://cx.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fl.nicolike.cn

[O06] 使用进程池
来源：http://uy.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://so.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ly.asd995.cn

JS:   // child_process / cluster 模块
来源：http://dd.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://pm.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kj.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yf.bjjhwx.cn

Ruby: // fork 块
来源：http://xe.newstarts.cn

C#:   Parallel.For
来源：http://ai.shxzskj.cn

================================================================================
来源：http://tg.bjjhwx.cn

P. 常用工具函数
来源：http://jw.gzmigu.cn

================================================================================
来源：http://pz.521024.cn

[P01] 生成 UUID
来源：http://wg.asd995.cn

Py:   str(uuid.uuid4())
来源：http://vt.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ak.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://ak.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://cr.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://ux.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://yj.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://ka.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://wg.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://yz.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sn.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ru.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wj.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ml.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bg.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rn.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://py.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xa.szsharing.cn

[P03] 生成短随机字符串
来源：http://cc.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pw.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://px.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ft.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vn.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xi.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://er.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zn.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vy.bookmarksfly.cn

[P04] 求长度
来源：http://qr.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wj.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oa.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ji.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fm.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://au.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://dp.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://gd.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mx.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://ra.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lj.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hn.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rj.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eh.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lg.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ky.jianghongdianzi.cn

Ruby: a == b
来源：http://fa.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fz.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kn.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jy.521024.cn

PHP:  if (empty($x)) {}
来源：http://hq.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ky.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://kj.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://no.muxihuayi.cn

Go:   if x == nil {}
来源：http://tv.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://er.muxihuayi.cn

C#:   if (x is null) {}
来源：http://jx.shxzukj.cn

[P07] 防抖与节流
来源：http://fe.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mh.asd995.cn

PHP:  // 手写时间戳比较
来源：http://rd.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qh.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rc.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xi.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sg.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dm.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ad.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://wm.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://id.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pc.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://op.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kq.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jx.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xz.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ob.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iz.colortex.cn

================================================================================
来源：http://rw.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cw.shxzukj.cn

================================================================================
来源：http://ae.nicolike.cn

[Q01] 创建表
来源：http://jl.muxihuayi.cn

CREATE TABLE users (
来源：http://gm.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kg.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://gs.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://bj.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hv.lnxyls.cn

);
来源：http://wm.szsharing.cn

[Q02] 创建带外键的表
来源：http://sh.bjjhwx.cn

CREATE TABLE orders (
来源：http://ab.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ak.shtwfgs.cn

user_id INT NOT NULL,
来源：http://jx.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://rw.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bz.shtwfgs.cn

);
来源：http://lv.9csxet.cn

[Q03] 增加列
来源：http://ld.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dv.colortex.cn

[Q04] 修改列类型
来源：http://og.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dh.nszjky.cn

[Q05] 重命名列
来源：http://go.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vs.shxzukj.cn

[Q06] 删除列
来源：http://ku.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ja.jianghongdianzi.cn

[Q07] 删除表
来源：http://jy.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://jh.9csxet.cn

[Q08] 创建普通索引
来源：http://de.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eu.nicolike.cn

[Q09] 创建唯一索引
来源：http://as.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sw.shxzskj.cn

[Q10] 插入单行
来源：http://bo.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ek.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://oh.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gn.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://bg.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tb.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oa.huanxung.cn

[Q13] 忽略重复插入
来源：http://fn.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zp.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://pq.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yh.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iy.bjjhwx.cn

[Q15] 查询全部
来源：http://ol.szxytkj.cn

SELECT * FROM users;
来源：http://ht.wgjwhj.cn

[Q16] 查询指定列
来源：http://oc.bjjhwx.cn

SELECT id, name FROM users;
来源：http://ca.jctech888.com.cn

[Q17] 条件查询
来源：http://hc.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rj.nicolike.cn

[Q18] 模糊匹配
来源：http://dk.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fj.huanxung.cn

[Q19] 范围查询
来源：http://rn.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bk.asd995.cn

[Q20] IN 列表
来源：http://sv.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zv.jctech888.com.cn

[Q21] 空值判断
来源：http://ng.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ex.szxytkj.cn

[Q22] 排序
来源：http://cm.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gu.yuntaijiaju.cn

[Q23] 分页
来源：http://jx.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lx.huanxung.cn

[Q24] 去重
来源：http://gs.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://ew.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://hh.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jx.yuexingan06.cn

[Q26] 计数
来源：http://zs.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://pq.muxihuayi.cn

[Q27] 条件计数
来源：http://jv.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vs.muxihuayi.cn

[Q28] 求和与平均
来源：http://xx.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nq.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://db.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mn.bookmarksfly.cn

[Q30] 分组统计
来源：http://uv.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rg.shxzukj.cn

[Q31] 分组后过滤
来源：http://tj.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mm.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://yn.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hj.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bu.huixiangedu.cn

[Q33] 多列分组
来源：http://ya.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cq.jctech888.com.cn

[Q34] 每组取第一条
来源：http://po.colortex.cn

SELECT * FROM (
来源：http://wq.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nm.9csxet.cn

) t WHERE rn = 1;
来源：http://ou.huixinmuqiang.cn

[Q35] 内连接
来源：http://kx.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://on.huixiangedu.cn

[Q36] 左连接
来源：http://cj.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://po.haigaiapp.cn

[Q37] 右连接
来源：http://ri.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fi.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ww.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dv.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ok.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ii.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://il.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yv.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nj.yuexingan06.cn

[Q41] 多表连接
来源：http://vi.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mb.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://my.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://wz.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://rd.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://ft.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hx.huanxung.cn

[Q43] 标量子查询
来源：http://qe.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uz.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://le.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uf.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://dj.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ar.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bn.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pp.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://en.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nv.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://wl.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://it.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://xg.panjiajie.cn

[Q49] 更新单行
来源：http://hd.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ji.shxzskj.cn

[Q50] 批量更新
来源：http://kx.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://um.jctech888.com.cn

[Q51] 用子查询更新
来源：http://mx.asd995.cn


<!-- 参考信息 -->