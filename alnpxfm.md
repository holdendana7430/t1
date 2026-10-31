代发 wailian999

Py:   itertools.permutations(arr)
来源：http://vo.nicolike.cn

PHP:  // 手写递归交换
来源：http://qe.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://ms.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://bg.szxytkj.cn

Java: // 手写回溯递归
来源：http://qi.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://le.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ik.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://dh.yuexingan06.cn

[N09] 栈与队列
来源：http://nk.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pv.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://we.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://av.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hu.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ip.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oi.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cp.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cc.gzmigu.cn

[N10] 链表节点定义
来源：http://xx.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aw.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xl.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lr.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zx.colortex.cn

Java: class Node { int v; Node next; }
来源：http://aa.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pv.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ew.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sq.szsharing.cn

[N11] 二叉树中序遍历
来源：http://ay.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ir.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://cn.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ek.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bs.szxytkj.cn

Java: // 手写递归
来源：http://on.shxzskj.cn

Go:   // 手写递归
来源：http://tg.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hd.huixiangedu.cn

C#:   // 手写递归
来源：http://qb.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xp.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gm.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xq.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ni.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wf.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ek.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gb.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lk.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fy.nicolike.cn

================================================================================
来源：http://lo.szxytkj.cn

O. 并发与异步
来源：http://xi.9csxet.cn

================================================================================
来源：http://wh.hnjuh.cn

[O01] 启动一个线程
来源：http://uk.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gp.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ev.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mj.jianghongdianzi.cn

TS:   // 同 JS
来源：http://fw.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://ff.shtwfgs.cn

Go:   go f()
来源：http://lm.hahajie.cn

Ruby: Thread.new { f }
来源：http://zk.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://ry.nicolike.cn

[O02] 使用线程池
来源：http://ag.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cs.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ho.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://ye.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://uk.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yw.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ib.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mr.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mr.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://tg.newstarts.cn

Py:   with lock: shared += 1
来源：http://zp.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://qi.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ti.shtwfgs.cn

TS:   // 同 JS
来源：http://dr.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://ld.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yd.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qd.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ax.huanxung.cn

[O04] 定义异步函数并等待
来源：http://ty.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://pb.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ce.521024.cn

JS:   async function f() { await g(); }
来源：http://bx.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dk.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oi.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uh.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ui.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://qz.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://ao.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://wh.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kg.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://sk.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://td.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dy.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ua.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://iv.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tt.shxzskj.cn

[O06] 使用进程池
来源：http://kp.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sv.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ku.521024.cn

JS:   // child_process / cluster 模块
来源：http://st.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://nn.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yo.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sl.huixinmuqiang.cn

Ruby: // fork 块
来源：http://si.huanxung.cn

C#:   Parallel.For
来源：http://hj.lnxyls.cn

================================================================================
来源：http://iq.haigaiapp.cn

P. 常用工具函数
来源：http://kg.huanxung.cn

================================================================================
来源：http://ol.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://pk.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://sp.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zq.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://bo.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://bo.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://hw.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://zx.521024.cn

Ruby: SecureRandom.uuid
来源：http://rc.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://iq.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://uq.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ww.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rm.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vz.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qw.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xm.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xy.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ru.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wi.521024.cn

[P03] 生成短随机字符串
来源：http://fc.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gf.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gv.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vl.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xz.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vb.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mu.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://an.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lv.wgjwhj.cn

[P04] 求长度
来源：http://dt.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ic.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vb.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nx.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sb.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://se.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://im.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://xj.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pm.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://lg.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://po.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gv.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://og.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kf.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fh.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://am.lnxyls.cn

Ruby: a == b
来源：http://di.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mg.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://km.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mv.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://bh.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wh.nszjky.cn

TS:   if (x == null) {}
来源：http://vp.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dm.nicolike.cn

Go:   if x == nil {}
来源：http://au.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gn.gzmigu.cn

C#:   if (x is null) {}
来源：http://dc.shtwfgs.cn

[P07] 防抖与节流
来源：http://ds.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://to.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://qt.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oa.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://il.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zb.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kq.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jy.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ba.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://kx.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rz.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xr.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fk.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cl.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ze.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cu.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qg.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ab.colortex.cn

================================================================================
来源：http://ns.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://av.asd995.cn

