代发 wailian999

[N09] 栈与队列
来源：http://cw.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://db.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yo.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cq.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://si.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qe.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jz.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://us.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uw.haigaiapp.cn

[N10] 链表节点定义
来源：http://lc.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cw.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ee.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zl.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://at.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://hy.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ao.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kc.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sw.newstarts.cn

[N11] 二叉树中序遍历
来源：http://uj.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xh.shxzskj.cn

PHP:  // 手写递归函数
来源：http://ax.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tm.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hl.asd995.cn

Java: // 手写递归
来源：http://nq.asd995.cn

Go:   // 手写递归
来源：http://ic.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ej.shxzskj.cn

C#:   // 手写递归
来源：http://kf.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gf.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qr.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sf.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://az.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://by.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nf.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ak.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eb.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lb.chemitech.net.cn

================================================================================
来源：http://eo.huixiangedu.cn

O. 并发与异步
来源：http://mp.shxzskj.cn

================================================================================
来源：http://bs.shxzukj.cn

[O01] 启动一个线程
来源：http://yw.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uw.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lg.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ye.muxihuayi.cn

TS:   // 同 JS
来源：http://uc.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://rp.nicolike.cn

Go:   go f()
来源：http://fs.hnjuh.cn

Ruby: Thread.new { f }
来源：http://yc.hahajie.cn

C#:   Task.Run(() => F());
来源：http://mq.yuexingan06.cn

[O02] 使用线程池
来源：http://mm.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dz.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ix.newstarts.cn

JS:   // worker_threads 线程池
来源：http://qf.hahajie.cn

TS:   // worker_threads 线程池
来源：http://yt.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wr.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lm.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ev.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pc.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://yy.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://wl.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://wc.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ya.haigaiapp.cn

TS:   // 同 JS
来源：http://yp.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://bc.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sz.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lh.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://gg.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://uf.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://bz.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rf.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://pc.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rb.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ub.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hd.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tu.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://lx.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://pk.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://my.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sd.asd995.cn

JS:   await Promise.all(tasks)
来源：http://js.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://ri.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tc.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://el.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://cb.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ah.newstarts.cn

[O06] 使用进程池
来源：http://xq.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qr.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rh.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://nk.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://sc.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sw.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mi.bjjhwx.cn

Ruby: // fork 块
来源：http://dn.jctech888.com.cn

C#:   Parallel.For
来源：http://pd.shxzskj.cn

================================================================================
来源：http://cw.chemitech.net.cn

P. 常用工具函数
来源：http://vm.shxzskj.cn

================================================================================
来源：http://hp.huanxung.cn

[P01] 生成 UUID
来源：http://nr.asd995.cn

Py:   str(uuid.uuid4())
来源：http://tw.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zj.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://zv.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://we.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://pj.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://er.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://ln.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://zg.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://ix.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wu.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xj.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wa.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://au.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iv.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dr.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ar.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bn.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://zb.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gb.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mf.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jd.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ka.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cj.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lc.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kb.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qy.shxzukj.cn

[P04] 求长度
来源：http://zc.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://va.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gh.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ks.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ck.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://md.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://oa.hnjuh.cn

Ruby: x.length;  x.size
来源：http://nt.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://di.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://lr.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bq.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xw.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rd.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jo.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gz.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jm.nicolike.cn

Ruby: a == b
来源：http://hv.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yf.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bj.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gx.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://cn.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ct.huixiangedu.cn

TS:   if (x == null) {}
来源：http://zj.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hr.gzmigu.cn

Go:   if x == nil {}
来源：http://if.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://px.huixiangedu.cn

C#:   if (x is null) {}
来源：http://nz.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://la.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ba.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://ia.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://la.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kp.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zq.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ip.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gc.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hc.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://ms.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ey.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ri.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iy.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pj.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cb.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oi.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ye.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://le.muxihuayi.cn

================================================================================
来源：http://lu.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yo.shxzskj.cn

================================================================================
来源：http://zw.jctech888.com.cn

[Q01] 创建表
来源：http://os.chemitech.net.cn

CREATE TABLE users (
来源：http://qs.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zn.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://pe.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://ho.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://to.9csxet.cn

);
来源：http://cs.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://wr.jctech888.com.cn

