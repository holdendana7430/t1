代发 wailian999

Py:   itertools.permutations(arr)
来源：http://uz.lnxyls.cn

PHP:  // 手写递归交换
来源：http://wf.huanxung.cn

JS:   // 手写回溯递归
来源：http://wr.huanxung.cn

TS:   // 手写回溯递归
来源：http://tc.panjiajie.cn

Java: // 手写回溯递归
来源：http://qc.lnxyls.cn

Go:   // 手写回溯递归
来源：http://ks.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://ws.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://ra.wgjwhj.cn

[N09] 栈与队列
来源：http://ba.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dp.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zi.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gu.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wy.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gf.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iu.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pa.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ls.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://no.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jv.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uq.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wd.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jh.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://yk.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mt.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zp.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mw.huanxung.cn

[N11] 二叉树中序遍历
来源：http://hi.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pp.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://ul.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://es.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzmigu.cn

Java: // 手写递归
来源：http://uh.gzmigu.cn

Go:   // 手写递归
来源：http://dt.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hh.lnxyls.cn

C#:   // 手写递归
来源：http://aw.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://el.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lk.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ab.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rh.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cr.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mx.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cg.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://my.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kb.bjjhwx.cn

================================================================================
来源：http://lj.huixinmuqiang.cn

O. 并发与异步
来源：http://cf.yuexingan06.cn

================================================================================
来源：http://py.yuexingan06.cn

[O01] 启动一个线程
来源：http://ds.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ym.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pw.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tx.gzmigu.cn

TS:   // 同 JS
来源：http://yt.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://kh.bjjhwx.cn

Go:   go f()
来源：http://iw.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://rx.521024.cn

C#:   Task.Run(() => F());
来源：http://nl.bjjhwx.cn

[O02] 使用线程池
来源：http://um.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ox.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dt.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://ix.newstarts.cn

TS:   // worker_threads 线程池
来源：http://ll.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xv.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ju.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://en.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gi.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://ar.9csxet.cn

Py:   with lock: shared += 1
来源：http://tc.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://sx.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ia.haigaiapp.cn

TS:   // 同 JS
来源：http://pl.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://ng.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wm.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hf.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://ae.hahajie.cn

[O04] 定义异步函数并等待
来源：http://il.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://qy.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rz.newstarts.cn

JS:   async function f() { await g(); }
来源：http://dz.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zc.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qa.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yd.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kw.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://hs.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://or.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://bc.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cs.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://bg.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://jj.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tr.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ob.szsharing.cn

Ruby: threads.map(&:join)
来源：http://sv.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://de.521024.cn

[O06] 使用进程池
来源：http://tx.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lc.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iw.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://ln.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://tz.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dy.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mf.hnjuh.cn

Ruby: // fork 块
来源：http://uo.bjjhwx.cn

C#:   Parallel.For
来源：http://ll.jctech888.com.cn

================================================================================
来源：http://km.gzmigu.cn

P. 常用工具函数
来源：http://jr.yuntaijiaju.cn

================================================================================
来源：http://tj.muxihuayi.cn

[P01] 生成 UUID
来源：http://eq.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://yd.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pm.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://av.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://iq.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://oq.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://dy.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://et.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://ii.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://wr.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uj.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ih.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iz.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fp.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bb.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gm.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jx.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vu.shxzukj.cn

[P03] 生成短随机字符串
来源：http://uw.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tj.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lo.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yu.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hh.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jx.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hy.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sq.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fe.szxytkj.cn

[P04] 求长度
来源：http://fy.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pi.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pd.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ou.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aa.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://yj.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://no.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://wv.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qq.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://bi.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dr.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rt.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dp.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lj.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fn.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aq.bjjhwx.cn

Ruby: a == b
来源：http://tz.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qt.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mr.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tf.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://ew.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rs.gzmigu.cn

TS:   if (x == null) {}
来源：http://jw.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dm.hnjuh.cn

Go:   if x == nil {}
来源：http://ph.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ow.lnxyls.cn

C#:   if (x is null) {}
来源：http://ud.panjiajie.cn

[P07] 防抖与节流
来源：http://vt.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fi.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://zz.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uy.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xt.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kh.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://by.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rg.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vn.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://jr.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zg.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ae.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xz.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://am.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ng.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xf.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wj.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nr.shxzskj.cn