================================================================================
来源：http://ge.panjiajie.cn

[Q01] 创建表
来源：http://cj.521024.cn

CREATE TABLE users (
来源：http://cz.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://id.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://rp.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://hp.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qh.lnxyls.cn

);
来源：http://cj.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://hf.bookmarksfly.cn

CREATE TABLE orders (
来源：http://mk.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jz.521024.cn

user_id INT NOT NULL,
来源：http://uj.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://bf.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hf.jctech888.com.cn

);
来源：http://re.huixiangedu.cn

[Q03] 增加列
来源：http://es.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lp.nicolike.cn

[Q04] 修改列类型
来源：http://nh.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jianghongdianzi.cn

[Q05] 重命名列
来源：http://ye.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fi.wgjwhj.cn

[Q06] 删除列
来源：http://jc.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oi.muxihuayi.cn

[Q07] 删除表
来源：http://am.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://op.szxytkj.cn

[Q08] 创建普通索引
来源：http://zz.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xu.9csxet.cn

[Q09] 创建唯一索引
来源：http://mu.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nz.muxihuayi.cn

[Q10] 插入单行
来源：http://ys.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ma.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://cb.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://je.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://fm.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cc.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fs.hahajie.cn

[Q13] 忽略重复插入
来源：http://bh.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ax.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://ei.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zd.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cv.yuexingan06.cn

[Q15] 查询全部
来源：http://dj.newstarts.cn

SELECT * FROM users;
来源：http://kw.hnjuh.cn

[Q16] 查询指定列
来源：http://wn.huixiangedu.cn

SELECT id, name FROM users;
来源：http://va.huixiangedu.cn

[Q17] 条件查询
来源：http://dc.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nr.lnxyls.cn

[Q18] 模糊匹配
来源：http://my.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aq.bookmarksfly.cn

[Q19] 范围查询
来源：http://tp.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pk.521024.cn

[Q20] IN 列表
来源：http://rq.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mq.bjjhwx.cn

[Q21] 空值判断
来源：http://ue.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ey.jctech888.com.cn

[Q22] 排序
来源：http://gh.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ay.jctech888.com.cn

[Q23] 分页
来源：http://hd.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fy.jianghongdianzi.cn

[Q24] 去重
来源：http://bx.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://ey.shxzskj.cn

[Q25] 只取前 N 条
来源：http://if.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rg.shxzukj.cn

[Q26] 计数
来源：http://yy.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://ts.hnjuh.cn

[Q27] 条件计数
来源：http://hx.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cx.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://yg.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ly.9csxet.cn

[Q29] 最大最小值
来源：http://em.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yk.panjiajie.cn

[Q30] 分组统计
来源：http://gu.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ot.panjiajie.cn

[Q31] 分组后过滤
来源：http://vn.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ke.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://sz.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mg.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bk.panjiajie.cn

[Q33] 多列分组
来源：http://tk.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sj.newstarts.cn

[Q34] 每组取第一条
来源：http://eh.jianghongdianzi.cn

SELECT * FROM (
来源：http://wh.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ii.newstarts.cn

) t WHERE rn = 1;
来源：http://wh.huanxung.cn

[Q35] 内连接
来源：http://jj.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ky.gzmigu.cn

[Q36] 左连接
来源：http://da.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sj.shxzukj.cn

[Q37] 右连接
来源：http://nc.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://it.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gg.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://br.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://fz.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://io.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://te.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xr.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sh.nicolike.cn

[Q41] 多表连接
来源：http://kq.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tb.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://kk.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://hm.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://xn.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://hw.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://em.shtwfgs.cn

[Q43] 标量子查询
来源：http://ix.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oa.panjiajie.cn

[Q44] IN 子查询
来源：http://di.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://np.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://do.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ho.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ls.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kv.szsharing.cn

[Q47] 与平均值比较
来源：http://vp.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jm.asd995.cn

[Q48] CTE 公用表表达式
来源：http://kc.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jn.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://gd.bookmarksfly.cn

[Q49] 更新单行
来源：http://av.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yp.panjiajie.cn

[Q50] 批量更新
来源：http://ch.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zi.huanxung.cn

[Q51] 用子查询更新
来源：http://tl.huanxung.cn


<!-- 参考信息 -->