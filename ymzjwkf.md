代发 wailian999

[N05] 最大公约数
来源：http://xa.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://hb.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ut.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iq.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lr.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nf.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zq.gzmigu.cn

Ruby: a.gcd(b)
来源：http://eg.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yo.muxihuayi.cn

[N06] 判断回文字符串
来源：http://ga.jctech888.com.cn

Py:   s == s[::-1]
来源：http://fp.nszjky.cn

PHP:  $s === strrev($s);
来源：http://ke.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://nk.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://zq.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zp.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://dy.nicolike.cn

Ruby: s == s.reverse
来源：http://ee.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ao.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://vl.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://om.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jc.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oh.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://uf.szxytkj.cn

Java: // 手写 HashMap
来源：http://su.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://qo.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://aa.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ai.nszjky.cn

[N08] 生成全排列
来源：http://yp.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://lm.nicolike.cn

PHP:  // 手写递归交换
来源：http://vq.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://jz.szxytkj.cn

TS:   // 手写回溯递归
来源：http://cb.521024.cn

Java: // 手写回溯递归
来源：http://dp.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://cw.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://qv.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://mr.gzmigu.cn

[N09] 栈与队列
来源：http://xb.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://by.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://is.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oq.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xy.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qb.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://um.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qv.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fg.521024.cn

[N10] 链表节点定义
来源：http://ls.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pm.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ds.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pe.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ov.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://sm.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hu.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yx.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rn.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://xg.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mo.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://ys.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uy.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cz.9csxet.cn

Java: // 手写递归
来源：http://vh.9csxet.cn

Go:   // 手写递归
来源：http://vi.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ig.9csxet.cn

C#:   // 手写递归
来源：http://hq.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tp.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://es.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yy.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ag.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://da.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mv.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zl.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jm.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fg.huixinmuqiang.cn

================================================================================
来源：http://po.nicolike.cn

O. 并发与异步
来源：http://zs.hahajie.cn

================================================================================
来源：http://or.yuexingan06.cn

[O01] 启动一个线程
来源：http://fs.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wb.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lv.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dc.lnxyls.cn

TS:   // 同 JS
来源：http://vh.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://rw.gzmigu.cn

Go:   go f()
来源：http://gc.nicolike.cn

Ruby: Thread.new { f }
来源：http://bz.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://ev.panjiajie.cn

[O02] 使用线程池
来源：http://ry.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mq.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ji.521024.cn

JS:   // worker_threads 线程池
来源：http://ji.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://rs.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cb.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iu.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nt.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kq.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://vo.521024.cn

Py:   with lock: shared += 1
来源：http://qe.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://sn.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ym.shxzskj.cn

TS:   // 同 JS
来源：http://bo.521024.cn

Java: synchronized (this) { shared++; }
来源：http://pl.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ff.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xc.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://xy.hahajie.cn

[O04] 定义异步函数并等待
来源：http://mp.colortex.cn

Py:   async def f():⏎    await g()
来源：http://kd.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eo.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://jv.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pp.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sr.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ma.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ex.521024.cn

C#:   async Task F() { await G(); }
来源：http://ym.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://mo.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://lc.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ee.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://ok.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://fq.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lk.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bu.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://yo.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ho.gzmigu.cn

[O06] 使用进程池
来源：http://gd.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ep.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fn.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://gz.521024.cn

TS:   // child_process / cluster 模块
来源：http://gr.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sr.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jc.newstarts.cn

Ruby: // fork 块
来源：http://bs.huanxung.cn

C#:   Parallel.For
来源：http://gn.bjjhwx.cn

================================================================================
来源：http://hp.wgjwhj.cn

P. 常用工具函数
来源：http://cx.chemitech.net.cn

================================================================================
来源：http://td.newstarts.cn

[P01] 生成 UUID
来源：http://tm.asd995.cn

Py:   str(uuid.uuid4())
来源：http://zm.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fz.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://dc.521024.cn

TS:   crypto.randomUUID()
来源：http://sz.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://gf.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://sa.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://ix.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://qs.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://ws.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vt.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ua.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rv.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aw.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wi.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oo.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ve.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bv.newstarts.cn

[P03] 生成短随机字符串
来源：http://or.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cg.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ja.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rn.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ld.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zr.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vz.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://by.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zy.huixinmuqiang.cn

