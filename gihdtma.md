代发 wailian999

Py:   itertools.permutations(arr)
来源：http://sa.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://dg.nszjky.cn

JS:   // 手写回溯递归
来源：http://jn.hnjuh.cn

TS:   // 手写回溯递归
来源：http://uc.asd995.cn

Java: // 手写回溯递归
来源：http://zw.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://zh.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ew.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://jq.chemitech.net.cn

[N09] 栈与队列
来源：http://jr.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dt.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ca.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fy.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hu.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kq.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://un.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vl.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pv.lnxyls.cn

[N10] 链表节点定义
来源：http://hk.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yj.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ii.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sq.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gc.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://wo.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://th.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gd.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ka.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://pn.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jy.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://zt.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ms.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://np.colortex.cn

Java: // 手写递归
来源：http://eg.yuntaijiaju.cn

Go:   // 手写递归
来源：http://aj.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ks.lnxyls.cn

C#:   // 手写递归
来源：http://gi.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ih.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pz.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://io.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qy.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pk.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kb.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vx.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bp.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xo.hahajie.cn

================================================================================
来源：http://tt.huanxung.cn

O. 并发与异步
来源：http://qi.bjjhwx.cn

================================================================================
来源：http://fo.chemitech.net.cn

[O01] 启动一个线程
来源：http://jt.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ne.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aq.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kh.hahajie.cn

TS:   // 同 JS
来源：http://aj.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://ss.bjjhwx.cn

Go:   go f()
来源：http://ar.521024.cn

Ruby: Thread.new { f }
来源：http://vx.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://og.shtwfgs.cn

[O02] 使用线程池
来源：http://ek.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nq.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kv.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://ak.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://fg.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fn.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nk.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wj.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ev.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://uz.szsharing.cn

Py:   with lock: shared += 1
来源：http://bv.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://zm.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ez.gzmigu.cn

TS:   // 同 JS
来源：http://rd.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://vx.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wl.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://de.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://wa.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://nt.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://xp.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://po.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://mq.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hk.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bw.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oc.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kc.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://fa.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://nm.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://rh.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hy.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://qg.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://tk.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ku.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wd.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://oi.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jq.asd995.cn

[O06] 使用进程池
来源：http://rd.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://km.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xb.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://gs.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://vg.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ix.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://if.bookmarksfly.cn

Ruby: // fork 块
来源：http://hy.yuntaijiaju.cn

C#:   Parallel.For
来源：http://jd.hahajie.cn

================================================================================
来源：http://rp.newstarts.cn

P. 常用工具函数
来源：http://uy.wgjwhj.cn

================================================================================
来源：http://ou.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://js.colortex.cn

Py:   str(uuid.uuid4())
来源：http://va.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yf.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://lg.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://rn.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://lz.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://bz.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://aq.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://yo.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://ii.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pz.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://og.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zp.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vt.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ne.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vv.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rv.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yh.hnjuh.cn

[P03] 生成短随机字符串
来源：http://kz.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kp.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cy.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uk.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ju.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ei.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xz.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kv.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ut.haigaiapp.cn

[P04] 求长度
来源：http://ml.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ny.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zm.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ep.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ie.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://og.nicolike.cn

Go:   len(arr);  len(m)
来源：http://ks.shxzukj.cn

Ruby: x.length;  x.size
来源：http://ql.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mo.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://xf.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qo.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nw.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fg.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://el.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dw.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zy.colortex.cn

Ruby: a == b
来源：http://vc.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mq.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xj.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ay.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://yg.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fs.szsharing.cn

TS:   if (x == null) {}
来源：http://wh.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mk.9csxet.cn

Go:   if x == nil {}
来源：http://lb.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iv.jctech888.com.cn

C#:   if (x is null) {}
来源：http://jd.szsharing.cn

[P07] 防抖与节流
来源：http://va.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cp.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://uc.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sq.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dc.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fk.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uh.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ob.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xy.huanxung.cn

[P08] 处理浮点精度问题
来源：http://yd.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fv.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cn.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ur.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://me.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xe.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bw.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oa.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://py.bookmarksfly.cn

================================================================================
来源：http://fl.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wx.haigaiapp.cn

