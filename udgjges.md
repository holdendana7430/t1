代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xk.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qt.szxytkj.cn

Ruby: a.gcd(b)
来源：http://vi.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gh.yuexingan06.cn

[N06] 判断回文字符串
来源：http://dd.gzmigu.cn

Py:   s == s[::-1]
来源：http://cu.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://vg.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://wc.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://to.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nk.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://ky.hnjuh.cn

Ruby: s == s.reverse
来源：http://qq.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bo.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://bu.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qg.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rh.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kg.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://rx.shtwfgs.cn

Java: // 手写 HashMap
来源：http://fp.9csxet.cn

Go:   // 手写 map[int]int
来源：http://lw.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://hn.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zl.szxytkj.cn

[N08] 生成全排列
来源：http://rt.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://ij.521024.cn

PHP:  // 手写递归交换
来源：http://jh.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://jr.gzmigu.cn

TS:   // 手写回溯递归
来源：http://xs.szsharing.cn

Java: // 手写回溯递归
来源：http://zf.huanxung.cn

Go:   // 手写回溯递归
来源：http://cn.asd995.cn

Ruby: arr.permutation.to_a
来源：http://yn.colortex.cn

C#:   // 手写回溯递归
来源：http://vm.colortex.cn

[N09] 栈与队列
来源：http://oj.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://el.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lg.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qw.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xv.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ed.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qd.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fb.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yr.wgjwhj.cn

[N10] 链表节点定义
来源：http://tu.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oe.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yw.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hp.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vh.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://sz.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ac.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dt.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://th.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://et.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ok.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://he.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://no.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dz.asd995.cn

Java: // 手写递归
来源：http://sz.521024.cn

Go:   // 手写递归
来源：http://co.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dg.bookmarksfly.cn

C#:   // 手写递归
来源：http://wd.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xx.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://la.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pf.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kb.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ah.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ww.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hc.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ji.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yo.huanxung.cn

================================================================================
来源：http://bn.haigaiapp.cn

O. 并发与异步
来源：http://ly.newstarts.cn

================================================================================
来源：http://ck.szxytkj.cn

[O01] 启动一个线程
来源：http://fa.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nz.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qz.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.huanxung.cn

TS:   // 同 JS
来源：http://aa.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://gj.lnxyls.cn

Go:   go f()
来源：http://rh.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://qg.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://qt.huixinmuqiang.cn

[O02] 使用线程池
来源：http://kr.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ho.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rk.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://rf.huanxung.cn

TS:   // worker_threads 线程池
来源：http://hj.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rn.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ed.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mz.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gi.szsharing.cn

[O03] 加锁保护共享数据
来源：http://yy.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://tl.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://gi.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ru.bjjhwx.cn

TS:   // 同 JS
来源：http://fq.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://ed.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rs.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oc.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://ep.szsharing.cn

[O04] 定义异步函数并等待
来源：http://pt.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://cu.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rr.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://tp.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://or.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jc.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gz.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ac.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://ec.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://yj.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://dj.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uy.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://rk.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://wr.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lu.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wx.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://pe.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://re.szxytkj.cn

[O06] 使用进程池
来源：http://ej.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wy.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cp.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://qo.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://ck.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ra.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://os.huanxung.cn

Ruby: // fork 块
来源：http://nj.yuexingan06.cn

C#:   Parallel.For
来源：http://oc.shxzskj.cn

================================================================================
来源：http://tm.bookmarksfly.cn

P. 常用工具函数
来源：http://se.haigaiapp.cn

================================================================================
来源：http://wx.9csxet.cn

[P01] 生成 UUID
来源：http://qm.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://gl.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://di.nszjky.cn

JS:   crypto.randomUUID()
来源：http://lx.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://hi.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://sn.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://ii.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://hs.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://om.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://pq.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hm.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pk.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gf.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kz.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yy.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rk.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://it.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fb.szsharing.cn

[P03] 生成短随机字符串
来源：http://sl.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cb.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qc.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pd.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ru.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uh.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uo.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pf.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hh.yuexingan06.cn

[P04] 求长度
来源：http://yf.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vo.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xl.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qc.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eb.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://vp.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://vk.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://ip.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mf.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://az.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xr.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qp.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hu.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jc.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dj.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cq.jctech888.com.cn

