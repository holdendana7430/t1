代发 wailian999

Java: // 手写回溯递归
来源：http://fi.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://ek.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://ni.gzmigu.cn

C#:   // 手写回溯递归
来源：http://uc.shtwfgs.cn

[N09] 栈与队列
来源：http://bp.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bq.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gn.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ia.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lb.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tt.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://at.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mj.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ju.panjiajie.cn

[N10] 链表节点定义
来源：http://yf.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dj.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ca.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hi.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mg.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://yz.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lq.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dw.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fx.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://jq.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://od.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://ku.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wt.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ms.muxihuayi.cn

Java: // 手写递归
来源：http://ya.jctech888.com.cn

Go:   // 手写递归
来源：http://pi.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://my.wgjwhj.cn

C#:   // 手写递归
来源：http://lm.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fd.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fw.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yr.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fc.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ge.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://me.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yl.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ap.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ax.gzmigu.cn

================================================================================
来源：http://vn.haigaiapp.cn

O. 并发与异步
来源：http://vb.yuntaijiaju.cn

================================================================================
来源：http://mc.gzmigu.cn

[O01] 启动一个线程
来源：http://yy.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jv.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hb.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://se.newstarts.cn

TS:   // 同 JS
来源：http://pe.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://xg.huanxung.cn

Go:   go f()
来源：http://rc.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://na.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://ek.gzmigu.cn

[O02] 使用线程池
来源：http://pa.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gl.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xq.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://fd.colortex.cn

TS:   // worker_threads 线程池
来源：http://rd.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nc.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://va.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dt.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zu.9csxet.cn

[O03] 加锁保护共享数据
来源：http://fs.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://da.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://tf.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sy.gzmigu.cn

TS:   // 同 JS
来源：http://qt.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://rz.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ld.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sj.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://os.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://sz.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://sy.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mp.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://ud.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://be.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://af.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lx.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lt.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://le.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://kr.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://tr.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mp.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://sn.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://fe.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zf.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fs.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://oy.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xz.yuexingan06.cn

[O06] 使用进程池
来源：http://pl.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oh.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dk.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://wd.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://ag.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://od.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ph.bookmarksfly.cn

Ruby: // fork 块
来源：http://ja.bookmarksfly.cn

C#:   Parallel.For
来源：http://aa.nszjky.cn

================================================================================
来源：http://bb.521024.cn

P. 常用工具函数
来源：http://np.colortex.cn

================================================================================
来源：http://ph.jctech888.com.cn

[P01] 生成 UUID
来源：http://kk.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://nv.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pq.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://lr.9csxet.cn

TS:   crypto.randomUUID()
来源：http://pa.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://dk.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://fl.asd995.cn

Ruby: SecureRandom.uuid
来源：http://kq.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://cb.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://uf.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hu.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zt.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ds.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yn.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ga.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qr.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pb.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gg.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://rq.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wa.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://di.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lz.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ez.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sq.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://et.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kt.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ga.szxytkj.cn

[P04] 求长度
来源：http://ii.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wt.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ji.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yd.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gl.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://bk.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://li.nszjky.cn

Ruby: x.length;  x.size
来源：http://kp.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ef.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://qs.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hd.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vh.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bh.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vc.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wc.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yq.shxzskj.cn

Ruby: a == b
来源：http://wp.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iq.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wy.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wy.521024.cn

PHP:  if (empty($x)) {}
来源：http://nk.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nx.hahajie.cn

TS:   if (x == null) {}
来源：http://zi.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ns.asd995.cn

Go:   if x == nil {}
来源：http://ik.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ce.bjjhwx.cn

C#:   if (x is null) {}
来源：http://dh.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://op.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wk.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://hx.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ra.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ra.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://af.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zf.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qu.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xs.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://jb.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aa.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qb.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yg.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qo.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oo.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ra.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ff.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lg.bjjhwx.cn

================================================================================
来源：http://dr.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rc.gzmigu.cn

================================================================================
来源：http://xu.hnjuh.cn

[Q01] 创建表
来源：http://gf.yuexingan06.cn

CREATE TABLE users (
来源：http://ip.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hm.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://nk.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ob.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ib.wgjwhj.cn

);
来源：http://jt.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://fw.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://vy.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gi.521024.cn

