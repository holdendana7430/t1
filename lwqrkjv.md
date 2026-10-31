代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://st.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gc.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xm.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zs.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ex.bookmarksfly.cn

[N10] 链表节点定义
来源：http://jv.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tq.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ne.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jo.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jk.colortex.cn

Java: class Node { int v; Node next; }
来源：http://ty.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mk.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://si.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zt.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://lf.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rk.9csxet.cn

PHP:  // 手写递归函数
来源：http://no.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pz.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eg.huixinmuqiang.cn

Java: // 手写递归
来源：http://pr.newstarts.cn

Go:   // 手写递归
来源：http://lt.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rv.gzmigu.cn

C#:   // 手写递归
来源：http://ow.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://un.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lg.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mu.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hl.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pc.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kq.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xo.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sr.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sj.wgjwhj.cn

================================================================================
来源：http://lu.muxihuayi.cn

O. 并发与异步
来源：http://xv.nicolike.cn

================================================================================
来源：http://mt.szxytkj.cn

[O01] 启动一个线程
来源：http://fp.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qw.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ov.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ur.hahajie.cn

TS:   // 同 JS
来源：http://fy.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://oa.shxzukj.cn

Go:   go f()
来源：http://mn.hnjuh.cn

Ruby: Thread.new { f }
来源：http://oi.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://qy.szsharing.cn

[O02] 使用线程池
来源：http://ab.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ep.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qd.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://yg.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://me.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ra.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nt.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bk.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jj.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://hu.nszjky.cn

Py:   with lock: shared += 1
来源：http://fw.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://tz.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wk.lnxyls.cn

TS:   // 同 JS
来源：http://si.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://we.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qi.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ek.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://iy.9csxet.cn

[O04] 定义异步函数并等待
来源：http://il.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://uw.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tv.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://in.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vp.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tu.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qg.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ez.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://lt.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://vi.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://yu.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://by.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://zk.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://uo.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eo.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nj.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://ma.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ea.chemitech.net.cn

[O06] 使用进程池
来源：http://zn.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dl.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fp.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://kr.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://gu.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://es.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xa.huixiangedu.cn

Ruby: // fork 块
来源：http://si.hnjuh.cn

C#:   Parallel.For
来源：http://lc.wgjwhj.cn

================================================================================
来源：http://hf.yuntaijiaju.cn

P. 常用工具函数
来源：http://iz.huixinmuqiang.cn

================================================================================
来源：http://qg.newstarts.cn

[P01] 生成 UUID
来源：http://ni.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://ok.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bk.9csxet.cn

JS:   crypto.randomUUID()
来源：http://kb.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://tg.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://vw.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://zy.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://dm.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://hs.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://gx.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nk.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gw.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wi.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kr.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sb.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ho.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qy.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fq.szsharing.cn

[P03] 生成短随机字符串
来源：http://st.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nz.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wf.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://im.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rl.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rc.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ko.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kg.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sv.muxihuayi.cn

[P04] 求长度
来源：http://lx.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://it.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ng.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jh.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://si.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://oz.colortex.cn

Go:   len(arr);  len(m)
来源：http://yr.nszjky.cn

Ruby: x.length;  x.size
来源：http://ln.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qx.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://tw.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zk.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ml.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xq.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hk.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://du.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ux.muxihuayi.cn

Ruby: a == b
来源：http://rf.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ul.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cj.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ww.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://od.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hk.newstarts.cn

TS:   if (x == null) {}
来源：http://be.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ey.521024.cn

Go:   if x == nil {}
来源：http://op.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ss.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://ze.haigaiapp.cn

[P07] 防抖与节流
来源：http://kr.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bo.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://vu.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://en.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jx.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nz.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hw.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bg.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://el.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://pz.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fu.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tr.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zm.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ku.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ak.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qz.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://im.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sz.newstarts.cn

================================================================================
来源：http://fn.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://no.colortex.cn

================================================================================
来源：http://rr.muxihuayi.cn

[Q01] 创建表
来源：http://my.huixinmuqiang.cn

CREATE TABLE users (
来源：http://pj.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rh.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://mt.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://bv.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wy.asd995.cn

);
来源：http://eo.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://kb.hahajie.cn

