代发 wailian999

Java: // 手写回溯递归
来源：http://ju.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://jq.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://bz.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://ha.yuexingan06.cn

[N09] 栈与队列
来源：http://cn.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://um.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dg.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nm.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tx.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ir.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gk.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ti.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rw.hahajie.cn

[N10] 链表节点定义
来源：http://tw.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uq.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ko.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ur.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mo.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://ew.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://df.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qe.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ok.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://bn.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fo.hnjuh.cn

PHP:  // 手写递归函数
来源：http://aw.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mb.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tx.bjjhwx.cn

Java: // 手写递归
来源：http://kd.panjiajie.cn

Go:   // 手写递归
来源：http://pa.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ha.haigaiapp.cn

C#:   // 手写递归
来源：http://aq.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xe.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rf.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ii.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cd.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ck.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://da.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rt.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cf.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bs.hnjuh.cn

================================================================================
来源：http://aa.newstarts.cn

O. 并发与异步
来源：http://uf.muxihuayi.cn

================================================================================
来源：http://ex.jctech888.com.cn

[O01] 启动一个线程
来源：http://ad.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yf.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ex.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://am.newstarts.cn

TS:   // 同 JS
来源：http://ae.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://kf.hahajie.cn

Go:   go f()
来源：http://iy.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://ba.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://zu.hnjuh.cn

[O02] 使用线程池
来源：http://yv.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fs.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yp.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://pt.hahajie.cn

TS:   // worker_threads 线程池
来源：http://qq.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pp.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oc.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://to.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://to.szsharing.cn

[O03] 加锁保护共享数据
来源：http://lq.colortex.cn

Py:   with lock: shared += 1
来源：http://wb.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://om.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jg.lnxyls.cn

TS:   // 同 JS
来源：http://mu.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://gb.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ii.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tf.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://qm.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://zq.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://by.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yc.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://xt.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rx.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sy.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zq.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ea.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://bw.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://ub.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://rq.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kc.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://kb.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://yu.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zc.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xc.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://yi.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ge.jctech888.com.cn

[O06] 使用进程池
来源：http://vn.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://el.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ym.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://ln.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://nm.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lv.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jk.lnxyls.cn

Ruby: // fork 块
来源：http://pu.huixiangedu.cn

C#:   Parallel.For
来源：http://ok.colortex.cn

================================================================================
来源：http://hq.chemitech.net.cn

P. 常用工具函数
来源：http://la.huanxung.cn

================================================================================
来源：http://xi.haigaiapp.cn

[P01] 生成 UUID
来源：http://ur.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://gq.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rk.newstarts.cn

JS:   crypto.randomUUID()
来源：http://vh.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ht.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://qh.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://eg.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://qc.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://rg.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://md.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gi.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://op.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cj.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hm.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ns.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xm.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tk.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jj.nicolike.cn

[P03] 生成短随机字符串
来源：http://pz.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ki.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://og.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wj.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uz.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gq.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qv.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sn.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ul.wgjwhj.cn

[P04] 求长度
来源：http://ci.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bh.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pe.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ii.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jq.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://xr.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://lk.521024.cn

Ruby: x.length;  x.size
来源：http://pu.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mn.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://qq.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qy.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yx.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tp.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fl.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xs.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ow.yuntaijiaju.cn

Ruby: a == b
来源：http://dn.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eh.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ey.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nj.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://sy.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kj.shxzskj.cn

TS:   if (x == null) {}
来源：http://sj.muxihuayi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xd.panjiajie.cn

Go:   if x == nil {}
来源：http://te.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dr.muxihuayi.cn

C#:   if (x is null) {}
来源：http://yn.yuexingan06.cn

[P07] 防抖与节流
来源：http://we.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sd.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://ks.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ls.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hw.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oj.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ai.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://so.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nw.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://zy.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bq.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bl.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zh.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lv.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://km.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qn.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ka.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mz.szxytkj.cn

================================================================================
来源：http://jp.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qf.gzmigu.cn

================================================================================
来源：http://hf.gzmigu.cn

[Q01] 创建表
来源：http://em.huanxung.cn

