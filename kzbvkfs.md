代发 wailian999

Py:   itertools.permutations(arr)
来源：http://wg.panjiajie.cn

PHP:  // 手写递归交换
来源：http://kq.newstarts.cn

JS:   // 手写回溯递归
来源：http://ye.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://zi.521024.cn

Java: // 手写回溯递归
来源：http://ww.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://zh.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://xn.newstarts.cn

C#:   // 手写回溯递归
来源：http://vf.yuntaijiaju.cn

[N09] 栈与队列
来源：http://my.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yh.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bw.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ut.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ro.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zy.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uv.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://no.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sj.lnxyls.cn

[N10] 链表节点定义
来源：http://fw.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mh.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yp.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://up.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yr.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://ro.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mj.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tp.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xz.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://oz.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ij.lnxyls.cn

PHP:  // 手写递归函数
来源：http://ud.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://np.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jc.hahajie.cn

Java: // 手写递归
来源：http://lz.hnjuh.cn

Go:   // 手写递归
来源：http://nz.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zm.huixinmuqiang.cn

C#:   // 手写递归
来源：http://gj.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://en.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wq.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kf.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lc.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kb.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jo.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nk.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vw.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jj.hnjuh.cn

================================================================================
来源：http://uk.jctech888.com.cn

O. 并发与异步
来源：http://jj.huixiangedu.cn

================================================================================
来源：http://mv.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://nb.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://af.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gl.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mh.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ux.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://hh.colortex.cn

Go:   go f()
来源：http://nd.asd995.cn

Ruby: Thread.new { f }
来源：http://mn.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://lj.hnjuh.cn

[O02] 使用线程池
来源：http://eb.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ws.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ra.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://kh.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://nb.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wv.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lj.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qn.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ph.9csxet.cn

[O03] 加锁保护共享数据
来源：http://da.hnjuh.cn

Py:   with lock: shared += 1
来源：http://vj.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://hi.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ud.jianghongdianzi.cn

TS:   // 同 JS
来源：http://in.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://if.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ku.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ko.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://el.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://sa.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://vl.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qm.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://sd.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fd.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xg.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://li.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://em.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://ix.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://cg.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://cj.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iu.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://zv.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://qk.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ld.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fj.newstarts.cn

Ruby: threads.map(&:join)
来源：http://ju.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jx.bjjhwx.cn

[O06] 使用进程池
来源：http://my.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ds.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hx.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://oj.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://tv.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bk.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sm.bookmarksfly.cn

Ruby: // fork 块
来源：http://dn.huixiangedu.cn

C#:   Parallel.For
来源：http://zv.chemitech.net.cn

================================================================================
来源：http://hu.muxihuayi.cn

P. 常用工具函数
来源：http://re.bjjhwx.cn

================================================================================
来源：http://yu.muxihuayi.cn

[P01] 生成 UUID
来源：http://xu.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://gp.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ec.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://lx.9csxet.cn

TS:   crypto.randomUUID()
来源：http://zb.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://og.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://sm.asd995.cn

Ruby: SecureRandom.uuid
来源：http://ew.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://bm.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://hm.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tq.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ks.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vi.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ps.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sf.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ib.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://su.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jp.szsharing.cn

[P03] 生成短随机字符串
来源：http://qh.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vi.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gl.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hf.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sf.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://br.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rq.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hl.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ei.yuntaijiaju.cn

[P04] 求长度
来源：http://hr.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oc.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qg.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ll.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hs.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://lu.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://xe.521024.cn

Ruby: x.length;  x.size
来源：http://tf.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ld.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://cr.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fu.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jh.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gx.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fg.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ce.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ee.lnxyls.cn

Ruby: a == b
来源：http://ks.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zm.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sb.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vi.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://qp.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xl.colortex.cn

TS:   if (x == null) {}
来源：http://nf.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kf.9csxet.cn

Go:   if x == nil {}
来源：http://rm.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zr.panjiajie.cn

C#:   if (x is null) {}
来源：http://uj.lnxyls.cn

[P07] 防抖与节流
来源：http://ba.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://va.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://ag.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pi.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xb.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ab.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jn.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wk.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sg.hahajie.cn

[P08] 处理浮点精度问题
来源：http://dq.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ti.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jb.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iy.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tz.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yh.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fm.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gp.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ad.yuntaijiaju.cn

