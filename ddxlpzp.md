代发 wailian999

Ruby: s == s.reverse
来源：http://yq.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xz.521024.cn

[N07] 两数之和（返回下标）
来源：http://tl.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sr.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://is.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gi.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://wx.szxytkj.cn

Java: // 手写 HashMap
来源：http://kh.colortex.cn

Go:   // 手写 map[int]int
来源：http://wg.9csxet.cn

Ruby: // 手写 Hash
来源：http://zq.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mz.9csxet.cn

[N08] 生成全排列
来源：http://fx.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://wm.newstarts.cn

PHP:  // 手写递归交换
来源：http://zi.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://ez.shxzskj.cn

TS:   // 手写回溯递归
来源：http://le.haigaiapp.cn

Java: // 手写回溯递归
来源：http://gx.shxzukj.cn

Go:   // 手写回溯递归
来源：http://iy.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://ll.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://zv.newstarts.cn

[N09] 栈与队列
来源：http://bh.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uk.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sg.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bn.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rx.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bz.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yr.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://im.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vp.haigaiapp.cn

[N10] 链表节点定义
来源：http://hd.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ca.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yy.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fq.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mk.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://zl.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hk.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hk.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://do.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://br.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://km.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://xr.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yi.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xr.gzmigu.cn

Java: // 手写递归
来源：http://nc.wgjwhj.cn

Go:   // 手写递归
来源：http://lh.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hc.huixiangedu.cn

C#:   // 手写递归
来源：http://og.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xx.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://or.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gn.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://em.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nr.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bh.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://io.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ja.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xe.shxzukj.cn

================================================================================
来源：http://tg.nszjky.cn

O. 并发与异步
来源：http://hj.yuntaijiaju.cn

================================================================================
来源：http://ao.521024.cn

[O01] 启动一个线程
来源：http://go.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://io.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ty.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qc.yuexingan06.cn

TS:   // 同 JS
来源：http://op.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://oo.shtwfgs.cn

Go:   go f()
来源：http://tr.asd995.cn

Ruby: Thread.new { f }
来源：http://ow.szsharing.cn

C#:   Task.Run(() => F());
来源：http://le.muxihuayi.cn

[O02] 使用线程池
来源：http://yh.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yy.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cr.asd995.cn

JS:   // worker_threads 线程池
来源：http://da.huanxung.cn

TS:   // worker_threads 线程池
来源：http://nb.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xe.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eq.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sb.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xp.nszjky.cn

[O03] 加锁保护共享数据
来源：http://xi.szsharing.cn

Py:   with lock: shared += 1
来源：http://cp.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://pj.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vm.panjiajie.cn

TS:   // 同 JS
来源：http://gu.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://wp.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://le.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tl.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://xm.nicolike.cn

[O04] 定义异步函数并等待
来源：http://zf.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://id.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jf.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://nw.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nn.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qn.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jy.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cp.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://wv.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://rx.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://kw.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vp.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://pu.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://sr.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://je.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mx.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://pp.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ex.huixiangedu.cn

[O06] 使用进程池
来源：http://fj.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ya.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yc.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://nv.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://rv.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zk.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://um.hnjuh.cn

Ruby: // fork 块
来源：http://sd.newstarts.cn

C#:   Parallel.For
来源：http://ak.huixiangedu.cn

================================================================================
来源：http://ub.jctech888.com.cn

P. 常用工具函数
来源：http://yp.521024.cn

================================================================================
来源：http://yj.asd995.cn

[P01] 生成 UUID
来源：http://ry.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://df.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nu.521024.cn

JS:   crypto.randomUUID()
来源：http://hl.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://sm.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://lw.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://az.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://xa.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://lc.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://ho.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nk.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fu.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oj.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://td.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://py.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ja.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jv.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hc.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://hi.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cj.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://az.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eq.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jf.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wx.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lw.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bf.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ip.shtwfgs.cn

[P04] 求长度
来源：http://nc.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ym.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hk.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ms.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lp.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://gk.colortex.cn

Go:   len(arr);  len(m)
来源：http://be.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ul.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ok.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://me.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kk.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yo.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ik.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fv.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dv.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fy.hnjuh.cn

Ruby: a == b
来源：http://je.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fo.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uh.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yo.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ou.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bt.nicolike.cn

TS:   if (x == null) {}
来源：http://lc.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vf.szxytkj.cn

