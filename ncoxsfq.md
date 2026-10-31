代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://al.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lm.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ao.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://el.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hh.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dr.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sp.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pn.panjiajie.cn

[N05] 最大公约数
来源：http://si.hahajie.cn

Py:   math.gcd(a, b)
来源：http://xh.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rg.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sy.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zj.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pi.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sg.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://xn.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rn.521024.cn

[N06] 判断回文字符串
来源：http://li.haigaiapp.cn

Py:   s == s[::-1]
来源：http://ia.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://eo.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://va.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://at.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qy.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://rp.szxytkj.cn

Ruby: s == s.reverse
来源：http://ls.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ex.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://qr.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dp.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lk.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bt.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://ok.haigaiapp.cn

Java: // 手写 HashMap
来源：http://my.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://os.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://td.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yu.lnxyls.cn

[N08] 生成全排列
来源：http://hl.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://in.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://nb.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://as.521024.cn

TS:   // 手写回溯递归
来源：http://xf.panjiajie.cn

Java: // 手写回溯递归
来源：http://sb.hahajie.cn

Go:   // 手写回溯递归
来源：http://gk.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://oy.asd995.cn

C#:   // 手写回溯递归
来源：http://ml.chemitech.net.cn

[N09] 栈与队列
来源：http://dr.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lm.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zt.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oc.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sx.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uk.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yq.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://at.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aq.asd995.cn

[N10] 链表节点定义
来源：http://sn.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://im.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yl.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ve.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ko.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://nd.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ad.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jq.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://co.521024.cn

[N11] 二叉树中序遍历
来源：http://jg.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vi.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://pg.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vv.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qn.huanxung.cn

Java: // 手写递归
来源：http://qw.9csxet.cn

Go:   // 手写递归
来源：http://jv.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gd.muxihuayi.cn

C#:   // 手写递归
来源：http://hy.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wt.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ii.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://np.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xq.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tz.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oq.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zy.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://em.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://od.hnjuh.cn

================================================================================
来源：http://ko.bookmarksfly.cn

O. 并发与异步
来源：http://kj.huanxung.cn

================================================================================
来源：http://xi.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://rx.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ie.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://if.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xw.huixiangedu.cn

TS:   // 同 JS
来源：http://xi.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://rg.bjjhwx.cn

Go:   go f()
来源：http://qi.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://yb.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://tl.yuntaijiaju.cn

[O02] 使用线程池
来源：http://wj.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vg.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wb.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://eq.nszjky.cn

TS:   // worker_threads 线程池
来源：http://bd.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://za.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ij.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xm.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zf.521024.cn

[O03] 加锁保护共享数据
来源：http://tj.colortex.cn

Py:   with lock: shared += 1
来源：http://ly.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://nc.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lo.shxzskj.cn

TS:   // 同 JS
来源：http://yv.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://jt.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dr.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ac.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://py.newstarts.cn

[O04] 定义异步函数并等待
来源：http://kd.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://mx.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kn.colortex.cn

JS:   async function f() { await g(); }
来源：http://wn.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rh.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ez.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ut.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fg.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://jz.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://bs.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://fp.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://is.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://qo.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://rn.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://as.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ki.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://gf.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mk.colortex.cn

[O06] 使用进程池
来源：http://kw.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wf.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ef.colortex.cn

JS:   // child_process / cluster 模块
来源：http://qi.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://mu.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xb.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nl.gzmigu.cn

Ruby: // fork 块
来源：http://hf.gzmigu.cn

C#:   Parallel.For
来源：http://ms.szxytkj.cn

================================================================================
来源：http://ki.newstarts.cn

P. 常用工具函数
来源：http://oz.shxzskj.cn

================================================================================
来源：http://hu.jctech888.com.cn

[P01] 生成 UUID
来源：http://zo.colortex.cn

Py:   str(uuid.uuid4())
来源：http://qz.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ws.9csxet.cn

JS:   crypto.randomUUID()
来源：http://xs.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://yi.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://im.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://jm.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://hh.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://kr.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://hq.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rz.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ut.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ef.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gb.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tg.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vj.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fm.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jz.colortex.cn

[P03] 生成短随机字符串
来源：http://ae.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zo.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nt.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sg.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wy.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vk.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uv.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bu.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://md.huixiangedu.cn

