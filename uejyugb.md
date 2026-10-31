代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://vb.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ab.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xo.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://py.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ma.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vv.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://gf.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yh.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tx.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fs.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://st.bjjhwx.cn

Java: // 手写 HashMap
来源：http://uv.nicolike.cn

Go:   // 手写 map[int]int
来源：http://tp.asd995.cn

Ruby: // 手写 Hash
来源：http://ad.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qz.gzmigu.cn

[N08] 生成全排列
来源：http://kp.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://hx.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://wj.huanxung.cn

JS:   // 手写回溯递归
来源：http://xa.szxytkj.cn

TS:   // 手写回溯递归
来源：http://it.chemitech.net.cn

Java: // 手写回溯递归
来源：http://dd.lnxyls.cn

Go:   // 手写回溯递归
来源：http://wj.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://ww.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://fy.huixiangedu.cn

[N09] 栈与队列
来源：http://yz.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://la.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pl.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://za.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vg.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ld.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://td.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pn.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ei.newstarts.cn

[N10] 链表节点定义
来源：http://zn.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kl.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kh.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sx.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wf.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://iq.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ek.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xp.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kj.hahajie.cn

[N11] 二叉树中序遍历
来源：http://sz.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tw.colortex.cn

PHP:  // 手写递归函数
来源：http://lg.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sl.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ey.panjiajie.cn

Java: // 手写递归
来源：http://gh.colortex.cn

Go:   // 手写递归
来源：http://cj.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fs.newstarts.cn

C#:   // 手写递归
来源：http://zt.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ey.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cb.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qz.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zb.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ys.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qt.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://je.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uv.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pw.yuntaijiaju.cn

================================================================================
来源：http://ym.9csxet.cn

O. 并发与异步
来源：http://il.nszjky.cn

================================================================================
来源：http://wt.colortex.cn

[O01] 启动一个线程
来源：http://mm.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qa.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ab.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tt.chemitech.net.cn

TS:   // 同 JS
来源：http://bk.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://ko.hnjuh.cn

Go:   go f()
来源：http://gi.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://ll.hahajie.cn

C#:   Task.Run(() => F());
来源：http://cs.hahajie.cn

[O02] 使用线程池
来源：http://zh.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://th.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zi.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://wo.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://ml.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qh.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://au.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qc.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sm.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://fw.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://uo.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://zf.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bn.bookmarksfly.cn

TS:   // 同 JS
来源：http://ti.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://zk.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cn.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://js.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://bm.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://qc.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://ny.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vu.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://pk.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ce.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mb.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://il.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zh.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://mb.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://ax.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://nf.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ew.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://ns.521024.cn

TS:   await Promise.all(tasks)
来源：http://hb.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bp.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xg.9csxet.cn

Ruby: threads.map(&:join)
来源：http://ur.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://di.wgjwhj.cn

[O06] 使用进程池
来源：http://ca.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dr.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://so.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://ow.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://qc.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sr.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rl.bjjhwx.cn

Ruby: // fork 块
来源：http://yf.wgjwhj.cn

C#:   Parallel.For
来源：http://qx.haigaiapp.cn

================================================================================
来源：http://tr.yuntaijiaju.cn

P. 常用工具函数
来源：http://ic.huanxung.cn

================================================================================
来源：http://vf.nszjky.cn

[P01] 生成 UUID
来源：http://xy.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://jy.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nj.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://gl.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://js.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://zy.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://nw.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://cw.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://nj.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://nt.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nl.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gu.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lm.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vt.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nr.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gv.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jv.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://de.panjiajie.cn

[P03] 生成短随机字符串
来源：http://jz.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jm.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ee.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ih.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ow.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bg.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gj.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://to.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fs.panjiajie.cn

[P04] 求长度
来源：http://oe.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jp.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qk.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dn.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dj.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://aj.newstarts.cn

Go:   len(arr);  len(m)
来源：http://cl.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://ni.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://to.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://mo.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fu.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qa.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tj.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jj.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ey.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cn.newstarts.cn

Ruby: a == b
来源：http://zi.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dh.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gw.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zp.521024.cn

PHP:  if (empty($x)) {}
来源：http://ie.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ev.hahajie.cn

TS:   if (x == null) {}
来源：http://fy.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yu.nszjky.cn