CREATE TABLE orders (
来源：http://st.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bn.lnxyls.cn

user_id INT NOT NULL,
来源：http://md.nicolike.cn

amount DECIMAL(10, 2),
来源：http://fc.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cz.huixinmuqiang.cn

);
来源：http://bz.nicolike.cn

[Q03] 增加列
来源：http://oh.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kr.9csxet.cn

[Q04] 修改列类型
来源：http://ox.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ux.newstarts.cn

[Q05] 重命名列
来源：http://ua.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eg.yuntaijiaju.cn

[Q06] 删除列
来源：http://en.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lt.panjiajie.cn

[Q07] 删除表
来源：http://pz.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://yq.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://ar.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ae.nicolike.cn

[Q09] 创建唯一索引
来源：http://ot.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fk.huanxung.cn

[Q10] 插入单行
来源：http://zb.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vw.shxzskj.cn

[Q11] 一次插入多行
来源：http://mc.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cs.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://dq.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wd.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zo.lnxyls.cn

[Q13] 忽略重复插入
来源：http://gl.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yo.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://cg.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wb.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wn.yuexingan06.cn

[Q15] 查询全部
来源：http://qg.szxytkj.cn

SELECT * FROM users;
来源：http://xa.yuexingan06.cn

[Q16] 查询指定列
来源：http://jw.szxytkj.cn

SELECT id, name FROM users;
来源：http://ca.colortex.cn

[Q17] 条件查询
来源：http://sg.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://na.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://lu.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ne.wgjwhj.cn

[Q19] 范围查询
来源：http://vo.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jd.szsharing.cn

[Q20] IN 列表
来源：http://ai.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tw.521024.cn

[Q21] 空值判断
来源：http://ju.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kx.wgjwhj.cn

[Q22] 排序
来源：http://yt.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rx.hnjuh.cn

[Q23] 分页
来源：http://dn.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jb.yuntaijiaju.cn

[Q24] 去重
来源：http://nq.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://kr.521024.cn

[Q25] 只取前 N 条
来源：http://ge.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cm.jctech888.com.cn

[Q26] 计数
来源：http://tn.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://zx.jianghongdianzi.cn

[Q27] 条件计数
来源：http://ze.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ts.panjiajie.cn

[Q28] 求和与平均
来源：http://ya.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jl.lnxyls.cn

[Q29] 最大最小值
来源：http://es.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ko.jianghongdianzi.cn

[Q30] 分组统计
来源：http://zx.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ie.nszjky.cn

[Q31] 分组后过滤
来源：http://ly.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vf.521024.cn

[Q32] 分组拼接字符串
来源：http://na.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ii.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vq.yuntaijiaju.cn

[Q33] 多列分组
来源：http://tj.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vp.newstarts.cn

[Q34] 每组取第一条
来源：http://al.muxihuayi.cn

SELECT * FROM (
来源：http://ja.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kc.hahajie.cn

) t WHERE rn = 1;
来源：http://hc.lnxyls.cn

[Q35] 内连接
来源：http://vc.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xb.9csxet.cn

[Q36] 左连接
来源：http://vg.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ze.muxihuayi.cn

[Q37] 右连接
来源：http://hw.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zv.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jz.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gp.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://gn.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ez.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nb.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bn.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ix.bjjhwx.cn

[Q41] 多表连接
来源：http://jz.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gt.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://gg.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://bj.521024.cn

[Q42] 连接条件附加过滤
来源：http://lx.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://zc.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ip.wgjwhj.cn

[Q43] 标量子查询
来源：http://jf.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hp.huanxung.cn

[Q44] IN 子查询
来源：http://je.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rl.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://gm.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qr.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ve.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fp.521024.cn

[Q47] 与平均值比较
来源：http://hf.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jl.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://ac.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xi.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://cc.wgjwhj.cn

[Q49] 更新单行
来源：http://hi.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tp.hnjuh.cn

[Q50] 批量更新
来源：http://th.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rn.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://zy.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kf.shxzukj.cn

[Q52] 删除指定行
来源：http://sa.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://om.nszjky.cn

[Q53] 按条件删除
来源：http://ef.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aq.asd995.cn

[Q54] 清空表
来源：http://id.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://db.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://xl.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fh.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://ew.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vc.panjiajie.cn

[Q57] 行号
来源：http://bv.muxihuayi.cn


<!-- 参考信息 -->