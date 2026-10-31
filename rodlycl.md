代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lr.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ti.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://op.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hf.jctech888.com.cn

[N05] 最大公约数
来源：http://bu.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://jo.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fp.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zk.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://si.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ds.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mz.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://ph.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ca.521024.cn

[N06] 判断回文字符串
来源：http://lw.521024.cn

Py:   s == s[::-1]
来源：http://gk.9csxet.cn

PHP:  $s === strrev($s);
来源：http://hu.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://zu.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://en.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ng.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://cr.hahajie.cn

Ruby: s == s.reverse
来源：http://gi.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cn.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://al.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fv.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xx.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pa.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://ss.jctech888.com.cn

Java: // 手写 HashMap
来源：http://ls.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://ot.9csxet.cn

Ruby: // 手写 Hash
来源：http://hr.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vo.shxzukj.cn

[N08] 生成全排列
来源：http://ws.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://ag.szsharing.cn

PHP:  // 手写递归交换
来源：http://oc.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://zz.newstarts.cn

TS:   // 手写回溯递归
来源：http://vf.asd995.cn

Java: // 手写回溯递归
来源：http://mb.huanxung.cn

Go:   // 手写回溯递归
来源：http://nt.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://uk.asd995.cn

C#:   // 手写回溯递归
来源：http://hj.nszjky.cn

[N09] 栈与队列
来源：http://vq.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dz.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tx.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ut.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pi.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qq.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lo.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xx.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://to.shxzukj.cn

[N10] 链表节点定义
来源：http://ws.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yz.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jo.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hs.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://br.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://do.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://je.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vb.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bi.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://jy.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cs.hahajie.cn

PHP:  // 手写递归函数
来源：http://qh.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tz.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oa.wgjwhj.cn

Java: // 手写递归
来源：http://sn.shtwfgs.cn

Go:   // 手写递归
来源：http://rn.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mp.bookmarksfly.cn

C#:   // 手写递归
来源：http://ir.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lz.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pt.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mj.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bt.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bg.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ka.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ej.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uv.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://op.lnxyls.cn

================================================================================
来源：http://fn.9csxet.cn

O. 并发与异步
来源：http://lu.hnjuh.cn

================================================================================
来源：http://gg.nszjky.cn

[O01] 启动一个线程
来源：http://hx.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kc.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fs.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tp.haigaiapp.cn

TS:   // 同 JS
来源：http://eb.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://xr.szxytkj.cn

Go:   go f()
来源：http://fc.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://zc.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://uw.asd995.cn

[O02] 使用线程池
来源：http://kn.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ql.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ph.asd995.cn

JS:   // worker_threads 线程池
来源：http://kr.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://sx.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qy.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ni.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hf.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sz.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://jm.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://lb.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://ja.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ew.chemitech.net.cn

TS:   // 同 JS
来源：http://cj.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://og.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oa.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zp.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://hy.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://rv.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://vg.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ed.9csxet.cn

JS:   async function f() { await g(); }
来源：http://le.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zu.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tj.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fc.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://et.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://gn.521024.cn

[O05] 并发执行并等待全部完成
来源：http://me.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://jv.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dv.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://ek.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://qg.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://um.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xr.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://hk.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ik.huanxung.cn

[O06] 使用进程池
来源：http://yp.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://er.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gt.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://hu.colortex.cn

TS:   // child_process / cluster 模块
来源：http://da.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dz.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://la.szsharing.cn

Ruby: // fork 块
来源：http://gz.asd995.cn

C#:   Parallel.For
来源：http://rt.szxytkj.cn

================================================================================
来源：http://sj.colortex.cn

P. 常用工具函数
来源：http://wd.chemitech.net.cn

================================================================================
来源：http://za.bjjhwx.cn

[P01] 生成 UUID
来源：http://qu.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://tm.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://id.nicolike.cn

JS:   crypto.randomUUID()
来源：http://pe.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://vs.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://xo.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://xr.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://nz.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://cm.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://os.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fd.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iq.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rl.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ms.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yh.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wm.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qq.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yd.nszjky.cn

[P03] 生成短随机字符串
来源：http://yf.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rb.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dn.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yc.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sw.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qn.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dn.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wp.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qw.panjiajie.cn

[P04] 求长度
来源：http://kq.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ye.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://om.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vc.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dn.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://xg.nicolike.cn

