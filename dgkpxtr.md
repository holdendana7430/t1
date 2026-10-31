代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mq.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bz.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://to.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://dm.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nj.szxytkj.cn

[N06] 判断回文字符串
来源：http://jz.hahajie.cn

Py:   s == s[::-1]
来源：http://pi.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://rz.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://jt.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://kr.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ke.nicolike.cn

Go:   // 双指针从两端比较
来源：http://sg.shxzskj.cn

Ruby: s == s.reverse
来源：http://wq.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zm.colortex.cn

[N07] 两数之和（返回下标）
来源：http://ba.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sv.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ka.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ox.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://bi.gzmigu.cn

Java: // 手写 HashMap
来源：http://pw.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://ed.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://vk.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kr.yuntaijiaju.cn

[N08] 生成全排列
来源：http://jh.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://md.shxzukj.cn

PHP:  // 手写递归交换
来源：http://oc.gzmigu.cn

JS:   // 手写回溯递归
来源：http://ov.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://cf.shxzskj.cn

Java: // 手写回溯递归
来源：http://uv.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://hf.asd995.cn

Ruby: arr.permutation.to_a
来源：http://jp.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://ac.huanxung.cn

[N09] 栈与队列
来源：http://ip.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pj.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mc.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vt.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fe.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hx.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ky.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pd.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kg.gzmigu.cn

[N10] 链表节点定义
来源：http://sa.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gh.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mg.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wb.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sy.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://oc.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rb.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nv.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jt.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://tx.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mb.panjiajie.cn

PHP:  // 手写递归函数
来源：http://nf.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gw.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kz.wgjwhj.cn

Java: // 手写递归
来源：http://cu.muxihuayi.cn

Go:   // 手写递归
来源：http://kp.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gr.haigaiapp.cn

C#:   // 手写递归
来源：http://vj.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dr.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://at.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uo.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eq.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jz.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mw.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cv.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zj.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ol.shxzukj.cn

================================================================================
来源：http://ca.shtwfgs.cn

O. 并发与异步
来源：http://uq.lnxyls.cn

================================================================================
来源：http://bx.nicolike.cn

[O01] 启动一个线程
来源：http://ka.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yv.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fm.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uo.szxytkj.cn

TS:   // 同 JS
来源：http://yb.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://jm.jianghongdianzi.cn

Go:   go f()
来源：http://fg.hnjuh.cn

Ruby: Thread.new { f }
来源：http://wr.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://iv.jctech888.com.cn

[O02] 使用线程池
来源：http://il.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ae.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tu.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://lf.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://uu.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vy.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uv.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zw.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qh.9csxet.cn

[O03] 加锁保护共享数据
来源：http://fp.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://dd.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://if.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dn.shtwfgs.cn

TS:   // 同 JS
来源：http://yl.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://vs.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vv.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fz.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://tm.huanxung.cn

[O04] 定义异步函数并等待
来源：http://jg.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://wg.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ws.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://ix.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cy.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fz.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bj.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bh.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://yl.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://sl.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://tz.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gh.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://fv.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://fv.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ja.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cv.szsharing.cn

Ruby: threads.map(&:join)
来源：http://rz.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hl.521024.cn

[O06] 使用进程池
来源：http://vu.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mi.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ff.asd995.cn

JS:   // child_process / cluster 模块
来源：http://qx.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://wr.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ie.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oe.colortex.cn

Ruby: // fork 块
来源：http://xw.asd995.cn

C#:   Parallel.For
来源：http://mh.yuntaijiaju.cn

================================================================================
来源：http://up.wgjwhj.cn

P. 常用工具函数
来源：http://vg.haigaiapp.cn

================================================================================
来源：http://cp.lnxyls.cn

[P01] 生成 UUID
来源：http://dq.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://gv.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sy.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://in.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://px.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://ty.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://jp.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://cc.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://nc.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://yp.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tr.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lm.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ur.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ij.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hu.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vy.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yx.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kg.521024.cn

[P03] 生成短随机字符串
来源：http://cl.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oo.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dr.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tv.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rb.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wt.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vo.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ju.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tb.huixinmuqiang.cn

[P04] 求长度
来源：http://dt.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ix.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://px.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zl.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://us.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://pj.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://lc.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://ie.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wt.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://qo.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xw.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tg.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uc.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mu.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://he.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ba.nszjky.cn

