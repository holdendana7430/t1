代发 wailian999

[N09] 栈与队列
来源：http://xk.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cq.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xh.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jl.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kv.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ji.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xm.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ue.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://py.wgjwhj.cn

[N10] 链表节点定义
来源：http://cq.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oi.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cz.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lp.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ix.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://xg.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://of.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fo.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bb.nszjky.cn

[N11] 二叉树中序遍历
来源：http://lt.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ik.nicolike.cn

PHP:  // 手写递归函数
来源：http://kg.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sr.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nb.asd995.cn

Java: // 手写递归
来源：http://ez.muxihuayi.cn

Go:   // 手写递归
来源：http://rz.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pu.bookmarksfly.cn

C#:   // 手写递归
来源：http://bg.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qb.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dk.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://up.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eu.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kr.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wk.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vz.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fk.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qp.gzmigu.cn

================================================================================
来源：http://wj.huanxung.cn

O. 并发与异步
来源：http://eb.gzmigu.cn

================================================================================
来源：http://bf.nszjky.cn

[O01] 启动一个线程
来源：http://wb.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ti.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hv.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uz.hahajie.cn

TS:   // 同 JS
来源：http://ep.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://ni.hahajie.cn

Go:   go f()
来源：http://wv.9csxet.cn

Ruby: Thread.new { f }
来源：http://gp.asd995.cn

C#:   Task.Run(() => F());
来源：http://gj.bjjhwx.cn

[O02] 使用线程池
来源：http://if.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rv.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tw.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://iz.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://bq.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aj.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gv.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ry.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xg.nszjky.cn

[O03] 加锁保护共享数据
来源：http://uv.asd995.cn

Py:   with lock: shared += 1
来源：http://xv.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://uz.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pj.521024.cn

TS:   // 同 JS
来源：http://ro.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://ef.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eg.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qa.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://sz.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://li.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://jx.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bv.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://yd.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mb.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jr.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ae.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sq.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://os.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://sh.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://is.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eq.521024.cn

JS:   await Promise.all(tasks)
来源：http://gq.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://gv.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jx.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xy.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://al.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qz.huixinmuqiang.cn

[O06] 使用进程池
来源：http://lg.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xd.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://py.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://ii.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://df.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gc.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mq.lnxyls.cn

Ruby: // fork 块
来源：http://nq.shxzukj.cn

C#:   Parallel.For
来源：http://dk.yuexingan06.cn

================================================================================
来源：http://of.jianghongdianzi.cn

P. 常用工具函数
来源：http://zk.haigaiapp.cn

================================================================================
来源：http://ut.shxzukj.cn

[P01] 生成 UUID
来源：http://go.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://ax.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ia.asd995.cn

JS:   crypto.randomUUID()
来源：http://qk.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://kq.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://pr.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://zl.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://vb.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://cz.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://fs.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lf.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ks.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lt.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vy.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hn.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rr.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yg.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://if.gzmigu.cn

[P03] 生成短随机字符串
来源：http://xk.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ef.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://du.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://da.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kl.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://de.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ys.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://er.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ar.huixinmuqiang.cn

[P04] 求长度
来源：http://zl.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kf.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ti.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dd.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://he.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://vg.521024.cn

Go:   len(arr);  len(m)
来源：http://cj.9csxet.cn

Ruby: x.length;  x.size
来源：http://ni.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zl.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://hs.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bx.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qz.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xz.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ks.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bb.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oj.hnjuh.cn

Ruby: a == b
来源：http://xz.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ym.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ww.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ry.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://vg.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lp.colortex.cn

TS:   if (x == null) {}
来源：http://sh.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hp.haigaiapp.cn

Go:   if x == nil {}
来源：http://gx.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xk.shxzukj.cn

C#:   if (x is null) {}
来源：http://ph.huanxung.cn

[P07] 防抖与节流
来源：http://id.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tt.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://ul.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wk.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nh.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uf.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wi.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pk.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://za.huanxung.cn

[P08] 处理浮点精度问题
来源：http://gs.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bk.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://co.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jh.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ug.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://go.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mj.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oq.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xd.szxytkj.cn

================================================================================
来源：http://io.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ww.huixiangedu.cn

================================================================================
来源：http://ad.huanxung.cn

[Q01] 创建表
来源：http://vm.yuexingan06.cn

