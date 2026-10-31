代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nq.9csxet.cn

[N06] 判断回文字符串
来源：http://pb.jctech888.com.cn

Py:   s == s[::-1]
来源：http://xx.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://vn.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://cf.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://ve.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cm.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://il.lnxyls.cn

Ruby: s == s.reverse
来源：http://tv.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nc.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://td.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lo.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ks.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ai.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://en.asd995.cn

Java: // 手写 HashMap
来源：http://um.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://pk.szxytkj.cn

Ruby: // 手写 Hash
来源：http://bf.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ko.hahajie.cn

[N08] 生成全排列
来源：http://ax.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://nr.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://sx.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://da.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://ku.szxytkj.cn

Java: // 手写回溯递归
来源：http://cr.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://ks.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://uo.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://rs.wgjwhj.cn

[N09] 栈与队列
来源：http://ca.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uh.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://st.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sd.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://su.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yo.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ag.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://si.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lo.asd995.cn

[N10] 链表节点定义
来源：http://fh.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kn.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zq.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vp.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pz.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://hq.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ad.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mt.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yc.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://fq.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wh.colortex.cn

PHP:  // 手写递归函数
来源：http://sv.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://no.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nh.hahajie.cn

Java: // 手写递归
来源：http://zc.bookmarksfly.cn

Go:   // 手写递归
来源：http://ts.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ql.newstarts.cn

C#:   // 手写递归
来源：http://pp.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oo.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ke.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vq.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oc.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vo.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rf.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://on.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ix.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oo.chemitech.net.cn

================================================================================
来源：http://rh.hahajie.cn

O. 并发与异步
来源：http://ff.9csxet.cn

================================================================================
来源：http://gq.huixiangedu.cn

[O01] 启动一个线程
来源：http://kd.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uz.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ou.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vg.bookmarksfly.cn

TS:   // 同 JS
来源：http://og.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://el.yuexingan06.cn

Go:   go f()
来源：http://oz.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://fc.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://aj.colortex.cn

[O02] 使用线程池
来源：http://rx.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cf.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uu.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://da.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://lt.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nq.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wo.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://om.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uj.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://aj.shxzskj.cn

Py:   with lock: shared += 1
来源：http://id.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ae.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pm.hahajie.cn

TS:   // 同 JS
来源：http://qp.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://rz.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sk.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tp.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://st.9csxet.cn

[O04] 定义异步函数并等待
来源：http://fc.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://sa.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xa.szsharing.cn

JS:   async function f() { await g(); }
来源：http://xy.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xz.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rx.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mc.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cp.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://hp.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://mg.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://fe.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zj.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://oo.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://be.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://je.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://me.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://tt.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sd.hahajie.cn

[O06] 使用进程池
来源：http://yj.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mb.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ne.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://yh.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://sg.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uk.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yj.haigaiapp.cn

Ruby: // fork 块
来源：http://zr.yuntaijiaju.cn

C#:   Parallel.For
来源：http://dx.chemitech.net.cn

================================================================================
来源：http://gw.wgjwhj.cn

P. 常用工具函数
来源：http://iw.hahajie.cn

================================================================================
来源：http://we.bjjhwx.cn

[P01] 生成 UUID
来源：http://qj.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://ir.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zz.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://ws.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://kh.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://qz.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://gs.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://zh.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://zx.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://cx.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ml.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rl.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jk.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://up.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xi.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gw.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rj.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vx.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://oo.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sh.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pp.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rd.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://us.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://in.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ov.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fg.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uf.bjjhwx.cn

[P04] 求长度
来源：http://hg.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ix.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kf.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lm.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nz.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://lx.huanxung.cn

Go:   len(arr);  len(m)
来源：http://cv.newstarts.cn

Ruby: x.length;  x.size
来源：http://kv.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bj.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://nq.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ni.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ry.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xb.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://em.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gr.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qv.lnxyls.cn

Ruby: a == b
来源：http://bv.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ek.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://id.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xa.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://wg.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://br.gzmigu.cn

TS:   if (x == null) {}
来源：http://ne.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ca.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://kn.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rh.hnjuh.cn