Go:   len(arr);  len(m)
来源：http://ev.hnjuh.cn

Ruby: x.length;  x.size
来源：http://zf.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://om.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://lh.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kw.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jr.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wj.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fa.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yi.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bm.bjjhwx.cn

Ruby: a == b
来源：http://ib.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ta.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xe.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bd.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://gk.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yc.nicolike.cn

TS:   if (x == null) {}
来源：http://fe.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ke.lnxyls.cn

Go:   if x == nil {}
来源：http://rf.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://le.newstarts.cn

C#:   if (x is null) {}
来源：http://kj.haigaiapp.cn

[P07] 防抖与节流
来源：http://dc.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vy.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://ym.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ly.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oa.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yl.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://st.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fa.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mv.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://jz.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mt.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ni.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gb.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kh.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qb.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bk.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://la.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://od.szxytkj.cn

================================================================================
来源：http://ai.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uo.nszjky.cn

================================================================================
来源：http://xp.muxihuayi.cn

[Q01] 创建表
来源：http://kn.nszjky.cn

CREATE TABLE users (
来源：http://wr.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pc.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://aq.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://ew.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yy.chemitech.net.cn

);
来源：http://lp.szxytkj.cn

[Q02] 创建带外键的表
来源：http://zg.nszjky.cn

CREATE TABLE orders (
来源：http://un.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://du.jctech888.com.cn

user_id INT NOT NULL,
来源：http://lb.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://hq.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bp.hahajie.cn

);
来源：http://nq.wgjwhj.cn

[Q03] 增加列
来源：http://sw.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xy.wgjwhj.cn

[Q04] 修改列类型
来源：http://oa.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fo.newstarts.cn

[Q05] 重命名列
来源：http://yz.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ta.chemitech.net.cn

[Q06] 删除列
来源：http://jq.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jy.huixiangedu.cn

[Q07] 删除表
来源：http://rv.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://cn.szsharing.cn

[Q08] 创建普通索引
来源：http://in.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zx.panjiajie.cn

[Q09] 创建唯一索引
来源：http://lp.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lu.9csxet.cn

[Q10] 插入单行
来源：http://zb.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nm.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://er.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ip.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://tl.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sy.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uu.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://jm.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ty.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://jq.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bd.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ce.bjjhwx.cn

[Q15] 查询全部
来源：http://iw.colortex.cn

SELECT * FROM users;
来源：http://iy.shtwfgs.cn

[Q16] 查询指定列
来源：http://ok.huixiangedu.cn

SELECT id, name FROM users;
来源：http://kw.shtwfgs.cn

[Q17] 条件查询
来源：http://co.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ts.nicolike.cn

[Q18] 模糊匹配
来源：http://uj.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://il.shxzukj.cn

[Q19] 范围查询
来源：http://xm.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fp.huixiangedu.cn

[Q20] IN 列表
来源：http://mj.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cr.9csxet.cn

[Q21] 空值判断
来源：http://uc.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tm.nicolike.cn

[Q22] 排序
来源：http://ob.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://da.huixiangedu.cn

[Q23] 分页
来源：http://px.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zp.newstarts.cn

[Q24] 去重
来源：http://ba.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://wu.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://ce.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kf.521024.cn

[Q26] 计数
来源：http://vx.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://zb.shxzukj.cn

[Q27] 条件计数
来源：http://vt.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vl.nicolike.cn

[Q28] 求和与平均
来源：http://rn.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kg.hnjuh.cn

[Q29] 最大最小值
来源：http://yl.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pi.bookmarksfly.cn

[Q30] 分组统计
来源：http://bl.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ly.shxzukj.cn

[Q31] 分组后过滤
来源：http://ka.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sc.521024.cn

[Q32] 分组拼接字符串
来源：http://yu.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vr.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rh.colortex.cn

[Q33] 多列分组
来源：http://th.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jr.nicolike.cn

[Q34] 每组取第一条
来源：http://jm.hnjuh.cn

SELECT * FROM (
来源：http://jh.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://er.asd995.cn

) t WHERE rn = 1;
来源：http://cf.shtwfgs.cn

[Q35] 内连接
来源：http://gg.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ud.huanxung.cn

[Q36] 左连接
来源：http://uo.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xf.asd995.cn

[Q37] 右连接
来源：http://td.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://al.huixinmuqiang.cn


<!-- 参考信息 -->