Go:   if x == nil {}
来源：http://dm.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fh.yuexingan06.cn

C#:   if (x is null) {}
来源：http://op.hnjuh.cn

[P07] 防抖与节流
来源：http://ft.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jb.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://de.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ek.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sx.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hk.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uz.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tk.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mk.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://hh.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iz.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qr.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://od.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ct.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vq.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oy.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nu.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jg.huixinmuqiang.cn

================================================================================
来源：http://vn.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rl.9csxet.cn

================================================================================
来源：http://te.lnxyls.cn

[Q01] 创建表
来源：http://dz.9csxet.cn

CREATE TABLE users (
来源：http://nz.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://df.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://tk.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://uf.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pm.jianghongdianzi.cn

);
来源：http://bx.colortex.cn

[Q02] 创建带外键的表
来源：http://mh.521024.cn

CREATE TABLE orders (
来源：http://tg.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pi.newstarts.cn

user_id INT NOT NULL,
来源：http://yl.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://ph.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uo.bookmarksfly.cn

);
来源：http://wr.nszjky.cn

[Q03] 增加列
来源：http://up.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aj.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://nn.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xm.huixinmuqiang.cn

[Q05] 重命名列
来源：http://rt.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jq.panjiajie.cn

[Q06] 删除列
来源：http://gz.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mb.shxzskj.cn

[Q07] 删除表
来源：http://to.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://fw.bjjhwx.cn

[Q08] 创建普通索引
来源：http://nu.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pz.hnjuh.cn

[Q09] 创建唯一索引
来源：http://zp.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xn.colortex.cn

[Q10] 插入单行
来源：http://ps.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wz.hahajie.cn

[Q11] 一次插入多行
来源：http://qb.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wg.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://dh.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gx.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mg.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://cl.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sg.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://og.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cg.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uz.huanxung.cn

[Q15] 查询全部
来源：http://ce.colortex.cn

SELECT * FROM users;
来源：http://kq.shxzskj.cn

[Q16] 查询指定列
来源：http://yn.hnjuh.cn

SELECT id, name FROM users;
来源：http://cu.jianghongdianzi.cn

[Q17] 条件查询
来源：http://ze.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://au.bjjhwx.cn

[Q18] 模糊匹配
来源：http://dm.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pa.szxytkj.cn

[Q19] 范围查询
来源：http://vo.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tw.521024.cn

[Q20] IN 列表
来源：http://kw.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sy.521024.cn

[Q21] 空值判断
来源：http://zs.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lw.colortex.cn

[Q22] 排序
来源：http://lj.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wl.chemitech.net.cn

[Q23] 分页
来源：http://ar.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mf.bookmarksfly.cn

[Q24] 去重
来源：http://yw.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://hp.panjiajie.cn

[Q25] 只取前 N 条
来源：http://iu.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rh.nszjky.cn

[Q26] 计数
来源：http://oj.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://cr.szsharing.cn

[Q27] 条件计数
来源：http://dw.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qf.shxzskj.cn

[Q28] 求和与平均
来源：http://ri.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rx.nszjky.cn

[Q29] 最大最小值
来源：http://ca.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vr.nszjky.cn

[Q30] 分组统计
来源：http://jw.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fr.yuexingan06.cn

[Q31] 分组后过滤
来源：http://ka.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://md.9csxet.cn

[Q32] 分组拼接字符串
来源：http://ec.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sa.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pv.bookmarksfly.cn

[Q33] 多列分组
来源：http://tg.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yo.szxytkj.cn

[Q34] 每组取第一条
来源：http://uk.shtwfgs.cn

SELECT * FROM (
来源：http://jo.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eh.hnjuh.cn

) t WHERE rn = 1;
来源：http://sn.hahajie.cn

[Q35] 内连接
来源：http://uw.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jv.muxihuayi.cn

[Q36] 左连接
来源：http://dt.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zj.shxzskj.cn

[Q37] 右连接
来源：http://us.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fb.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gs.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zy.colortex.cn

[Q39] 自连接（查上下级）
来源：http://zl.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://an.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kn.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qb.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zf.huixinmuqiang.cn

[Q41] 多表连接
来源：http://mr.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zt.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://qa.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://ps.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://ao.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://xm.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://da.colortex.cn

[Q43] 标量子查询
来源：http://js.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://se.nszjky.cn


<!-- 参考信息 -->