Ruby: a == b
来源：http://is.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://km.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://me.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jx.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://pw.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cf.szxytkj.cn

TS:   if (x == null) {}
来源：http://xl.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ch.hnjuh.cn

Go:   if x == nil {}
来源：http://kh.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ah.huanxung.cn

C#:   if (x is null) {}
来源：http://ho.nszjky.cn

[P07] 防抖与节流
来源：http://pf.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pb.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://qi.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://at.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sf.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mq.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hd.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gy.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://of.521024.cn

[P08] 处理浮点精度问题
来源：http://eh.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ej.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qt.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ie.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ny.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yl.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://in.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rh.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ub.hahajie.cn

================================================================================
来源：http://nz.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cw.hahajie.cn

================================================================================
来源：http://od.gzmigu.cn

[Q01] 创建表
来源：http://wt.huixinmuqiang.cn

CREATE TABLE users (
来源：http://qz.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gh.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://rp.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://ur.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://av.szsharing.cn

);
来源：http://uv.szsharing.cn

[Q02] 创建带外键的表
来源：http://sa.chemitech.net.cn

CREATE TABLE orders (
来源：http://rl.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qs.nicolike.cn

user_id INT NOT NULL,
来源：http://ig.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://st.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://js.yuexingan06.cn

);
来源：http://iv.bjjhwx.cn

[Q03] 增加列
来源：http://lc.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xy.wgjwhj.cn

[Q04] 修改列类型
来源：http://no.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://la.gzmigu.cn

[Q05] 重命名列
来源：http://lj.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jn.szxytkj.cn

[Q06] 删除列
来源：http://ab.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lb.muxihuayi.cn

[Q07] 删除表
来源：http://hs.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://ea.muxihuayi.cn

[Q08] 创建普通索引
来源：http://fv.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://on.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://gh.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uq.hahajie.cn

[Q10] 插入单行
来源：http://je.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ip.shtwfgs.cn

[Q11] 一次插入多行
来源：http://ha.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://za.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://df.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sn.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yu.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://wv.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rn.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://va.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ud.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zn.bjjhwx.cn

[Q15] 查询全部
来源：http://um.shxzukj.cn

SELECT * FROM users;
来源：http://iw.muxihuayi.cn

[Q16] 查询指定列
来源：http://hs.nicolike.cn

SELECT id, name FROM users;
来源：http://hq.521024.cn

[Q17] 条件查询
来源：http://fk.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ud.szxytkj.cn

[Q18] 模糊匹配
来源：http://yv.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ww.colortex.cn

[Q19] 范围查询
来源：http://uc.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vg.muxihuayi.cn

[Q20] IN 列表
来源：http://gb.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qj.haigaiapp.cn

[Q21] 空值判断
来源：http://pg.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ha.huanxung.cn

[Q22] 排序
来源：http://lo.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sx.huanxung.cn

[Q23] 分页
来源：http://wf.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zm.nicolike.cn

[Q24] 去重
来源：http://cb.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://mj.nicolike.cn

[Q25] 只取前 N 条
来源：http://oz.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mh.szsharing.cn

[Q26] 计数
来源：http://bm.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://cc.521024.cn

[Q27] 条件计数
来源：http://wc.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wk.bjjhwx.cn

[Q28] 求和与平均
来源：http://gb.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vu.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://kj.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ep.hnjuh.cn

[Q30] 分组统计
来源：http://lz.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ff.9csxet.cn

[Q31] 分组后过滤
来源：http://rg.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dh.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://kr.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rl.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hj.bjjhwx.cn

[Q33] 多列分组
来源：http://hv.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yn.hahajie.cn

[Q34] 每组取第一条
来源：http://yi.yuexingan06.cn

SELECT * FROM (
来源：http://sw.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qu.huanxung.cn

) t WHERE rn = 1;
来源：http://ad.jctech888.com.cn

[Q35] 内连接
来源：http://rq.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rt.huixinmuqiang.cn

[Q36] 左连接
来源：http://rm.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nk.jctech888.com.cn

[Q37] 右连接
来源：http://sc.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pc.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oe.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eg.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://ti.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://go.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ap.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rs.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vn.panjiajie.cn

[Q41] 多表连接
来源：http://jr.9csxet.cn


<!-- 参考信息 -->