CREATE TABLE users (
来源：http://ia.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xl.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://rd.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://bh.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ib.wgjwhj.cn

);
来源：http://br.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://gc.chemitech.net.cn

CREATE TABLE orders (
来源：http://jr.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eo.hahajie.cn

user_id INT NOT NULL,
来源：http://et.521024.cn

amount DECIMAL(10, 2),
来源：http://ku.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aj.wgjwhj.cn

);
来源：http://os.shxzskj.cn

[Q03] 增加列
来源：http://rx.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qb.asd995.cn

[Q04] 修改列类型
来源：http://zq.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iw.yuexingan06.cn

[Q05] 重命名列
来源：http://uh.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aw.szsharing.cn

[Q06] 删除列
来源：http://is.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ty.jianghongdianzi.cn

[Q07] 删除表
来源：http://la.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ib.asd995.cn

[Q08] 创建普通索引
来源：http://ur.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yi.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://hl.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zn.hnjuh.cn

[Q10] 插入单行
来源：http://wl.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gl.yuexingan06.cn

[Q11] 一次插入多行
来源：http://qb.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ln.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://tm.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bc.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://os.colortex.cn

[Q13] 忽略重复插入
来源：http://sh.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://re.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://za.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vc.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vx.panjiajie.cn

[Q15] 查询全部
来源：http://gu.nszjky.cn

SELECT * FROM users;
来源：http://cs.lnxyls.cn

[Q16] 查询指定列
来源：http://bs.szxytkj.cn

SELECT id, name FROM users;
来源：http://ow.szsharing.cn

[Q17] 条件查询
来源：http://up.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mg.panjiajie.cn

[Q18] 模糊匹配
来源：http://fq.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sy.nszjky.cn

[Q19] 范围查询
来源：http://yq.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uc.szsharing.cn

[Q20] IN 列表
来源：http://jk.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zw.shxzskj.cn

[Q21] 空值判断
来源：http://mq.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ug.9csxet.cn

[Q22] 排序
来源：http://qo.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tm.shtwfgs.cn

[Q23] 分页
来源：http://tu.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vj.haigaiapp.cn

[Q24] 去重
来源：http://bo.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://yi.nicolike.cn

[Q25] 只取前 N 条
来源：http://iw.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://le.9csxet.cn

[Q26] 计数
来源：http://ef.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://to.hahajie.cn

[Q27] 条件计数
来源：http://pc.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kh.jctech888.com.cn

[Q28] 求和与平均
来源：http://zz.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iv.gzmigu.cn

[Q29] 最大最小值
来源：http://ha.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ao.hnjuh.cn

[Q30] 分组统计
来源：http://qc.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rx.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://km.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wf.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://dr.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jq.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vy.huixinmuqiang.cn

[Q33] 多列分组
来源：http://mn.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wc.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://ix.newstarts.cn

SELECT * FROM (
来源：http://yf.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://on.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://qv.newstarts.cn

[Q35] 内连接
来源：http://tm.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bk.szsharing.cn

[Q36] 左连接
来源：http://zr.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ac.shxzukj.cn

[Q37] 右连接
来源：http://cq.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ac.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ku.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sw.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://dp.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hx.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mz.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bn.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ri.huixiangedu.cn

[Q41] 多表连接
来源：http://yj.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ev.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://yx.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://ku.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://ph.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://vi.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kq.shtwfgs.cn

[Q43] 标量子查询
来源：http://ia.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pw.gzmigu.cn

[Q44] IN 子查询
来源：http://xc.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xk.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://ex.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ze.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fq.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bv.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://bi.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jx.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://xv.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qh.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://to.colortex.cn

[Q49] 更新单行
来源：http://eq.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cg.yuntaijiaju.cn

[Q50] 批量更新
来源：http://ol.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://he.newstarts.cn

[Q51] 用子查询更新
来源：http://xh.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ul.hahajie.cn

[Q52] 删除指定行
来源：http://il.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://cq.yuexingan06.cn

[Q53] 按条件删除
来源：http://mu.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gg.haigaiapp.cn

[Q54] 清空表
来源：http://ux.colortex.cn

TRUNCATE TABLE logs;
来源：http://yn.9csxet.cn

[Q55] 排名（并列占位）
来源：http://tg.huixinmuqiang.cn


<!-- 参考信息 -->