CREATE TABLE users (
来源：http://yh.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cn.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://zb.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://cz.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ns.wgjwhj.cn

);
来源：http://tt.panjiajie.cn

[Q02] 创建带外键的表
来源：http://ty.9csxet.cn

CREATE TABLE orders (
来源：http://fa.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qi.wgjwhj.cn

user_id INT NOT NULL,
来源：http://gz.szsharing.cn

amount DECIMAL(10, 2),
来源：http://hg.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ir.bookmarksfly.cn

);
来源：http://th.hahajie.cn

[Q03] 增加列
来源：http://pl.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zm.hnjuh.cn

[Q04] 修改列类型
来源：http://cm.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qo.hahajie.cn

[Q05] 重命名列
来源：http://nb.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dv.nszjky.cn

[Q06] 删除列
来源：http://lm.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oh.muxihuayi.cn

[Q07] 删除表
来源：http://qg.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://kt.9csxet.cn

[Q08] 创建普通索引
来源：http://av.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lq.lnxyls.cn

[Q09] 创建唯一索引
来源：http://ty.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tb.gzmigu.cn

[Q10] 插入单行
来源：http://pu.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uj.bjjhwx.cn

[Q11] 一次插入多行
来源：http://nt.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ny.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://xj.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ln.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uq.colortex.cn

[Q13] 忽略重复插入
来源：http://uu.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cj.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://gh.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kg.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ho.wgjwhj.cn

[Q15] 查询全部
来源：http://ee.shxzskj.cn

SELECT * FROM users;
来源：http://sk.hnjuh.cn

[Q16] 查询指定列
来源：http://cu.jctech888.com.cn

SELECT id, name FROM users;
来源：http://pp.newstarts.cn

[Q17] 条件查询
来源：http://ux.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rp.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://tt.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yh.szxytkj.cn

[Q19] 范围查询
来源：http://rq.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mr.yuntaijiaju.cn

[Q20] IN 列表
来源：http://tg.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qn.jianghongdianzi.cn

[Q21] 空值判断
来源：http://nz.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xj.nszjky.cn

[Q22] 排序
来源：http://ku.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://af.lnxyls.cn

[Q23] 分页
来源：http://lk.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ty.shxzukj.cn

[Q24] 去重
来源：http://xc.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://xp.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://yb.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rs.muxihuayi.cn

[Q26] 计数
来源：http://qm.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://pj.szxytkj.cn

[Q27] 条件计数
来源：http://vd.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wu.nszjky.cn

[Q28] 求和与平均
来源：http://ry.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ey.shxzskj.cn

[Q29] 最大最小值
来源：http://bs.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bj.colortex.cn

[Q30] 分组统计
来源：http://aa.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kd.hahajie.cn

[Q31] 分组后过滤
来源：http://pr.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yf.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://cy.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dq.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://re.9csxet.cn

[Q33] 多列分组
来源：http://zd.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ta.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ch.hnjuh.cn

SELECT * FROM (
来源：http://ne.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kb.jctech888.com.cn

) t WHERE rn = 1;
来源：http://xe.newstarts.cn

[Q35] 内连接
来源：http://ji.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rn.chemitech.net.cn

[Q36] 左连接
来源：http://ru.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eq.asd995.cn

[Q37] 右连接
来源：http://yn.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aq.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pc.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oy.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ei.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ni.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pw.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lf.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://by.nicolike.cn

[Q41] 多表连接
来源：http://gw.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://op.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://gz.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://sd.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://hb.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://iu.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dh.asd995.cn

[Q43] 标量子查询
来源：http://ut.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xu.yuexingan06.cn

[Q44] IN 子查询
来源：http://sn.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nx.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://ho.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hf.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ol.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wp.shxzskj.cn

[Q47] 与平均值比较
来源：http://jb.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ka.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://dc.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lk.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://go.shxzukj.cn

[Q49] 更新单行
来源：http://as.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yk.lnxyls.cn

[Q50] 批量更新
来源：http://qv.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ku.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://va.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sf.huanxung.cn

[Q52] 删除指定行
来源：http://jr.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://qu.bookmarksfly.cn

[Q53] 按条件删除
来源：http://zi.bjjhwx.cn


<!-- 参考信息 -->