Ruby: a == b
来源：http://fn.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kl.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://og.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vn.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://nf.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zf.jctech888.com.cn

TS:   if (x == null) {}
来源：http://jc.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ej.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://ej.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vm.hnjuh.cn

C#:   if (x is null) {}
来源：http://wg.bookmarksfly.cn

[P07] 防抖与节流
来源：http://kc.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yu.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://qk.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aj.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://da.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kc.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aj.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ty.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ra.nszjky.cn

[P08] 处理浮点精度问题
来源：http://xd.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ac.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hw.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vs.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hw.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://af.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ah.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sp.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xg.yuexingan06.cn

================================================================================
来源：http://vt.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gq.huixiangedu.cn

================================================================================
来源：http://iu.nicolike.cn

[Q01] 创建表
来源：http://nw.jianghongdianzi.cn

CREATE TABLE users (
来源：http://vi.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qh.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://mn.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://ne.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://km.newstarts.cn

);
来源：http://qw.szxytkj.cn

[Q02] 创建带外键的表
来源：http://uk.jctech888.com.cn

CREATE TABLE orders (
来源：http://lh.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sv.gzmigu.cn

user_id INT NOT NULL,
来源：http://kf.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://dj.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tb.asd995.cn

);
来源：http://rg.jctech888.com.cn

[Q03] 增加列
来源：http://cd.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xx.huixiangedu.cn

[Q04] 修改列类型
来源：http://jg.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ig.jianghongdianzi.cn

[Q05] 重命名列
来源：http://er.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nl.jianghongdianzi.cn

[Q06] 删除列
来源：http://td.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://so.shxzskj.cn

[Q07] 删除表
来源：http://vz.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://hu.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://yy.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://be.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://af.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ms.panjiajie.cn

[Q10] 插入单行
来源：http://cf.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oq.nicolike.cn

[Q11] 一次插入多行
来源：http://oy.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pj.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://zc.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dt.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lq.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://qu.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ji.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://eb.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ji.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xu.9csxet.cn

[Q15] 查询全部
来源：http://ix.yuntaijiaju.cn

SELECT * FROM users;
来源：http://de.szsharing.cn

[Q16] 查询指定列
来源：http://ic.yuexingan06.cn

SELECT id, name FROM users;
来源：http://iw.huanxung.cn

[Q17] 条件查询
来源：http://dk.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vj.shxzukj.cn

[Q18] 模糊匹配
来源：http://ug.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hc.shtwfgs.cn

[Q19] 范围查询
来源：http://zk.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ei.lnxyls.cn

[Q20] IN 列表
来源：http://ae.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ru.nszjky.cn

[Q21] 空值判断
来源：http://sj.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ph.nicolike.cn

[Q22] 排序
来源：http://md.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yn.9csxet.cn

[Q23] 分页
来源：http://ry.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dv.gzmigu.cn

[Q24] 去重
来源：http://jc.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://vt.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://aq.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://im.bjjhwx.cn

[Q26] 计数
来源：http://ou.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://mi.9csxet.cn

[Q27] 条件计数
来源：http://qi.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ux.gzmigu.cn

[Q28] 求和与平均
来源：http://hj.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rw.shxzukj.cn

[Q29] 最大最小值
来源：http://qh.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xs.szsharing.cn

[Q30] 分组统计
来源：http://kc.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gc.shtwfgs.cn

[Q31] 分组后过滤
来源：http://gd.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bm.asd995.cn

[Q32] 分组拼接字符串
来源：http://sn.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dr.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fe.jianghongdianzi.cn

[Q33] 多列分组
来源：http://oa.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jx.chemitech.net.cn

[Q34] 每组取第一条
来源：http://jx.muxihuayi.cn

SELECT * FROM (
来源：http://jy.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uz.szsharing.cn

) t WHERE rn = 1;
来源：http://hd.chemitech.net.cn

[Q35] 内连接
来源：http://ue.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lx.szxytkj.cn

[Q36] 左连接
来源：http://km.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jj.yuexingan06.cn

[Q37] 右连接
来源：http://qv.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oz.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jq.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://df.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ty.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ey.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tq.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yk.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gj.jianghongdianzi.cn

[Q41] 多表连接
来源：http://og.bjjhwx.cn


<!-- 参考信息 -->