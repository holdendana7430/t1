代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxcswwu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rksovvxn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xjeoseez.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kvbdzkkk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xerktrum.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rjnllewe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vddtytqo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bvukzckh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kcbtqkjv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tnlhpoft.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lzmxabct.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fogydjfx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3swvmwdtr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uocxosnz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ivszzgew.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ojxsxtyj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3drxacewq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hatuemkm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xggpxgli.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3luezjbqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgqjpsuq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ybtpltgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jadtkqcg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ojrovkxu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jgbylelg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tuoohokp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3puydnbhf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rweqnijt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jjkdrmav.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yezpnmvr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3aouutvpg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3htqdlxhs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ksqarhke.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3uxvxcfhk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3etigrenx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fobifryf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ynphguxc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ogjdddrd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nryivqtd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kakxseqd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lomfvinp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zzqqftez.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxbxertm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fggpmeqo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3oomcgucz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3othidbah.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqazkdnp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ruvyammu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iittrgtz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3arbggzba.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mjvmuskm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bkxoobnm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yzzdomrr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rcuowlfe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3feuoibxd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yjwcxrea.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nuqqszoy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3chilwone.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pqpovxxj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mkkqkybn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3itfyqofw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3szfadwqs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lyedccwk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rdylamef.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lvgzjyzs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ikezllta.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ifkfzhrg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3flrcruwh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nekhualg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ogguhjhk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3sljijdpt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pzynacns.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bqdkmktp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3abnmujbs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3lalmptio.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mnxiovrb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jljkljua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfkzkrrj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqaaunvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwbpcweq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cdnjzbqn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lmkcjuwq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hlbyjhdx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3odqnpxcz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oifyzqho.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nhaxtppg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ekbsuasd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nbqtrfry.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oswkmmvx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dbhingve.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ayenwoki.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qawqnbpa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mvbnyubg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3yvurszuc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3blzcdckq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zcrkwudk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mgglpgae.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yjskwwya.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tqnuzuaf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3eabilmla.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tyelieqx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yvdifcvw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3osnwudwt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rijhbtle.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ohljpjxg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3urobgxwd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3yskvtulg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vzczgude.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qjzvomzp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3exnqvbwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mtigwqdk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cztukqfz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ssddfrso.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tbkkgpfw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vlbucrvq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zqjbtnyv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vozhxmdf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cotyxwdp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tyhkmkgq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jjppchua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tsppfjrd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qklfsyjc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wtqmfejb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xxkfeqrw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pgnblcma.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3axjxmnvx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cepohalt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ayjcneog.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rsaywkoy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyimjcde.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rmiafzwv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nhwxntoa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjwdzyi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsmlwikf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3haypxtyj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xboeoodx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rmhbjgyk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kgcjqfpc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cohfsvwr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3bpwmcsef.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dtmummbb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kvfycnpo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ckyzkbyi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3miqagmxs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vnhzlavn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ukumcjjq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tubtekrn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qepbotrt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3dfpoeaut.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vhboctmv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hjxezymg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jpdtvkrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgkteiyt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hiecpfko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upywgboo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dqbogrrf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fhztpkzf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nokwbaon.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mxtnhhye.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pvsrkjvb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3iunbclqn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qsjooipf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3twrmlajp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ayooybgt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fbpdjlns.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bhdnwfwg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ybcwgbja.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pggekmwi.html

);
来源：http://www.52xcode.cn/Article/details/gt3danxpvnr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ywxchvxt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kttuxjao.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qwwcpebo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hiwifnqh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3deniisxc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ejrhyodp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kyixqufh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3znrtvsdn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jczlsxko.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ewwzjakf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3cunyfxch.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bbpryaii.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3evpywvgn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3heelzxts.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jgbadajl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tbqzmdlr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wxpbhwqi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ylmtiwky.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ahwkwstv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lfnhrbop.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3hwyqxsmr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3csoknuik.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pvklryvq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3adyhceeu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3xulhnoxc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tybpogbs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vowbiegw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gstoxekp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3rpellqer.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3plcbqmeg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tezkmdss.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3thhogjec.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3brnaxkmk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hbmofcwk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mlbdgrbv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oycfdgul.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yzzfqbqr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ijhoqjqa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ibdkjgbr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pdypnbzs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3okbwiyqz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3utzincha.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vlvyqovx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dpxmyfmh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vjdedclh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgbtlwmv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pohbwlej.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nxpaxouf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ervdiwqp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wdbiqrqp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3djojcnqr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3luipulrh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wllyagfd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3slouqrax.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qpqmemlj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fuigvcam.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3osvmsdfa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fnrjejrd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gcxbgxdu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ajfpyjlb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ivmijvkn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zfzclion.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3chukbxqo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcifpizy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hjghknbe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mgkzfljq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3weevsjvf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tnfbovzs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zbnkymnk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zjvrmxdw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mbnuotee.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vtujqmst.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tvzygaqn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3whilbznz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3khjxhckl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ovwclkzx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sbjdhjtm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3runwolki.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3erugbefx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3sydtqwcw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mifqqern.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zjeralck.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fzhlqtek.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3lgkgddxd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ucwoemhk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ctpssvrl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fmnnlvzr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nquapqmg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zxwdsofa.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3etukdfgh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tfzmpwoj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hplnaxeb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ckdronmu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3bhbdybtn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3enghpenm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hrhxdkjk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3orzbkorg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hbclzayk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ceemvveb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cdgiqmpd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3eszrebtt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ilercqsy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jzzmjnwi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eybybxaz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ligsiqch.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3noqylyhc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3btkmcpod.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3eixxrwyt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3udffvyvg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iykmaimt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3erirsqpg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3quziggvv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tyzipvts.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wpaldgni.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3behbktns.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aygtwsmi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ykajnpqh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fhchntdz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fvbkdlud.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrugdxnb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3edvyfbcr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rikgwgar.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3saeiqlsl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qifunfzx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3iqruhwuy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yhqfehqo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3epjeckdd.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cobrxxiu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nufefhvh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3edwxxzlu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hjznyrro.html


<!-- 参考信息 -->