user_id INT NOT NULL,
来源：http://km.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://vm.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fi.muxihuayi.cn

);
来源：http://jg.panjiajie.cn

[Q03] 增加列
来源：http://wz.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ma.szxytkj.cn

[Q04] 修改列类型
来源：http://br.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bs.shxzukj.cn

[Q05] 重命名列
来源：http://au.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ze.bjjhwx.cn

[Q06] 删除列
来源：http://if.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tp.szsharing.cn

[Q07] 删除表
来源：http://sf.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://bb.nszjky.cn

[Q08] 创建普通索引
来源：http://vb.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iw.shxzukj.cn

[Q09] 创建唯一索引
来源：http://xe.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gi.bookmarksfly.cn

[Q10] 插入单行
来源：http://hh.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rs.wgjwhj.cn

[Q11] 一次插入多行
来源：http://td.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://th.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://lr.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sm.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ob.shxzskj.cn

[Q13] 忽略重复插入
来源：http://nt.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hc.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://xd.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jg.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ue.bookmarksfly.cn

[Q15] 查询全部
来源：http://ms.colortex.cn

SELECT * FROM users;
来源：http://vt.colortex.cn

[Q16] 查询指定列
来源：http://ij.panjiajie.cn

SELECT id, name FROM users;
来源：http://vg.wgjwhj.cn

[Q17] 条件查询
来源：http://bj.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sn.bjjhwx.cn

[Q18] 模糊匹配
来源：http://zp.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ge.newstarts.cn

[Q19] 范围查询
来源：http://bi.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kt.jianghongdianzi.cn

[Q20] IN 列表
来源：http://sw.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vp.huanxung.cn

[Q21] 空值判断
来源：http://pq.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ri.huanxung.cn

[Q22] 排序
来源：http://zv.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cv.huixiangedu.cn

[Q23] 分页
来源：http://oj.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hg.nicolike.cn

[Q24] 去重
来源：http://qs.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://pl.nszjky.cn

[Q25] 只取前 N 条
来源：http://ym.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lz.colortex.cn

[Q26] 计数
来源：http://mq.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://gt.yuexingan06.cn

[Q27] 条件计数
来源：http://xd.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yn.jctech888.com.cn

[Q28] 求和与平均
来源：http://nj.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xg.huanxung.cn

[Q29] 最大最小值
来源：http://cx.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bd.yuexingan06.cn

[Q30] 分组统计
来源：http://wd.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://se.huanxung.cn

[Q31] 分组后过滤
来源：http://di.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vt.9csxet.cn

[Q32] 分组拼接字符串
来源：http://ro.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mg.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xy.bjjhwx.cn

[Q33] 多列分组
来源：http://sc.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ea.muxihuayi.cn

[Q34] 每组取第一条
来源：http://td.yuexingan06.cn

SELECT * FROM (
来源：http://zq.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fh.jctech888.com.cn

) t WHERE rn = 1;
来源：http://pq.yuexingan06.cn

[Q35] 内连接
来源：http://au.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jg.szxytkj.cn

[Q36] 左连接
来源：http://tf.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dm.lnxyls.cn

[Q37] 右连接
来源：http://cc.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bw.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kh.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bo.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://dh.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ql.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vb.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fq.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://up.jianghongdianzi.cn

[Q41] 多表连接
来源：http://qj.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rk.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://bh.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://qy.asd995.cn

[Q42] 连接条件附加过滤
来源：http://as.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://vm.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ql.shxzukj.cn

[Q43] 标量子查询
来源：http://aq.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sz.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://bg.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ys.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://cw.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tb.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ov.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rk.muxihuayi.cn

[Q47] 与平均值比较
来源：http://ar.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nd.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://pm.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vt.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://qh.huixinmuqiang.cn

[Q49] 更新单行
来源：http://xu.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qf.panjiajie.cn

[Q50] 批量更新
来源：http://ff.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pa.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://ue.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://us.lnxyls.cn

[Q52] 删除指定行
来源：http://px.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://ep.9csxet.cn

[Q53] 按条件删除
来源：http://ic.nszjky.cn


<!-- 参考信息 -->