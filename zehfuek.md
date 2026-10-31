代发 wailian999

Java: // 手写回溯递归
来源：http://my.shxzukj.cn

Go:   // 手写回溯递归
来源：http://da.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://jw.lnxyls.cn

C#:   // 手写回溯递归
来源：http://nw.nszjky.cn

[N09] 栈与队列
来源：http://rj.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dc.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ki.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vo.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tb.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zg.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aw.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://by.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xv.bookmarksfly.cn

[N10] 链表节点定义
来源：http://sk.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qm.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ev.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wf.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xf.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://uz.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xa.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ap.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aq.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://bl.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fl.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://ol.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://di.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iw.hnjuh.cn

Java: // 手写递归
来源：http://wr.yuntaijiaju.cn

Go:   // 手写递归
来源：http://hw.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vz.9csxet.cn

C#:   // 手写递归
来源：http://ey.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xe.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ec.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zz.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nb.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wt.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uh.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vg.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lz.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zz.yuexingan06.cn

================================================================================
来源：http://uv.yuexingan06.cn

O. 并发与异步
来源：http://wp.bookmarksfly.cn

================================================================================
来源：http://pr.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://an.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tj.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pd.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gr.jctech888.com.cn

TS:   // 同 JS
来源：http://ta.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://wk.yuexingan06.cn

Go:   go f()
来源：http://hn.newstarts.cn

Ruby: Thread.new { f }
来源：http://df.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://fs.huixinmuqiang.cn

[O02] 使用线程池
来源：http://gb.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yr.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gm.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://qa.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://fa.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qy.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zg.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ut.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vn.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://qx.panjiajie.cn

Py:   with lock: shared += 1
来源：http://sv.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ky.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zx.yuexingan06.cn

TS:   // 同 JS
来源：http://co.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://tp.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rp.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tc.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://pc.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://fj.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://rx.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://or.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://df.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fy.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ry.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ry.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ak.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://cu.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://zp.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://hl.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gu.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://rd.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://rw.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ap.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sa.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://ot.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ga.newstarts.cn

[O06] 使用进程池
来源：http://gk.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://do.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ws.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://yb.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://xs.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wp.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://li.asd995.cn

Ruby: // fork 块
来源：http://kg.huixiangedu.cn

C#:   Parallel.For
来源：http://qd.jianghongdianzi.cn

================================================================================
来源：http://qs.newstarts.cn

P. 常用工具函数
来源：http://su.huanxung.cn

================================================================================
来源：http://ew.colortex.cn

[P01] 生成 UUID
来源：http://oe.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://uv.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yu.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://wk.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://lg.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://dv.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://pr.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://bb.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://rm.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://az.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mh.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ss.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ni.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pd.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qe.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lu.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jj.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zn.colortex.cn

[P03] 生成短随机字符串
来源：http://ap.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kt.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jn.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gg.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nh.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vw.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mq.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xv.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tk.huixiangedu.cn

[P04] 求长度
来源：http://vj.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xi.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://di.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jt.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jq.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://av.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://vp.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://ru.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ql.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://ns.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rx.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vv.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://of.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ut.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xm.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hv.nicolike.cn

Ruby: a == b
来源：http://uy.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zw.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ax.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vx.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://nt.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://th.asd995.cn

TS:   if (x == null) {}
来源：http://rp.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://na.szxytkj.cn

Go:   if x == nil {}
来源：http://rc.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aa.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://je.chemitech.net.cn

[P07] 防抖与节流
来源：http://hq.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://it.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://xp.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gq.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zo.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ou.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dy.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kc.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iw.huanxung.cn

[P08] 处理浮点精度问题
来源：http://na.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uj.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tw.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vi.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mc.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bk.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aj.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aa.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://al.521024.cn

================================================================================
来源：http://om.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lv.bookmarksfly.cn

================================================================================
来源：http://su.szsharing.cn

[Q01] 创建表
来源：http://tj.panjiajie.cn