================================================================================
来源：http://qf.asd995.cn

[Q01] 创建表
来源：http://jp.panjiajie.cn

CREATE TABLE users (
来源：http://ld.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zz.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://qc.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://vj.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zk.hnjuh.cn

);
来源：http://km.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://vn.shxzskj.cn

CREATE TABLE orders (
来源：http://yt.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vl.yuexingan06.cn

user_id INT NOT NULL,
来源：http://wd.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://al.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dc.bjjhwx.cn

);
来源：http://cb.jianghongdianzi.cn

[Q03] 增加列
来源：http://dl.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fo.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://xu.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yo.huixinmuqiang.cn

[Q05] 重命名列
来源：http://qc.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mi.newstarts.cn

[Q06] 删除列
来源：http://ed.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ex.shxzukj.cn

[Q07] 删除表
来源：http://ys.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://sk.huanxung.cn

[Q08] 创建普通索引
来源：http://hd.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qt.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://ut.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ja.yuexingan06.cn

[Q10] 插入单行
来源：http://yx.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oz.jctech888.com.cn

[Q11] 一次插入多行
来源：http://xu.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hk.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://lt.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ap.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ki.szsharing.cn

[Q13] 忽略重复插入
来源：http://xm.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ex.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://qq.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yh.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rs.nicolike.cn

[Q15] 查询全部
来源：http://di.lnxyls.cn

SELECT * FROM users;
来源：http://ff.haigaiapp.cn

[Q16] 查询指定列
来源：http://aa.lnxyls.cn

SELECT id, name FROM users;
来源：http://kq.nicolike.cn

[Q17] 条件查询
来源：http://am.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://by.chemitech.net.cn

[Q18] 模糊匹配
来源：http://sk.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tk.521024.cn

[Q19] 范围查询
来源：http://qi.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lw.jctech888.com.cn

[Q20] IN 列表
来源：http://pj.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vt.wgjwhj.cn

[Q21] 空值判断
来源：http://ud.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zv.wgjwhj.cn

[Q22] 排序
来源：http://ti.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dv.hnjuh.cn

[Q23] 分页
来源：http://oy.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ux.521024.cn

[Q24] 去重
来源：http://lz.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://uj.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://ej.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bk.colortex.cn

[Q26] 计数
来源：http://wj.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://to.wgjwhj.cn

[Q27] 条件计数
来源：http://ni.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://og.yuexingan06.cn

[Q28] 求和与平均
来源：http://kw.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fw.colortex.cn

[Q29] 最大最小值
来源：http://ck.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kc.hnjuh.cn

[Q30] 分组统计
来源：http://gs.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ae.521024.cn

[Q31] 分组后过滤
来源：http://nn.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://az.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://dq.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mv.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cr.huixiangedu.cn

[Q33] 多列分组
来源：http://pb.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hc.jctech888.com.cn

[Q34] 每组取第一条
来源：http://dk.colortex.cn

SELECT * FROM (
来源：http://zr.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xw.newstarts.cn

) t WHERE rn = 1;
来源：http://dy.nicolike.cn

[Q35] 内连接
来源：http://og.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ka.haigaiapp.cn

[Q36] 左连接
来源：http://bz.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xl.nicolike.cn

[Q37] 右连接
来源：http://lb.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ht.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ci.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aj.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://kh.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ut.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ts.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sv.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hy.shtwfgs.cn

[Q41] 多表连接
来源：http://qt.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mu.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://ns.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://pb.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://kc.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://gl.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bv.shxzskj.cn

[Q43] 标量子查询
来源：http://wl.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rz.szxytkj.cn

[Q44] IN 子查询
来源：http://wt.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kv.521024.cn

[Q45] EXISTS 判断存在
来源：http://ld.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qj.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bz.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gw.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://vd.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ie.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://la.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lt.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://kp.yuntaijiaju.cn

[Q49] 更新单行
来源：http://ay.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sa.haigaiapp.cn

[Q50] 批量更新
来源：http://un.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cr.9csxet.cn

[Q51] 用子查询更新
来源：http://yi.asd995.cn


<!-- 参考信息 -->