================================================================================
来源：http://hs.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://su.lnxyls.cn

================================================================================
来源：http://iv.asd995.cn

[Q01] 创建表
来源：http://ik.shxzskj.cn

CREATE TABLE users (
来源：http://aj.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zf.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://xx.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://rx.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://te.hnjuh.cn

);
来源：http://ol.asd995.cn

[Q02] 创建带外键的表
来源：http://lp.shxzukj.cn

CREATE TABLE orders (
来源：http://yi.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ss.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://wb.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://lg.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://et.panjiajie.cn

);
来源：http://ym.jianghongdianzi.cn

[Q03] 增加列
来源：http://ta.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://te.gzmigu.cn

[Q04] 修改列类型
来源：http://wy.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rk.chemitech.net.cn

[Q05] 重命名列
来源：http://bi.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hy.shxzukj.cn

[Q06] 删除列
来源：http://jw.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xl.shtwfgs.cn

[Q07] 删除表
来源：http://hm.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://ma.chemitech.net.cn

[Q08] 创建普通索引
来源：http://ng.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ul.hnjuh.cn

[Q09] 创建唯一索引
来源：http://fg.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fg.nicolike.cn

[Q10] 插入单行
来源：http://ef.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nt.panjiajie.cn

[Q11] 一次插入多行
来源：http://zl.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nk.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://te.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fp.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yv.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://bu.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jl.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://gm.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qq.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pa.shxzskj.cn

[Q15] 查询全部
来源：http://fu.shtwfgs.cn

SELECT * FROM users;
来源：http://ta.shxzukj.cn

[Q16] 查询指定列
来源：http://nx.muxihuayi.cn

SELECT id, name FROM users;
来源：http://xg.hnjuh.cn

[Q17] 条件查询
来源：http://xl.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wi.hnjuh.cn

[Q18] 模糊匹配
来源：http://pa.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ae.shxzskj.cn

[Q19] 范围查询
来源：http://qi.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bf.shxzskj.cn

[Q20] IN 列表
来源：http://is.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cg.lnxyls.cn

[Q21] 空值判断
来源：http://qw.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hm.huixinmuqiang.cn

[Q22] 排序
来源：http://of.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://br.colortex.cn

[Q23] 分页
来源：http://qw.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://be.bjjhwx.cn

[Q24] 去重
来源：http://mq.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://xm.nszjky.cn

[Q25] 只取前 N 条
来源：http://et.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oz.szsharing.cn

[Q26] 计数
来源：http://ru.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://zw.chemitech.net.cn

[Q27] 条件计数
来源：http://hx.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ve.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://qs.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sb.wgjwhj.cn

[Q29] 最大最小值
来源：http://ng.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fk.panjiajie.cn

[Q30] 分组统计
来源：http://gg.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zn.shxzukj.cn

[Q31] 分组后过滤
来源：http://gt.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kz.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://ol.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://od.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xz.szxytkj.cn

[Q33] 多列分组
来源：http://cl.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ur.panjiajie.cn

[Q34] 每组取第一条
来源：http://vw.newstarts.cn

SELECT * FROM (
来源：http://ky.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gc.gzmigu.cn

) t WHERE rn = 1;
来源：http://jg.wgjwhj.cn

[Q35] 内连接
来源：http://bj.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bi.huixinmuqiang.cn

[Q36] 左连接
来源：http://sh.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kr.bookmarksfly.cn

[Q37] 右连接
来源：http://sb.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jc.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jv.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ns.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://zr.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fc.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ah.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://op.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ye.shtwfgs.cn

[Q41] 多表连接
来源：http://aw.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ia.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://fe.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://vi.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://hu.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://uq.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jw.9csxet.cn

[Q43] 标量子查询
来源：http://fd.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ko.yuexingan06.cn

[Q44] IN 子查询
来源：http://bl.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pp.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://sc.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yf.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hv.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xy.hnjuh.cn

[Q47] 与平均值比较
来源：http://pg.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tq.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://tz.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jo.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://lk.bookmarksfly.cn

[Q49] 更新单行
来源：http://ex.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gu.bookmarksfly.cn

[Q50] 批量更新
来源：http://px.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bm.shxzskj.cn

[Q51] 用子查询更新
来源：http://rq.shxzskj.cn


<!-- 参考信息 -->