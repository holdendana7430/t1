代发 wailian999

Go:   // 手写 map[int]int
来源：http://kj.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://ve.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lj.asd995.cn

[N08] 生成全排列
来源：http://nq.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://xs.nszjky.cn

PHP:  // 手写递归交换
来源：http://zh.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://bw.newstarts.cn

TS:   // 手写回溯递归
来源：http://xx.shxzskj.cn

Java: // 手写回溯递归
来源：http://cm.lnxyls.cn

Go:   // 手写回溯递归
来源：http://jb.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://up.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://rk.bjjhwx.cn

[N09] 栈与队列
来源：http://yt.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cq.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wh.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eb.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dg.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qn.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fd.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hv.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ly.lnxyls.cn

[N10] 链表节点定义
来源：http://wu.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ge.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ds.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://it.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://li.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://jm.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://av.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zg.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aw.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://pp.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bi.newstarts.cn

PHP:  // 手写递归函数
来源：http://tb.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vy.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ga.asd995.cn

Java: // 手写递归
来源：http://cl.huanxung.cn

Go:   // 手写递归
来源：http://ok.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jw.colortex.cn

C#:   // 手写递归
来源：http://ux.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ps.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://do.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://od.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fl.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://il.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dh.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oo.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oj.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xe.bookmarksfly.cn

================================================================================
来源：http://bl.nszjky.cn

O. 并发与异步
来源：http://ep.shxzskj.cn

================================================================================
来源：http://au.chemitech.net.cn

[O01] 启动一个线程
来源：http://ux.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sg.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xd.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jn.huanxung.cn

TS:   // 同 JS
来源：http://xh.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://xj.bookmarksfly.cn

Go:   go f()
来源：http://ok.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://ec.szsharing.cn

C#:   Task.Run(() => F());
来源：http://eb.gzmigu.cn

[O02] 使用线程池
来源：http://hq.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yb.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bb.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://rh.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://sw.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jo.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kr.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pr.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ex.hahajie.cn

[O03] 加锁保护共享数据
来源：http://rp.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://fg.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://zy.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nn.wgjwhj.cn

TS:   // 同 JS
来源：http://kg.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://tm.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://im.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ik.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://zr.9csxet.cn

[O04] 定义异步函数并等待
来源：http://ns.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://nz.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rr.newstarts.cn

JS:   async function f() { await g(); }
来源：http://db.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bm.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vj.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fy.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://df.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://xo.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://ul.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://lh.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xc.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://ef.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://gg.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sp.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zm.hahajie.cn

Ruby: threads.map(&:join)
来源：http://gm.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xy.wgjwhj.cn

[O06] 使用进程池
来源：http://km.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ps.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://or.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://at.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://qg.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rq.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://en.hnjuh.cn

Ruby: // fork 块
来源：http://yg.huixiangedu.cn

C#:   Parallel.For
来源：http://xy.panjiajie.cn

================================================================================
来源：http://pb.bookmarksfly.cn

P. 常用工具函数
来源：http://ne.hahajie.cn

================================================================================
来源：http://nq.huanxung.cn

[P01] 生成 UUID
来源：http://hd.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://yy.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yt.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://ul.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://av.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://fm.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://do.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://hs.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://qv.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://nu.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jq.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aa.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iq.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ac.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hb.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jd.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vk.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://si.colortex.cn

[P03] 生成短随机字符串
来源：http://ss.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iq.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ey.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ck.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ja.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cb.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://di.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vu.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jw.shxzskj.cn

[P04] 求长度
来源：http://un.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yh.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eh.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://je.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://le.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://pj.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://fh.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://zi.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gv.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://or.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://up.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ts.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wc.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aq.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ml.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nq.huixiangedu.cn

Ruby: a == b
来源：http://cy.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ko.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ah.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cd.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://be.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hr.asd995.cn

TS:   if (x == null) {}
来源：http://ad.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ul.lnxyls.cn

Go:   if x == nil {}
来源：http://ez.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pf.asd995.cn

C#:   if (x is null) {}
来源：http://aj.szsharing.cn

[P07] 防抖与节流
来源：http://oa.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ji.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://cd.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ts.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nl.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://om.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dr.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cf.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ib.newstarts.cn

