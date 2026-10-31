代发 wailian999

Py:   itertools.permutations(arr)
来源：http://sl.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://yw.shxzukj.cn

JS:   // 手写回溯递归
来源：http://tk.lnxyls.cn

TS:   // 手写回溯递归
来源：http://pf.chemitech.net.cn

Java: // 手写回溯递归
来源：http://sq.szsharing.cn

Go:   // 手写回溯递归
来源：http://fl.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://uq.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://ov.colortex.cn

[N09] 栈与队列
来源：http://tq.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zj.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zh.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mv.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nz.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cl.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pn.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mc.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fo.muxihuayi.cn

[N10] 链表节点定义
来源：http://kr.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nj.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yu.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://is.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ph.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://jz.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dn.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nc.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wj.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://jo.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://au.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://sh.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mo.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xc.szxytkj.cn

Java: // 手写递归
来源：http://fm.lnxyls.cn

Go:   // 手写递归
来源：http://sr.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ks.huixinmuqiang.cn

C#:   // 手写递归
来源：http://rp.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xa.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pw.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vu.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rf.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fl.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://az.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dn.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vk.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ea.bookmarksfly.cn

================================================================================
来源：http://gh.bjjhwx.cn

O. 并发与异步
来源：http://vc.shtwfgs.cn

================================================================================
来源：http://wr.nicolike.cn

[O01] 启动一个线程
来源：http://sz.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wd.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mv.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ak.huixinmuqiang.cn

TS:   // 同 JS
来源：http://hv.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://tc.nicolike.cn

Go:   go f()
来源：http://uk.nicolike.cn

Ruby: Thread.new { f }
来源：http://ed.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://gk.szsharing.cn

[O02] 使用线程池
来源：http://co.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fg.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zm.9csxet.cn

JS:   // worker_threads 线程池
来源：http://ey.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://et.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bj.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://om.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sd.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://im.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://yx.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://qw.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://rj.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ke.jctech888.com.cn

TS:   // 同 JS
来源：http://fe.521024.cn

Java: synchronized (this) { shared++; }
来源：http://qg.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xi.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bc.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://jb.huanxung.cn

[O04] 定义异步函数并等待
来源：http://pn.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://ju.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gl.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://xq.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://um.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bd.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pp.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ot.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://lx.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://ay.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://bw.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vh.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://hz.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://pi.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mx.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cy.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://nf.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pl.huanxung.cn

[O06] 使用进程池
来源：http://oo.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://me.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ur.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://ks.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://jo.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qb.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fu.nicolike.cn

Ruby: // fork 块
来源：http://su.colortex.cn

C#:   Parallel.For
来源：http://tt.asd995.cn

================================================================================
来源：http://xw.gzmigu.cn

P. 常用工具函数
来源：http://qm.nszjky.cn

================================================================================
来源：http://dp.haigaiapp.cn

[P01] 生成 UUID
来源：http://bm.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://ky.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sj.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://hp.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://co.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://cx.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://bl.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://co.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://eb.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://kk.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qc.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ug.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dd.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vd.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kz.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wa.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kq.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ff.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://pl.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pt.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fc.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fc.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://al.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kg.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gp.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://eq.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mw.yuntaijiaju.cn

[P04] 求长度
来源：http://tj.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nz.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gc.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mq.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sj.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://mi.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://du.newstarts.cn

Ruby: x.length;  x.size
来源：http://ig.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ki.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://dn.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fp.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mz.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dn.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fp.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nb.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ev.asd995.cn

Ruby: a == b
来源：http://uw.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rj.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wq.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://te.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://tm.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wu.colortex.cn

TS:   if (x == null) {}
来源：http://as.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hb.asd995.cn

Go:   if x == nil {}
来源：http://oi.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hv.wgjwhj.cn

C#:   if (x is null) {}
来源：http://fb.nszjky.cn

[P07] 防抖与节流
来源：http://if.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bu.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://on.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ud.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://st.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sq.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cs.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gj.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xa.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://if.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ew.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://av.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lk.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hv.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://be.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xw.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yi.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ct.huixiangedu.cn

================================================================================
来源：http://jq.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dp.yuntaijiaju.cn

================================================================================
来源：http://oh.nicolike.cn

[Q01] 创建表
来源：http://xx.huixinmuqiang.cn

