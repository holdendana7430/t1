代发 wailian999

Java: // 手写回溯递归
来源：http://fy.huanxung.cn

Go:   // 手写回溯递归
来源：http://fk.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://gd.szxytkj.cn

C#:   // 手写回溯递归
来源：http://pe.yuexingan06.cn

[N09] 栈与队列
来源：http://ty.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wv.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dg.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gk.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fq.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rl.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sb.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yc.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dj.panjiajie.cn

[N10] 链表节点定义
来源：http://ff.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zm.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gm.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ic.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sv.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://iu.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rt.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mm.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ed.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://gc.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ld.panjiajie.cn

PHP:  // 手写递归函数
来源：http://pf.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wh.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uf.huixinmuqiang.cn

Java: // 手写递归
来源：http://de.bookmarksfly.cn

Go:   // 手写递归
来源：http://qv.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sp.newstarts.cn

C#:   // 手写递归
来源：http://oh.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iy.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hi.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sc.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bx.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sg.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lo.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://to.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ph.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bj.wgjwhj.cn

================================================================================
来源：http://in.lnxyls.cn

O. 并发与异步
来源：http://lt.hahajie.cn

================================================================================
来源：http://jl.shxzskj.cn

[O01] 启动一个线程
来源：http://jh.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qe.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yz.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ks.shxzskj.cn

TS:   // 同 JS
来源：http://go.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ks.asd995.cn

Go:   go f()
来源：http://pf.nszjky.cn

Ruby: Thread.new { f }
来源：http://qa.nszjky.cn

C#:   Task.Run(() => F());
来源：http://dn.yuntaijiaju.cn

[O02] 使用线程池
来源：http://gs.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zo.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wl.nszjky.cn

JS:   // worker_threads 线程池
来源：http://yj.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://cv.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fr.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yz.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oc.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hk.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://ux.9csxet.cn

Py:   with lock: shared += 1
来源：http://vf.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://bj.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zy.shxzskj.cn

TS:   // 同 JS
来源：http://bq.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://pe.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fs.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xb.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://tx.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://ym.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://dj.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xd.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://yj.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ak.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zl.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wf.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hw.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://rg.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://qf.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://yq.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nr.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://my.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://kh.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://at.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wb.colortex.cn

Ruby: threads.map(&:join)
来源：http://vj.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pu.huanxung.cn

[O06] 使用进程池
来源：http://ss.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jw.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mz.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://nb.521024.cn

TS:   // child_process / cluster 模块
来源：http://ym.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jn.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rh.bookmarksfly.cn

Ruby: // fork 块
来源：http://gc.shtwfgs.cn

C#:   Parallel.For
来源：http://vf.9csxet.cn

================================================================================
来源：http://wg.huixinmuqiang.cn

P. 常用工具函数
来源：http://bf.9csxet.cn

================================================================================
来源：http://df.hnjuh.cn

[P01] 生成 UUID
来源：http://px.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://jq.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uz.nicolike.cn

JS:   crypto.randomUUID()
来源：http://ua.nszjky.cn

TS:   crypto.randomUUID()
来源：http://xh.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://kf.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://fu.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://uo.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://yq.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://ao.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nn.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rq.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://it.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kf.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qg.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cl.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ae.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jt.szsharing.cn

[P03] 生成短随机字符串
来源：http://my.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xb.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zi.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wm.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sd.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sz.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cv.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sy.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fm.haigaiapp.cn

[P04] 求长度
来源：http://yi.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aj.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iq.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://to.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yz.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://wp.szsharing.cn

Go:   len(arr);  len(m)
来源：http://pf.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://ta.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pn.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://nu.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ae.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bf.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://we.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eb.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ai.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rd.jctech888.com.cn

Ruby: a == b
来源：http://im.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zq.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ke.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xs.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://oy.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fl.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://dh.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pj.hahajie.cn

Go:   if x == nil {}
来源：http://kp.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tp.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://we.szsharing.cn

[P07] 防抖与节流
来源：http://vh.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sw.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://pu.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ul.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bc.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ql.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ea.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oa.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nc.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://di.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tc.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ho.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ts.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hj.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xw.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zu.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sa.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ht.jianghongdianzi.cn

================================================================================
来源：http://aj.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wb.asd995.cn

================================================================================
来源：http://ju.hnjuh.cn

[Q01] 创建表
来源：http://kj.gzmigu.cn