Go:   if x == nil {}
来源：http://ih.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ig.huixiangedu.cn

C#:   if (x is null) {}
来源：http://gh.asd995.cn

[P07] 防抖与节流
来源：http://lj.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rb.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://aa.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hn.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zf.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tg.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cr.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rk.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://to.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://kd.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sc.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nm.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vm.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hw.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aq.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gs.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ea.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ck.gzmigu.cn

================================================================================
来源：http://ah.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://az.huixinmuqiang.cn

================================================================================
来源：http://hm.chemitech.net.cn

[Q01] 创建表
来源：http://sx.huixiangedu.cn

CREATE TABLE users (
来源：http://wy.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://je.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://cl.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://ki.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yy.hahajie.cn

);
来源：http://ou.huanxung.cn

[Q02] 创建带外键的表
来源：http://gb.colortex.cn

CREATE TABLE orders (
来源：http://ki.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://it.hahajie.cn

user_id INT NOT NULL,
来源：http://ve.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://hf.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://up.gzmigu.cn

);
来源：http://js.asd995.cn

[Q03] 增加列
来源：http://tb.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hy.szxytkj.cn

[Q04] 修改列类型
来源：http://ht.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qb.szsharing.cn

[Q05] 重命名列
来源：http://yt.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oc.bjjhwx.cn

[Q06] 删除列
来源：http://iy.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ff.nszjky.cn

[Q07] 删除表
来源：http://su.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://vn.nszjky.cn

[Q08] 创建普通索引
来源：http://nl.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fc.asd995.cn

[Q09] 创建唯一索引
来源：http://ga.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sn.yuexingan06.cn

[Q10] 插入单行
来源：http://pk.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ne.newstarts.cn

[Q11] 一次插入多行
来源：http://bz.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eb.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://vq.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ay.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wc.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://un.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://am.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://eo.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nq.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ii.nszjky.cn

[Q15] 查询全部
来源：http://ek.yuntaijiaju.cn

SELECT * FROM users;
来源：http://lk.huixiangedu.cn

[Q16] 查询指定列
来源：http://mr.huanxung.cn

SELECT id, name FROM users;
来源：http://cg.muxihuayi.cn

[Q17] 条件查询
来源：http://cq.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://us.szxytkj.cn

[Q18] 模糊匹配
来源：http://hp.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ti.wgjwhj.cn

[Q19] 范围查询
来源：http://xs.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ph.nicolike.cn

[Q20] IN 列表
来源：http://ws.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rt.9csxet.cn

[Q21] 空值判断
来源：http://js.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pb.panjiajie.cn

[Q22] 排序
来源：http://wu.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ls.wgjwhj.cn

[Q23] 分页
来源：http://ot.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ax.yuntaijiaju.cn

[Q24] 去重
来源：http://ts.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://gn.szsharing.cn

[Q25] 只取前 N 条
来源：http://yi.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://si.jctech888.com.cn

[Q26] 计数
来源：http://gl.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://xa.huixiangedu.cn

[Q27] 条件计数
来源：http://ev.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hq.shxzukj.cn

[Q28] 求和与平均
来源：http://ds.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ax.muxihuayi.cn

[Q29] 最大最小值
来源：http://ov.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fg.hahajie.cn

[Q30] 分组统计
来源：http://xs.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yc.shxzskj.cn

[Q31] 分组后过滤
来源：http://ni.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xg.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://jr.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://in.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ud.shxzukj.cn

[Q33] 多列分组
来源：http://to.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jk.wgjwhj.cn

[Q34] 每组取第一条
来源：http://cd.shxzukj.cn

SELECT * FROM (
来源：http://wq.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xj.gzmigu.cn

) t WHERE rn = 1;
来源：http://ue.nszjky.cn

[Q35] 内连接
来源：http://ek.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bm.huixinmuqiang.cn

[Q36] 左连接
来源：http://kj.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jc.huixinmuqiang.cn

[Q37] 右连接
来源：http://ik.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qc.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ph.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ls.colortex.cn

[Q39] 自连接（查上下级）
来源：http://ps.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vo.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vl.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qw.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://py.muxihuayi.cn

[Q41] 多表连接
来源：http://tm.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ei.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://rl.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://wi.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://lu.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://lz.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gc.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://fv.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://an.9csxet.cn

[Q44] IN 子查询
来源：http://uh.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jn.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://tg.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fs.haigaiapp.cn


<!-- 参考信息 -->