================================================================================
来源：http://rn.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qx.panjiajie.cn

================================================================================
来源：http://lo.shtwfgs.cn

[Q01] 创建表
来源：http://vj.colortex.cn

CREATE TABLE users (
来源：http://tg.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ki.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://cx.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://ku.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kn.haigaiapp.cn

);
来源：http://tz.521024.cn

[Q02] 创建带外键的表
来源：http://jw.colortex.cn

CREATE TABLE orders (
来源：http://nd.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vv.colortex.cn

user_id INT NOT NULL,
来源：http://eu.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://qr.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uf.shxzukj.cn

);
来源：http://dm.521024.cn

[Q03] 增加列
来源：http://cb.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bd.shxzskj.cn

[Q04] 修改列类型
来源：http://to.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hd.nicolike.cn

[Q05] 重命名列
来源：http://dg.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vh.yuntaijiaju.cn

[Q06] 删除列
来源：http://ov.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tu.wgjwhj.cn

[Q07] 删除表
来源：http://dd.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://ne.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://oc.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lt.szxytkj.cn

[Q09] 创建唯一索引
来源：http://sn.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://li.colortex.cn

[Q10] 插入单行
来源：http://bc.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pn.shxzskj.cn

[Q11] 一次插入多行
来源：http://sn.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rc.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://gj.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xf.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pj.asd995.cn

[Q13] 忽略重复插入
来源：http://hf.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lp.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://ok.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fb.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://am.jianghongdianzi.cn

[Q15] 查询全部
来源：http://sj.jctech888.com.cn

SELECT * FROM users;
来源：http://ww.huixiangedu.cn

[Q16] 查询指定列
来源：http://xm.nicolike.cn

SELECT id, name FROM users;
来源：http://op.szxytkj.cn

[Q17] 条件查询
来源：http://co.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aj.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://qi.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ql.jianghongdianzi.cn

[Q19] 范围查询
来源：http://yi.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tn.hahajie.cn

[Q20] IN 列表
来源：http://kj.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qy.bookmarksfly.cn

[Q21] 空值判断
来源：http://og.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fk.shxzskj.cn

[Q22] 排序
来源：http://em.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cu.gzmigu.cn

[Q23] 分页
来源：http://nv.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ve.huanxung.cn

[Q24] 去重
来源：http://ra.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://av.gzmigu.cn

[Q25] 只取前 N 条
来源：http://es.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vc.asd995.cn

[Q26] 计数
来源：http://hl.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://nk.haigaiapp.cn

[Q27] 条件计数
来源：http://pb.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bj.nszjky.cn

[Q28] 求和与平均
来源：http://er.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ub.nicolike.cn

[Q29] 最大最小值
来源：http://kv.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qq.lnxyls.cn

[Q30] 分组统计
来源：http://ux.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pi.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://jj.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zt.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://aj.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gc.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sm.muxihuayi.cn

[Q33] 多列分组
来源：http://kc.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rz.chemitech.net.cn

[Q34] 每组取第一条
来源：http://lh.gzmigu.cn

SELECT * FROM (
来源：http://gb.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ja.9csxet.cn

) t WHERE rn = 1;
来源：http://cx.huixiangedu.cn

[Q35] 内连接
来源：http://th.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ov.nicolike.cn

[Q36] 左连接
来源：http://qi.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ro.shxzukj.cn

[Q37] 右连接
来源：http://ht.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://my.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sb.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qf.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://xd.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://li.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ba.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vg.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lw.hahajie.cn

[Q41] 多表连接
来源：http://wq.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cv.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://gz.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://tr.asd995.cn

[Q42] 连接条件附加过滤
来源：http://vf.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://hl.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ij.szxytkj.cn

[Q43] 标量子查询
来源：http://yk.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zj.huixiangedu.cn

[Q44] IN 子查询
来源：http://fb.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://do.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://vi.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iz.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jx.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wd.hahajie.cn

[Q47] 与平均值比较
来源：http://tl.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gy.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://wo.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hw.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://kd.hnjuh.cn

[Q49] 更新单行
来源：http://lm.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qe.521024.cn

[Q50] 批量更新
来源：http://ri.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xv.yuexingan06.cn

[Q51] 用子查询更新
来源：http://ji.nicolike.cn


<!-- 参考信息 -->