CREATE TABLE users (
来源：http://li.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uh.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://xq.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://on.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zz.521024.cn

);
来源：http://jk.szxytkj.cn

[Q02] 创建带外键的表
来源：http://zp.9csxet.cn

CREATE TABLE orders (
来源：http://jf.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jc.szxytkj.cn

user_id INT NOT NULL,
来源：http://pu.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://rr.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gu.nszjky.cn

);
来源：http://na.nicolike.cn

[Q03] 增加列
来源：http://uu.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xf.szsharing.cn

[Q04] 修改列类型
来源：http://yg.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hu.wgjwhj.cn

[Q05] 重命名列
来源：http://hz.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cb.shxzukj.cn

[Q06] 删除列
来源：http://lu.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mi.muxihuayi.cn

[Q07] 删除表
来源：http://ss.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://db.gzmigu.cn

[Q08] 创建普通索引
来源：http://gf.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cu.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://gm.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ih.bjjhwx.cn

[Q10] 插入单行
来源：http://sr.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://av.szsharing.cn

[Q11] 一次插入多行
来源：http://rq.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sv.asd995.cn

[Q12] 插入后取自增 ID
来源：http://ps.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://of.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kz.9csxet.cn

[Q13] 忽略重复插入
来源：http://ew.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ww.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://pt.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://we.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://or.9csxet.cn

[Q15] 查询全部
来源：http://ah.lnxyls.cn

SELECT * FROM users;
来源：http://hz.hahajie.cn

[Q16] 查询指定列
来源：http://yj.shtwfgs.cn

SELECT id, name FROM users;
来源：http://ct.nszjky.cn

[Q17] 条件查询
来源：http://lb.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oe.shxzukj.cn

[Q18] 模糊匹配
来源：http://yn.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://of.shxzukj.cn

[Q19] 范围查询
来源：http://al.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jj.szxytkj.cn

[Q20] IN 列表
来源：http://qt.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ko.szsharing.cn

[Q21] 空值判断
来源：http://ds.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xw.muxihuayi.cn

[Q22] 排序
来源：http://tu.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ji.521024.cn

[Q23] 分页
来源：http://xn.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pd.huanxung.cn

[Q24] 去重
来源：http://df.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://qt.hahajie.cn

[Q25] 只取前 N 条
来源：http://mt.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://md.gzmigu.cn

[Q26] 计数
来源：http://sm.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://fa.newstarts.cn

[Q27] 条件计数
来源：http://vw.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ln.hahajie.cn

[Q28] 求和与平均
来源：http://qi.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zf.wgjwhj.cn

[Q29] 最大最小值
来源：http://na.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eg.jctech888.com.cn

[Q30] 分组统计
来源：http://fo.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wp.panjiajie.cn

[Q31] 分组后过滤
来源：http://mz.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wd.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://wt.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bp.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ho.jianghongdianzi.cn

[Q33] 多列分组
来源：http://nq.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kw.nszjky.cn

[Q34] 每组取第一条
来源：http://zh.asd995.cn

SELECT * FROM (
来源：http://go.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tm.colortex.cn

) t WHERE rn = 1;
来源：http://jv.bookmarksfly.cn

[Q35] 内连接
来源：http://bs.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fe.szxytkj.cn

[Q36] 左连接
来源：http://rj.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ut.jctech888.com.cn

[Q37] 右连接
来源：http://sy.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wz.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dv.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hk.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://ay.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vm.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zw.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://so.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ha.jianghongdianzi.cn

[Q41] 多表连接
来源：http://oc.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hb.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://jj.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://pk.521024.cn

[Q42] 连接条件附加过滤
来源：http://yo.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://qn.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dj.gzmigu.cn

[Q43] 标量子查询
来源：http://fh.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://to.shxzukj.cn

[Q44] IN 子查询
来源：http://fh.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ij.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://px.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qw.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bo.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nu.gzmigu.cn

[Q47] 与平均值比较
来源：http://lb.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wd.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://as.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cf.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://hq.huixinmuqiang.cn

[Q49] 更新单行
来源：http://om.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zv.newstarts.cn

[Q50] 批量更新
来源：http://uu.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iq.521024.cn

[Q51] 用子查询更新
来源：http://jp.shxzukj.cn


<!-- 参考信息 -->