CREATE TABLE orders (
来源：http://ts.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fv.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://rx.colortex.cn

amount DECIMAL(10, 2),
来源：http://qk.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://li.bookmarksfly.cn

);
来源：http://ux.shtwfgs.cn

[Q03] 增加列
来源：http://ob.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ff.lnxyls.cn

[Q04] 修改列类型
来源：http://hl.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://av.haigaiapp.cn

[Q05] 重命名列
来源：http://xq.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sn.9csxet.cn

[Q06] 删除列
来源：http://uq.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jd.haigaiapp.cn

[Q07] 删除表
来源：http://ji.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://jn.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://ul.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xy.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://vn.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://km.szsharing.cn

[Q10] 插入单行
来源：http://ro.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oi.9csxet.cn

[Q11] 一次插入多行
来源：http://qq.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dm.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://vl.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pz.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://al.szsharing.cn

[Q13] 忽略重复插入
来源：http://qp.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bt.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://if.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ez.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ai.lnxyls.cn

[Q15] 查询全部
来源：http://ph.bjjhwx.cn

SELECT * FROM users;
来源：http://qz.9csxet.cn

[Q16] 查询指定列
来源：http://ht.huixiangedu.cn

SELECT id, name FROM users;
来源：http://yi.lnxyls.cn

[Q17] 条件查询
来源：http://se.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pe.haigaiapp.cn

[Q18] 模糊匹配
来源：http://lt.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eu.jctech888.com.cn

[Q19] 范围查询
来源：http://ld.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mz.szsharing.cn

[Q20] IN 列表
来源：http://ng.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yg.shtwfgs.cn

[Q21] 空值判断
来源：http://jj.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dn.shtwfgs.cn

[Q22] 排序
来源：http://hc.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wf.szxytkj.cn

[Q23] 分页
来源：http://tu.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bj.chemitech.net.cn

[Q24] 去重
来源：http://dx.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://eh.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://wt.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ho.jctech888.com.cn

[Q26] 计数
来源：http://xk.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://jf.9csxet.cn

[Q27] 条件计数
来源：http://dc.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jv.huixiangedu.cn

[Q28] 求和与平均
来源：http://od.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xd.colortex.cn

[Q29] 最大最小值
来源：http://pk.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jo.521024.cn

[Q30] 分组统计
来源：http://nk.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dt.asd995.cn

[Q31] 分组后过滤
来源：http://gt.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ia.asd995.cn

[Q32] 分组拼接字符串
来源：http://oi.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nl.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oq.newstarts.cn

[Q33] 多列分组
来源：http://mj.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lv.hnjuh.cn

[Q34] 每组取第一条
来源：http://sb.hnjuh.cn

SELECT * FROM (
来源：http://ae.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://by.bjjhwx.cn

) t WHERE rn = 1;
来源：http://ky.lnxyls.cn

[Q35] 内连接
来源：http://wi.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jf.newstarts.cn

[Q36] 左连接
来源：http://yx.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qq.shtwfgs.cn

[Q37] 右连接
来源：http://gi.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cb.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ui.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xm.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ty.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lt.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://st.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jt.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jw.chemitech.net.cn

[Q41] 多表连接
来源：http://st.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tz.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://my.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://rs.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://ec.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://kk.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://po.shxzskj.cn

[Q43] 标量子查询
来源：http://ok.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kj.9csxet.cn

[Q44] IN 子查询
来源：http://zo.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://br.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://eb.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eb.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://id.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mc.lnxyls.cn

[Q47] 与平均值比较
来源：http://ms.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mf.521024.cn

[Q48] CTE 公用表表达式
来源：http://qb.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xj.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://xo.gzmigu.cn

[Q49] 更新单行
来源：http://za.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ai.huanxung.cn

[Q50] 批量更新
来源：http://af.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ln.nicolike.cn

[Q51] 用子查询更新
来源：http://ya.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kz.nszjky.cn

[Q52] 删除指定行
来源：http://mg.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://ax.szsharing.cn

[Q53] 按条件删除
来源：http://mu.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fs.huixinmuqiang.cn

[Q54] 清空表
来源：http://wk.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://pd.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://rb.panjiajie.cn


<!-- 参考信息 -->