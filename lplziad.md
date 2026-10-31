代发 wailian999

Java: // 手写回溯递归
来源：http://gy.shxzukj.cn

Go:   // 手写回溯递归
来源：http://sh.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://zk.szsharing.cn

C#:   // 手写回溯递归
来源：http://pv.wgjwhj.cn

[N09] 栈与队列
来源：http://sp.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uv.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eb.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mb.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yk.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fi.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jh.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bi.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ck.jctech888.com.cn

[N10] 链表节点定义
来源：http://sw.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ph.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ob.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ma.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yc.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://ct.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ia.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rp.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sq.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://zy.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wx.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://hn.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hi.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nz.hnjuh.cn

Java: // 手写递归
来源：http://ce.asd995.cn

Go:   // 手写递归
来源：http://es.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ri.newstarts.cn

C#:   // 手写递归
来源：http://jw.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uz.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ue.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yd.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wc.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fl.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sr.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mp.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vk.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ra.hnjuh.cn

================================================================================
来源：http://ez.jianghongdianzi.cn

O. 并发与异步
来源：http://ve.jctech888.com.cn

================================================================================
来源：http://lb.shxzukj.cn

[O01] 启动一个线程
来源：http://gx.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ff.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yi.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ch.hnjuh.cn

TS:   // 同 JS
来源：http://zd.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ka.nszjky.cn

Go:   go f()
来源：http://py.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://ts.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://fv.nszjky.cn

[O02] 使用线程池
来源：http://zz.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rb.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rb.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://vm.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://rh.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xp.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xh.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://il.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ib.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://ff.9csxet.cn

Py:   with lock: shared += 1
来源：http://rx.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://rz.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uf.shtwfgs.cn

TS:   // 同 JS
来源：http://nc.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://pk.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tl.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pu.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://rg.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://my.asd995.cn

Py:   async def f():⏎    await g()
来源：http://bt.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wz.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://oe.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jl.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yn.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qk.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zk.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://gh.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://cy.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://cl.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kd.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://aw.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://wy.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bv.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vg.asd995.cn

Ruby: threads.map(&:join)
来源：http://zn.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zx.huixinmuqiang.cn

[O06] 使用进程池
来源：http://qo.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nq.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ek.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://lf.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://tq.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gx.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://je.nicolike.cn

Ruby: // fork 块
来源：http://ot.gzmigu.cn

C#:   Parallel.For
来源：http://nk.shxzskj.cn

================================================================================
来源：http://cd.wgjwhj.cn

P. 常用工具函数
来源：http://an.nszjky.cn

================================================================================
来源：http://mp.521024.cn

[P01] 生成 UUID
来源：http://vc.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://ft.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fq.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://li.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://ii.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://lf.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://nm.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://ko.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://xm.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://qb.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://we.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gn.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://be.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tm.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dh.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://go.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sg.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bm.9csxet.cn

[P03] 生成短随机字符串
来源：http://jw.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uo.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uc.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://na.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lh.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zo.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ar.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qf.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rf.shxzskj.cn

[P04] 求长度
来源：http://le.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tz.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://od.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lj.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pi.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://zy.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://cz.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://zm.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://ai.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ju.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cl.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ua.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mq.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nw.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tf.wgjwhj.cn

Ruby: a == b
来源：http://ox.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pg.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ns.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fc.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://px.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rd.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://ua.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://px.gzmigu.cn

Go:   if x == nil {}
来源：http://ki.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vg.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://jf.colortex.cn

[P07] 防抖与节流
来源：http://br.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ho.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://tc.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://db.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lp.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ch.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sp.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vt.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fp.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://hu.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pg.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ny.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ss.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xa.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gr.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wc.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yn.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kw.shtwfgs.cn

================================================================================
来源：http://gw.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rh.huanxung.cn

================================================================================
来源：http://rq.panjiajie.cn

[Q01] 创建表
来源：http://xm.lnxyls.cn

CREATE TABLE users (
来源：http://zn.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tt.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://vl.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://xh.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cc.colortex.cn

);
来源：http://dj.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://sn.szsharing.cn