C#:   if (x is null) {}
来源：http://eb.hahajie.cn

[P07] 防抖与节流
来源：http://yj.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tu.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://dt.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ra.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xh.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nn.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qh.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://om.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zy.hahajie.cn

[P08] 处理浮点精度问题
来源：http://ud.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jp.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xz.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ig.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lk.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zd.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xm.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qd.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ws.shxzukj.cn

================================================================================
来源：http://ia.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ha.yuntaijiaju.cn

================================================================================
来源：http://sw.chemitech.net.cn

[Q01] 创建表
来源：http://cx.shxzskj.cn

CREATE TABLE users (
来源：http://sm.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rx.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://iq.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://wu.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sr.nicolike.cn

);
来源：http://zs.szxytkj.cn

[Q02] 创建带外键的表
来源：http://rk.jctech888.com.cn

CREATE TABLE orders (
来源：http://mx.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wx.hahajie.cn

user_id INT NOT NULL,
来源：http://ll.szsharing.cn

amount DECIMAL(10, 2),
来源：http://sz.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jy.shxzskj.cn

);
来源：http://fe.jianghongdianzi.cn

[Q03] 增加列
来源：http://ju.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fo.huanxung.cn

[Q04] 修改列类型
来源：http://hc.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://me.newstarts.cn

[Q05] 重命名列
来源：http://dn.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zj.bookmarksfly.cn

[Q06] 删除列
来源：http://ku.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ix.colortex.cn

[Q07] 删除表
来源：http://zk.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://jn.yuexingan06.cn

[Q08] 创建普通索引
来源：http://ne.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qu.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://gg.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qk.szxytkj.cn

[Q10] 插入单行
来源：http://gx.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uu.panjiajie.cn

[Q11] 一次插入多行
来源：http://pr.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uk.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://hb.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ss.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uc.9csxet.cn

[Q13] 忽略重复插入
来源：http://rj.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bh.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://kf.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mn.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dh.9csxet.cn

[Q15] 查询全部
来源：http://iv.hahajie.cn

SELECT * FROM users;
来源：http://go.colortex.cn

[Q16] 查询指定列
来源：http://jy.521024.cn

SELECT id, name FROM users;
来源：http://as.yuntaijiaju.cn

[Q17] 条件查询
来源：http://ny.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cr.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://ab.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zu.huanxung.cn

[Q19] 范围查询
来源：http://fl.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ul.shxzukj.cn

[Q20] IN 列表
来源：http://vo.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rv.huixinmuqiang.cn

[Q21] 空值判断
来源：http://fm.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qj.nicolike.cn

[Q22] 排序
来源：http://pr.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nn.shxzukj.cn

[Q23] 分页
来源：http://bx.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nz.haigaiapp.cn

[Q24] 去重
来源：http://ac.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://ib.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://mw.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wp.panjiajie.cn

[Q26] 计数
来源：http://bp.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://sw.521024.cn

[Q27] 条件计数
来源：http://sf.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://la.shxzskj.cn

[Q28] 求和与平均
来源：http://gg.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lr.wgjwhj.cn

[Q29] 最大最小值
来源：http://jq.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fv.shxzukj.cn

[Q30] 分组统计
来源：http://ff.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ii.szxytkj.cn

[Q31] 分组后过滤
来源：http://kg.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uf.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://ps.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ze.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jr.shxzskj.cn

[Q33] 多列分组
来源：http://jz.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tx.521024.cn

[Q34] 每组取第一条
来源：http://na.nszjky.cn

SELECT * FROM (
来源：http://ct.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ev.lnxyls.cn

) t WHERE rn = 1;
来源：http://ld.gzmigu.cn

[Q35] 内连接
来源：http://op.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ig.huanxung.cn

[Q36] 左连接
来源：http://wu.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hu.lnxyls.cn

[Q37] 右连接
来源：http://rf.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zi.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lr.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qn.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://wg.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ye.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ox.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yy.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ap.huanxung.cn

[Q41] 多表连接
来源：http://hy.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rf.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://ki.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://ge.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://qb.9csxet.cn


<!-- 参考信息 -->