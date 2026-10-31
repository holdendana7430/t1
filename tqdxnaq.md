代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xj.nicolike.cn

[N06] 判断回文字符串
来源：http://fa.nicolike.cn

Py:   s == s[::-1]
来源：http://ma.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://qy.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://qd.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://as.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ow.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://lg.haigaiapp.cn

Ruby: s == s.reverse
来源：http://pm.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://up.521024.cn

[N07] 两数之和（返回下标）
来源：http://dl.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vt.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ux.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://at.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://bj.muxihuayi.cn

Java: // 手写 HashMap
来源：http://id.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://vw.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://op.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tp.wgjwhj.cn

[N08] 生成全排列
来源：http://ze.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://vl.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://jf.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://jr.shxzukj.cn

TS:   // 手写回溯递归
来源：http://yk.9csxet.cn

Java: // 手写回溯递归
来源：http://js.gzmigu.cn

Go:   // 手写回溯递归
来源：http://rv.colortex.cn

Ruby: arr.permutation.to_a
来源：http://oy.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://qp.shxzukj.cn

[N09] 栈与队列
来源：http://ow.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://us.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eh.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://om.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rt.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tk.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tl.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cp.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ef.hnjuh.cn

[N10] 链表节点定义
来源：http://rq.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sj.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xs.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ri.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pw.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://wq.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jx.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://st.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ec.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://qa.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tt.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://ks.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hw.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ye.asd995.cn

Java: // 手写递归
来源：http://nw.haigaiapp.cn

Go:   // 手写递归
来源：http://jn.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vg.yuexingan06.cn

C#:   // 手写递归
来源：http://ao.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qv.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ev.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ct.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lu.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xt.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ao.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oy.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://se.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yi.huanxung.cn

================================================================================
来源：http://rc.haigaiapp.cn

O. 并发与异步
来源：http://mf.huixiangedu.cn

================================================================================
来源：http://ia.shxzskj.cn

[O01] 启动一个线程
来源：http://xw.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kn.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mj.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hr.yuexingan06.cn

TS:   // 同 JS
来源：http://zl.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://qe.shxzskj.cn

Go:   go f()
来源：http://qr.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://ly.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://pk.yuntaijiaju.cn

[O02] 使用线程池
来源：http://jg.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ey.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://do.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://kl.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://vy.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lb.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jx.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wj.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kc.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://bf.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://fi.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://he.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kr.lnxyls.cn

TS:   // 同 JS
来源：http://us.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://mx.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nc.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ut.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://jm.9csxet.cn

[O04] 定义异步函数并等待
来源：http://qs.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://rq.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fy.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://yb.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ju.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qx.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kx.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nr.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://kr.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://nv.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://bc.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://am.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://kr.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://bb.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sz.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qu.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://em.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gh.521024.cn

[O06] 使用进程池
来源：http://sq.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cn.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vt.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://wz.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://zf.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ep.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dr.huixiangedu.cn

Ruby: // fork 块
来源：http://oz.bjjhwx.cn

C#:   Parallel.For
来源：http://vc.wgjwhj.cn

================================================================================
来源：http://zz.huixinmuqiang.cn

P. 常用工具函数
来源：http://rz.huixinmuqiang.cn

================================================================================
来源：http://at.asd995.cn

[P01] 生成 UUID
来源：http://ah.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://ed.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://el.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://nv.newstarts.cn

TS:   crypto.randomUUID()
来源：http://zd.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://yx.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://gm.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://wn.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://dh.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://fz.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xo.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tv.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vl.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uz.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hh.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kk.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yy.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://so.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://af.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tu.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cx.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xy.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yv.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ta.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fh.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hm.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ht.yuexingan06.cn

[P04] 求长度
来源：http://yx.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dr.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sw.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ek.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ih.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://ig.nicolike.cn

Go:   len(arr);  len(m)
来源：http://vl.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://qm.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jh.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://ns.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://av.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gi.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vw.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hu.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://am.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://et.huanxung.cn

Ruby: a == b
来源：http://ni.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hb.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gx.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oz.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://cs.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fb.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://gx.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yh.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://gz.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ih.haigaiapp.cn