[P08] 处理浮点精度问题
来源：http://bc.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fd.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://io.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vn.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xo.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wl.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tu.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ps.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ez.shxzukj.cn

================================================================================
来源：http://cn.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bl.wgjwhj.cn

================================================================================
来源：http://sz.hahajie.cn

[Q01] 创建表
来源：http://kn.gzmigu.cn

CREATE TABLE users (
来源：http://ph.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sw.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://gv.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://fz.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hm.nicolike.cn

);
来源：http://gn.newstarts.cn

[Q02] 创建带外键的表
来源：http://tl.nicolike.cn

CREATE TABLE orders (
来源：http://bf.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jj.huanxung.cn

user_id INT NOT NULL,
来源：http://sz.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://xp.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kk.newstarts.cn

);
来源：http://vy.shxzukj.cn

[Q03] 增加列
来源：http://in.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tf.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://lr.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bz.newstarts.cn

[Q05] 重命名列
来源：http://hb.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dt.jctech888.com.cn

[Q06] 删除列
来源：http://fb.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://av.newstarts.cn

[Q07] 删除表
来源：http://xx.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://bu.lnxyls.cn

[Q08] 创建普通索引
来源：http://ru.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sj.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://le.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dv.jctech888.com.cn

[Q10] 插入单行
来源：http://hs.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://de.asd995.cn

[Q11] 一次插入多行
来源：http://uq.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ep.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://nw.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gj.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uj.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://kd.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ah.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://ak.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rj.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://li.shxzukj.cn

[Q15] 查询全部
来源：http://er.chemitech.net.cn

SELECT * FROM users;
来源：http://zl.haigaiapp.cn

[Q16] 查询指定列
来源：http://lq.muxihuayi.cn

SELECT id, name FROM users;
来源：http://ez.szsharing.cn

[Q17] 条件查询
来源：http://dm.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ja.jctech888.com.cn

[Q18] 模糊匹配
来源：http://dd.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wc.hnjuh.cn

[Q19] 范围查询
来源：http://vy.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://un.huanxung.cn

[Q20] IN 列表
来源：http://ad.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mb.yuexingan06.cn

[Q21] 空值判断
来源：http://dn.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zl.haigaiapp.cn

[Q22] 排序
来源：http://sx.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tv.jctech888.com.cn

[Q23] 分页
来源：http://lm.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dz.jctech888.com.cn

[Q24] 去重
来源：http://dz.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://ag.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://wo.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ba.wgjwhj.cn

[Q26] 计数
来源：http://bp.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://yr.hahajie.cn

[Q27] 条件计数
来源：http://zo.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rr.huixiangedu.cn

[Q28] 求和与平均
来源：http://jj.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hr.asd995.cn

[Q29] 最大最小值
来源：http://yn.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xm.hahajie.cn

[Q30] 分组统计
来源：http://ym.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ke.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://bu.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fk.521024.cn

[Q32] 分组拼接字符串
来源：http://nn.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ag.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gq.shxzskj.cn

[Q33] 多列分组
来源：http://bc.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cl.shxzukj.cn

[Q34] 每组取第一条
来源：http://qg.panjiajie.cn

SELECT * FROM (
来源：http://yt.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iw.newstarts.cn

) t WHERE rn = 1;
来源：http://rb.chemitech.net.cn

[Q35] 内连接
来源：http://jr.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mc.nszjky.cn

[Q36] 左连接
来源：http://ep.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qw.nicolike.cn

[Q37] 右连接
来源：http://dz.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bz.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fy.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hu.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://ct.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://np.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kh.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ef.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tq.yuntaijiaju.cn

[Q41] 多表连接
来源：http://yd.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://px.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://ae.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://xg.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://ej.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://yr.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ow.jctech888.com.cn

[Q43] 标量子查询
来源：http://hc.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kf.nicolike.cn

[Q44] IN 子查询
来源：http://wv.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jp.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://uh.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iv.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gk.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pm.wgjwhj.cn

[Q47] 与平均值比较
来源：http://cg.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gs.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://ax.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ps.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://rf.lnxyls.cn

[Q49] 更新单行
来源：http://tk.wgjwhj.cn


<!-- 参考信息 -->