[P04] 求长度
来源：http://li.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qf.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hv.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sq.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wc.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://uh.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://jy.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://ij.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uj.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://yb.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xg.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xl.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ur.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tl.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pn.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eu.521024.cn

Ruby: a == b
来源：http://aa.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vd.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fj.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bc.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://kz.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pd.shxzukj.cn

TS:   if (x == null) {}
来源：http://wy.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rj.haigaiapp.cn

Go:   if x == nil {}
来源：http://xc.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zm.nszjky.cn

C#:   if (x is null) {}
来源：http://eg.wgjwhj.cn

[P07] 防抖与节流
来源：http://bm.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tc.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://nd.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ve.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rs.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vu.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cn.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lm.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bt.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://sj.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kc.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kc.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ua.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nx.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wl.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mf.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bd.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wn.huanxung.cn

================================================================================
来源：http://mm.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zn.hahajie.cn

================================================================================
来源：http://sv.chemitech.net.cn

[Q01] 创建表
来源：http://gv.shtwfgs.cn

CREATE TABLE users (
来源：http://kv.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://be.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://kx.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://va.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://js.shxzskj.cn

);
来源：http://qa.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://wl.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://hj.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://er.panjiajie.cn

user_id INT NOT NULL,
来源：http://gu.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://wn.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nk.lnxyls.cn

);
来源：http://jr.huanxung.cn

[Q03] 增加列
来源：http://wd.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kk.shxzskj.cn

[Q04] 修改列类型
来源：http://cr.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ww.9csxet.cn

[Q05] 重命名列
来源：http://mo.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hx.yuexingan06.cn

[Q06] 删除列
来源：http://rk.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xg.lnxyls.cn

[Q07] 删除表
来源：http://to.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://og.wgjwhj.cn

[Q08] 创建普通索引
来源：http://no.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nv.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://aw.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pb.asd995.cn

[Q10] 插入单行
来源：http://bj.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kc.hnjuh.cn

[Q11] 一次插入多行
来源：http://fb.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://en.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://hc.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qo.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pn.nicolike.cn

[Q13] 忽略重复插入
来源：http://rk.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bl.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://oe.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ru.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oi.shxzskj.cn

[Q15] 查询全部
来源：http://bv.jianghongdianzi.cn

SELECT * FROM users;
来源：http://gs.shxzskj.cn

[Q16] 查询指定列
来源：http://fo.wgjwhj.cn

SELECT id, name FROM users;
来源：http://is.yuexingan06.cn

[Q17] 条件查询
来源：http://wz.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bc.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://tl.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jp.szxytkj.cn

[Q19] 范围查询
来源：http://ru.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dj.chemitech.net.cn

[Q20] IN 列表
来源：http://bh.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pw.shxzukj.cn

[Q21] 空值判断
来源：http://wj.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zq.chemitech.net.cn

[Q22] 排序
来源：http://vy.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xu.521024.cn

[Q23] 分页
来源：http://bm.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mw.jianghongdianzi.cn

[Q24] 去重
来源：http://qj.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://zd.asd995.cn

[Q25] 只取前 N 条
来源：http://ap.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://id.nicolike.cn

[Q26] 计数
来源：http://zp.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://wg.huixiangedu.cn

[Q27] 条件计数
来源：http://qg.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gz.shxzskj.cn

[Q28] 求和与平均
来源：http://lm.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jc.jctech888.com.cn

[Q29] 最大最小值
来源：http://ip.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wg.wgjwhj.cn

[Q30] 分组统计
来源：http://ed.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cy.panjiajie.cn

[Q31] 分组后过滤
来源：http://db.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uz.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://ya.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dz.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://em.haigaiapp.cn

[Q33] 多列分组
来源：http://eg.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rr.nszjky.cn

[Q34] 每组取第一条
来源：http://we.huixinmuqiang.cn

SELECT * FROM (
来源：http://qn.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://el.newstarts.cn

) t WHERE rn = 1;
来源：http://kz.jctech888.com.cn

[Q35] 内连接
来源：http://ev.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://za.9csxet.cn

[Q36] 左连接
来源：http://hc.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wz.wgjwhj.cn

[Q37] 右连接
来源：http://cc.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nc.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nx.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wb.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://vl.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vn.haigaiapp.cn


<!-- 参考信息 -->