CREATE TABLE users (
来源：http://sp.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ol.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://qa.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://co.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hg.shxzukj.cn

);
来源：http://eu.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://oa.521024.cn

CREATE TABLE orders (
来源：http://sd.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kz.jctech888.com.cn

user_id INT NOT NULL,
来源：http://lz.huanxung.cn

amount DECIMAL(10, 2),
来源：http://rl.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pw.colortex.cn

);
来源：http://ir.szsharing.cn

[Q03] 增加列
来源：http://ok.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lk.panjiajie.cn

[Q04] 修改列类型
来源：http://ny.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qe.shxzskj.cn

[Q05] 重命名列
来源：http://lc.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gv.shxzukj.cn

[Q06] 删除列
来源：http://xd.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xn.jianghongdianzi.cn

[Q07] 删除表
来源：http://uy.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://xj.nicolike.cn

[Q08] 创建普通索引
来源：http://wr.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fz.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://ku.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rx.szxytkj.cn

[Q10] 插入单行
来源：http://hj.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wx.jctech888.com.cn

[Q11] 一次插入多行
来源：http://fm.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wf.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://gj.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gu.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://il.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://xs.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tl.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://ri.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ka.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bs.yuntaijiaju.cn

[Q15] 查询全部
来源：http://qi.chemitech.net.cn

SELECT * FROM users;
来源：http://vy.chemitech.net.cn

[Q16] 查询指定列
来源：http://xb.gzmigu.cn

SELECT id, name FROM users;
来源：http://ch.yuexingan06.cn

[Q17] 条件查询
来源：http://ev.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tw.asd995.cn

[Q18] 模糊匹配
来源：http://ci.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vr.shxzskj.cn

[Q19] 范围查询
来源：http://dz.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jk.huanxung.cn

[Q20] IN 列表
来源：http://bj.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ok.gzmigu.cn

[Q21] 空值判断
来源：http://mm.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bd.shxzskj.cn

[Q22] 排序
来源：http://mj.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sl.9csxet.cn

[Q23] 分页
来源：http://kj.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cf.nszjky.cn

[Q24] 去重
来源：http://vm.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://in.colortex.cn

[Q25] 只取前 N 条
来源：http://vl.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jo.colortex.cn

[Q26] 计数
来源：http://kq.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://ed.huixiangedu.cn

[Q27] 条件计数
来源：http://tc.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mu.huanxung.cn

[Q28] 求和与平均
来源：http://ve.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ve.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://vs.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cf.shxzukj.cn

[Q30] 分组统计
来源：http://pu.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fu.chemitech.net.cn

[Q31] 分组后过滤
来源：http://kv.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ra.9csxet.cn

[Q32] 分组拼接字符串
来源：http://rq.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nt.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tp.nszjky.cn

[Q33] 多列分组
来源：http://tl.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cp.shxzukj.cn

[Q34] 每组取第一条
来源：http://pa.muxihuayi.cn

SELECT * FROM (
来源：http://kg.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lu.szxytkj.cn

) t WHERE rn = 1;
来源：http://vr.hnjuh.cn

[Q35] 内连接
来源：http://tt.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yw.nszjky.cn

[Q36] 左连接
来源：http://ez.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dz.chemitech.net.cn

[Q37] 右连接
来源：http://oh.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kw.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tq.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ls.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://pl.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://li.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pv.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ut.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qx.szsharing.cn

[Q41] 多表连接
来源：http://gk.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uz.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://gi.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://zl.521024.cn

[Q42] 连接条件附加过滤
来源：http://vp.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://dw.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sf.newstarts.cn

[Q43] 标量子查询
来源：http://wv.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ww.shxzukj.cn

[Q44] IN 子查询
来源：http://qb.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nb.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://yb.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://le.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lz.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tm.huixiangedu.cn

[Q47] 与平均值比较
来源：http://dv.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jw.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://nj.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fu.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://lr.haigaiapp.cn

[Q49] 更新单行
来源：http://fk.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xs.bjjhwx.cn

[Q50] 批量更新
来源：http://ug.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hl.yuexingan06.cn

[Q51] 用子查询更新
来源：http://ez.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sx.szsharing.cn

[Q52] 删除指定行
来源：http://yx.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://ff.huanxung.cn

[Q53] 按条件删除
来源：http://qo.shxzukj.cn


<!-- 参考信息 -->