CREATE TABLE orders (
来源：http://ah.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tp.bjjhwx.cn

user_id INT NOT NULL,
来源：http://cu.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://qb.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rj.jctech888.com.cn

);
来源：http://iz.huixiangedu.cn

[Q03] 增加列
来源：http://yj.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aa.asd995.cn

[Q04] 修改列类型
来源：http://hq.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vp.huanxung.cn

[Q05] 重命名列
来源：http://le.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yj.bookmarksfly.cn

[Q06] 删除列
来源：http://um.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yl.chemitech.net.cn

[Q07] 删除表
来源：http://hn.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://eg.nszjky.cn

[Q08] 创建普通索引
来源：http://qo.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iy.szxytkj.cn

[Q09] 创建唯一索引
来源：http://im.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xs.yuexingan06.cn

[Q10] 插入单行
来源：http://sz.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yb.jctech888.com.cn

[Q11] 一次插入多行
来源：http://cl.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cl.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://ye.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dy.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pr.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://ru.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bg.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://qr.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jn.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cl.shxzukj.cn

[Q15] 查询全部
来源：http://fq.bookmarksfly.cn

SELECT * FROM users;
来源：http://xo.wgjwhj.cn

[Q16] 查询指定列
来源：http://id.521024.cn

SELECT id, name FROM users;
来源：http://li.9csxet.cn

[Q17] 条件查询
来源：http://gy.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ko.hahajie.cn

[Q18] 模糊匹配
来源：http://qr.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nn.jianghongdianzi.cn

[Q19] 范围查询
来源：http://vt.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rl.wgjwhj.cn

[Q20] IN 列表
来源：http://he.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gj.nicolike.cn

[Q21] 空值判断
来源：http://mc.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ft.newstarts.cn

[Q22] 排序
来源：http://cd.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fd.gzmigu.cn

[Q23] 分页
来源：http://qn.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ah.9csxet.cn

[Q24] 去重
来源：http://lo.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://tz.panjiajie.cn

[Q25] 只取前 N 条
来源：http://zw.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xw.lnxyls.cn

[Q26] 计数
来源：http://ef.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://yx.gzmigu.cn

[Q27] 条件计数
来源：http://aw.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://by.muxihuayi.cn

[Q28] 求和与平均
来源：http://sf.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://de.huanxung.cn

[Q29] 最大最小值
来源：http://ic.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pj.chemitech.net.cn

[Q30] 分组统计
来源：http://ds.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hg.521024.cn

[Q31] 分组后过滤
来源：http://yy.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rd.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://av.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rp.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nr.jctech888.com.cn

[Q33] 多列分组
来源：http://lg.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://of.bjjhwx.cn

[Q34] 每组取第一条
来源：http://na.521024.cn

SELECT * FROM (
来源：http://sp.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uj.hahajie.cn

) t WHERE rn = 1;
来源：http://ve.shtwfgs.cn

[Q35] 内连接
来源：http://ra.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yt.panjiajie.cn

[Q36] 左连接
来源：http://no.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vx.lnxyls.cn

[Q37] 右连接
来源：http://rt.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nj.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hx.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dc.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://nc.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cw.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ub.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pi.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ml.shtwfgs.cn

[Q41] 多表连接
来源：http://zt.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qp.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://kn.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://ku.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://yb.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://eu.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mn.muxihuayi.cn

[Q43] 标量子查询
来源：http://ek.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lx.muxihuayi.cn

[Q44] IN 子查询
来源：http://ug.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gl.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://od.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ll.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ne.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hd.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://zi.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lr.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://yz.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ut.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://gz.bookmarksfly.cn

[Q49] 更新单行
来源：http://nt.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jv.shxzskj.cn

[Q50] 批量更新
来源：http://es.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ra.hnjuh.cn

[Q51] 用子查询更新
来源：http://yv.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hr.colortex.cn

[Q52] 删除指定行
来源：http://qh.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://ka.hahajie.cn

[Q53] 按条件删除
来源：http://mx.jianghongdianzi.cn


<!-- 参考信息 -->