[P04] 求长度
来源：http://ph.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zz.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oq.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ez.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hg.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://qr.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://tz.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://ak.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rb.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://om.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jg.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ag.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rl.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://id.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ek.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tx.521024.cn

Ruby: a == b
来源：http://uk.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xi.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bj.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yh.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://yg.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fx.wgjwhj.cn

TS:   if (x == null) {}
来源：http://dv.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fs.wgjwhj.cn

Go:   if x == nil {}
来源：http://kf.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xo.szsharing.cn

C#:   if (x is null) {}
来源：http://us.szsharing.cn

[P07] 防抖与节流
来源：http://yq.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tr.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://nn.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ts.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vj.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sl.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ef.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://il.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lt.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://le.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ht.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jt.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://di.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rh.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://po.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yn.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lm.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qv.shtwfgs.cn

================================================================================
来源：http://hm.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wy.521024.cn

================================================================================
来源：http://iz.yuntaijiaju.cn

[Q01] 创建表
来源：http://sw.szsharing.cn

CREATE TABLE users (
来源：http://oh.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://di.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://ow.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://kl.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cc.bookmarksfly.cn

);
来源：http://rk.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://kh.yuexingan06.cn

CREATE TABLE orders (
来源：http://ro.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xn.gzmigu.cn

user_id INT NOT NULL,
来源：http://qg.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://ge.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jy.9csxet.cn

);
来源：http://ar.bjjhwx.cn

[Q03] 增加列
来源：http://yl.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wm.bookmarksfly.cn

[Q04] 修改列类型
来源：http://el.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hu.shxzukj.cn

[Q05] 重命名列
来源：http://am.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cg.shxzukj.cn

[Q06] 删除列
来源：http://ki.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kj.gzmigu.cn

[Q07] 删除表
来源：http://sd.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://br.gzmigu.cn

[Q08] 创建普通索引
来源：http://vf.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cm.szxytkj.cn

[Q09] 创建唯一索引
来源：http://ds.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yo.bjjhwx.cn

[Q10] 插入单行
来源：http://vg.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lq.newstarts.cn

[Q11] 一次插入多行
来源：http://gg.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hj.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://by.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ae.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pj.9csxet.cn

[Q13] 忽略重复插入
来源：http://kw.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://id.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://js.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fy.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mw.hnjuh.cn

[Q15] 查询全部
来源：http://uy.szsharing.cn

SELECT * FROM users;
来源：http://hs.yuexingan06.cn

[Q16] 查询指定列
来源：http://lm.shxzukj.cn

SELECT id, name FROM users;
来源：http://yt.haigaiapp.cn

[Q17] 条件查询
来源：http://io.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vb.jctech888.com.cn

[Q18] 模糊匹配
来源：http://mf.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xz.nicolike.cn

[Q19] 范围查询
来源：http://zb.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gx.huanxung.cn

[Q20] IN 列表
来源：http://kp.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pv.gzmigu.cn

[Q21] 空值判断
来源：http://mb.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bz.szsharing.cn

[Q22] 排序
来源：http://eh.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://za.newstarts.cn

[Q23] 分页
来源：http://gn.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nt.huixinmuqiang.cn

[Q24] 去重
来源：http://ec.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://ps.szsharing.cn

[Q25] 只取前 N 条
来源：http://td.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xa.szsharing.cn

[Q26] 计数
来源：http://tc.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://vt.shxzskj.cn

[Q27] 条件计数
来源：http://mp.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ao.shtwfgs.cn

[Q28] 求和与平均
来源：http://eh.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lg.colortex.cn

[Q29] 最大最小值
来源：http://vz.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rk.shtwfgs.cn

[Q30] 分组统计
来源：http://lu.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bu.shtwfgs.cn

[Q31] 分组后过滤
来源：http://xy.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://et.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://gb.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vc.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://te.lnxyls.cn

[Q33] 多列分组
来源：http://rs.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wc.lnxyls.cn

[Q34] 每组取第一条
来源：http://by.jctech888.com.cn

SELECT * FROM (
来源：http://kv.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gp.yuexingan06.cn

) t WHERE rn = 1;
来源：http://tk.nicolike.cn

[Q35] 内连接
来源：http://ms.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rd.521024.cn


<!-- 参考信息 -->