CREATE TABLE users (
来源：http://zh.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xw.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ld.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://su.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yv.hahajie.cn

);
来源：http://eb.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://nu.szsharing.cn

CREATE TABLE orders (
来源：http://kd.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ok.szxytkj.cn

user_id INT NOT NULL,
来源：http://uj.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://uk.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ab.521024.cn

);
来源：http://mx.yuntaijiaju.cn

[Q03] 增加列
来源：http://lt.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qu.wgjwhj.cn

[Q04] 修改列类型
来源：http://em.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ux.huanxung.cn

[Q05] 重命名列
来源：http://ma.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ud.newstarts.cn

[Q06] 删除列
来源：http://zu.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pz.hahajie.cn

[Q07] 删除表
来源：http://wd.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://jn.newstarts.cn

[Q08] 创建普通索引
来源：http://oo.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://px.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://kt.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ej.huixinmuqiang.cn

[Q10] 插入单行
来源：http://xc.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ej.hnjuh.cn

[Q11] 一次插入多行
来源：http://wz.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oq.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://me.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ge.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ud.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://hw.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mk.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://av.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cv.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bx.yuntaijiaju.cn

[Q15] 查询全部
来源：http://oh.colortex.cn

SELECT * FROM users;
来源：http://pn.huanxung.cn

[Q16] 查询指定列
来源：http://wt.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://ph.huixinmuqiang.cn

[Q17] 条件查询
来源：http://xn.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tl.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://eg.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sn.szxytkj.cn

[Q19] 范围查询
来源：http://rd.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gn.panjiajie.cn

[Q20] IN 列表
来源：http://rb.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xw.9csxet.cn

[Q21] 空值判断
来源：http://mh.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ks.huanxung.cn

[Q22] 排序
来源：http://dl.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yw.wgjwhj.cn

[Q23] 分页
来源：http://ij.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nc.chemitech.net.cn

[Q24] 去重
来源：http://kr.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ux.nicolike.cn

[Q25] 只取前 N 条
来源：http://po.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://av.nszjky.cn

[Q26] 计数
来源：http://kz.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://oa.hnjuh.cn

[Q27] 条件计数
来源：http://go.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ts.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://fh.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lo.jctech888.com.cn

[Q29] 最大最小值
来源：http://zb.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pq.haigaiapp.cn

[Q30] 分组统计
来源：http://av.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kz.lnxyls.cn

[Q31] 分组后过滤
来源：http://tj.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sx.szsharing.cn

[Q32] 分组拼接字符串
来源：http://fp.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rn.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zt.huixinmuqiang.cn

[Q33] 多列分组
来源：http://qq.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qp.huixiangedu.cn

[Q34] 每组取第一条
来源：http://nr.chemitech.net.cn

SELECT * FROM (
来源：http://rl.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mt.wgjwhj.cn

) t WHERE rn = 1;
来源：http://bs.jctech888.com.cn

[Q35] 内连接
来源：http://mb.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rz.shxzukj.cn

[Q36] 左连接
来源：http://ue.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ci.szxytkj.cn

[Q37] 右连接
来源：http://le.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ju.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://di.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wc.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://ah.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ej.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zt.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hp.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://we.shxzukj.cn

[Q41] 多表连接
来源：http://mp.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wv.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://yx.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://en.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://dq.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://ty.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gu.colortex.cn

[Q43] 标量子查询
来源：http://ai.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yu.bjjhwx.cn

[Q44] IN 子查询
来源：http://el.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sz.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://ik.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vv.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rl.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zi.shtwfgs.cn

[Q47] 与平均值比较
来源：http://tq.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qh.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://id.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ai.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://og.jctech888.com.cn

[Q49] 更新单行
来源：http://vc.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ts.wgjwhj.cn

[Q50] 批量更新
来源：http://ga.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ar.shxzukj.cn

[Q51] 用子查询更新
来源：http://cs.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ut.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://ww.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://pz.lnxyls.cn

[Q53] 按条件删除
来源：http://zi.bjjhwx.cn


<!-- 参考信息 -->