C#:   if (x is null) {}
来源：http://na.gzmigu.cn

[P07] 防抖与节流
来源：http://wl.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qo.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://vc.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wo.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nm.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ka.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pr.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ww.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cv.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://as.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oi.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ss.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fs.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qb.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rt.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oq.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mz.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ok.wgjwhj.cn

================================================================================
来源：http://kl.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nd.huixinmuqiang.cn

================================================================================
来源：http://ri.shxzskj.cn

[Q01] 创建表
来源：http://cw.szxytkj.cn

CREATE TABLE users (
来源：http://js.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dv.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://jk.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://vm.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rv.nszjky.cn

);
来源：http://qw.shxzukj.cn

[Q02] 创建带外键的表
来源：http://ua.asd995.cn

CREATE TABLE orders (
来源：http://nj.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ph.shxzskj.cn

user_id INT NOT NULL,
来源：http://lf.hahajie.cn

amount DECIMAL(10, 2),
来源：http://wr.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aa.9csxet.cn

);
来源：http://nx.huixiangedu.cn

[Q03] 增加列
来源：http://yp.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zw.huixiangedu.cn

[Q04] 修改列类型
来源：http://yl.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oj.jctech888.com.cn

[Q05] 重命名列
来源：http://fg.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pg.jctech888.com.cn

[Q06] 删除列
来源：http://du.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wb.521024.cn

[Q07] 删除表
来源：http://bj.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://wq.jctech888.com.cn

[Q08] 创建普通索引
来源：http://db.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fq.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://hz.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mw.nszjky.cn

[Q10] 插入单行
来源：http://xl.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qj.muxihuayi.cn

[Q11] 一次插入多行
来源：http://qb.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zx.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://vg.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://no.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hi.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://bt.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fn.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://mc.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ng.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jd.bookmarksfly.cn

[Q15] 查询全部
来源：http://yc.huanxung.cn

SELECT * FROM users;
来源：http://ou.asd995.cn

[Q16] 查询指定列
来源：http://re.lnxyls.cn

SELECT id, name FROM users;
来源：http://up.szsharing.cn

[Q17] 条件查询
来源：http://lo.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qo.nszjky.cn

[Q18] 模糊匹配
来源：http://pm.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wm.newstarts.cn

[Q19] 范围查询
来源：http://rb.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rg.bookmarksfly.cn

[Q20] IN 列表
来源：http://ie.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ud.shxzukj.cn

[Q21] 空值判断
来源：http://of.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ow.bookmarksfly.cn

[Q22] 排序
来源：http://mx.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bg.muxihuayi.cn

[Q23] 分页
来源：http://gm.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vg.jctech888.com.cn

[Q24] 去重
来源：http://cn.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://vo.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://ek.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aw.yuntaijiaju.cn

[Q26] 计数
来源：http://gb.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://dh.szsharing.cn

[Q27] 条件计数
来源：http://kw.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ql.asd995.cn

[Q28] 求和与平均
来源：http://gm.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cu.haigaiapp.cn

[Q29] 最大最小值
来源：http://hg.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hu.jianghongdianzi.cn

[Q30] 分组统计
来源：http://ln.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sy.hnjuh.cn

[Q31] 分组后过滤
来源：http://hs.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ph.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://lp.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://we.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gn.yuexingan06.cn

[Q33] 多列分组
来源：http://zl.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yh.lnxyls.cn

[Q34] 每组取第一条
来源：http://gq.huanxung.cn

SELECT * FROM (
来源：http://za.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gk.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://ch.asd995.cn

[Q35] 内连接
来源：http://mk.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sm.nszjky.cn

[Q36] 左连接
来源：http://bg.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gy.jianghongdianzi.cn

[Q37] 右连接
来源：http://qv.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tb.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fx.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ej.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://pp.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://es.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cn.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tu.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pi.huanxung.cn

[Q41] 多表连接
来源：http://so.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ch.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://qd.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://dr.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://yh.muxihuayi.cn


<!-- 参考信息 -->