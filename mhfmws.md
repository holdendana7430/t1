代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3trqnrmim.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3srkboxoz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xwhpsqit.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3skgazvke.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lahkzxfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ekneprve.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3avravyum.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3losahdgo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljwchuic.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3wogcnnvy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ibtnhyla.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gqstfkfq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ywmgetcn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oxflmees.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oldozqsw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lgviixin.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lhcjxiyh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hypnszod.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ixvhxfbu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3czvuzale.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmxwxwsp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ypeyxpjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3styamqqy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3enfvpnym.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mtytdmte.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ngqhjdfe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rstkydcp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qxvalrcr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gezaeziy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ctjysyww.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xjvvdnaj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jeduzvsy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cnvqvgop.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ngmhqqpy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bzcwxteu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3conqglxt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mswlzqdb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vgljvugx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3asibufcn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rkaxojur.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3scmtvdkh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3apakhndc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjyqhmuv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3iougmjpg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jnywmrjy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fvdpqxad.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tfmkpxsi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3sxtkytjm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3igogjckn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wzjojgic.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3shacdunh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3csdjlemb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3sdlaqdwd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vhxhmwrd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pikpuqyz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qnwoathx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cmxconur.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3bxwwcauh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcjkvjof.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pqyllotb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3piszmtuj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3peyhtjxr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lzhtmnel.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mvigpmmq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gdwipeby.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hfteuacn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yprrxqto.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zesndlis.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lqtbmoms.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sujukmoe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cwnqdhiw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eauynwww.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vbsewehc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ktaliowq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ngsagpbi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3eunetqok.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yuoxjfpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oytvxjsh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lhxeovnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmsvmizf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gvgxtotj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3arvvkpkx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3frruvyps.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3snxtgrpi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qupgtkwm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ubhgnxav.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zaxmtspz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fwrogxsq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xrlvufbk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vsyeqnru.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hheccqvp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvvcivdz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3uvhpblng.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yituwpfg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3muzyhdgh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qsamwehd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wuhpyuqo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tulugakp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lqspeduf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ygldkpob.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3phvbunqs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rderciwr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fffumkdi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3hqmnjlsx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dentoywr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dwlzqibc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nqchtica.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rhyphsad.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3golqxckd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lpbvsnrx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nlaksvza.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qoakrvsa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wsamlfup.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3slkcaaep.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3yiglxlvs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3blutkdds.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yfxljmyi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wtzivdrr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ldineoxs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3evhgpeck.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3saryhxnl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3pbygigkm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tsoudcgv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nqfhfytk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rjjwjojk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rsrpfbjr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ggoizdti.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tyrnyihn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pdjzvaiq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbdjzgxv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ldctjifo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ghgtspbj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3oinfyrbi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdkmtcvq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rtlkzent.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3yetfkbze.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3chasevqj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3haimrthe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cmosbcux.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rkvvldca.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3cjxkdfne.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lprkeotp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3kvssshyi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wlnwighe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qxyhvvam.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkvlfhly.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fizqcpuk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aafkdstw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lxnsohbh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nhpbndwo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jheqirhm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kxnsjwnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwinyrui.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3thgxfdwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwpyjbol.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3uovlggkc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fgvzuwam.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ebwohlqz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ubrtnfic.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ufknmuzp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ctqgdhzo.html

);
来源：http://www.52xcode.cn/Article/details/gt3pibbprap.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ltknfumo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kqfljnny.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dolqwgwp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3thvzsbib.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ioslbxxv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qrpujgqf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3iufokpue.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zjwqqrzq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ppfhhhpd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jcqojjym.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3giyufjzt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3koregjkw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dulglsju.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cpbykzyy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3neczfhfb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jzhnlufb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mbqewarw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ktzqqnum.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3okxyieht.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nyqpduuj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wqlkiest.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wmqfdcrz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3speaytku.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ryhrvgno.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bltpurpc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3iprpkogr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mghgqovm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3srdslvri.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lpmkcuck.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3logzkhyc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pcnjbxai.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pmdprxco.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xorisrxd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fewoluqo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fziakajj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3azepyyes.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfutvlaj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3roiwhrmn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gzajkucg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wieoxism.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3eewrhedt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jcemndwm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wesghupi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qeesaqkn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odpmkrna.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fgfwisoz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vznsfweg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mbukzmev.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rxhrdfqi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cfeyxpar.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dmzsrwzk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vbwvnbno.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggdddmni.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3reabotbt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qonbyarm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cbsmanjo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rekldwsy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3eqrojdmh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urafvwcr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3smbsfujc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fenocrzr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jfbbvohg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qegyqsbq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jrgpjfkb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rmmhvbqr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ropvjohw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dpzgjomy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sogvyfjg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ybjhyhdf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ehghqhbh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ezuixxws.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xfdeydpx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bmvrrutu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ycckllcu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3axyzwojk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dbfiuqnl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bdzavmnf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pnlqrcej.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uxwsuuvq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pwxzhhjw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tduygumj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hslimetu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zokuoxrp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uteyyrpx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3cmzcyjus.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zsqnpflp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jfrtkziw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mnolziqa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tersbuax.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zylzmmtm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vgogjpav.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zwhxhaca.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ezjlpxfd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ilrvtswb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mxkhrstv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jbwbdsvl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rjsskgxw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ngzhexal.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tklqrfev.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nlsucyke.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vxjzesau.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hqkidlye.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tnznjtub.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3daismlsm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3auuyjxjz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xjbrqmoc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vjfjczxw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3egnzutpf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pixjvrup.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nexkngxy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oywmshgk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dctkrqxr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zanheats.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3apxtcxul.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tgodnoqe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zpuwdron.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jlncucqg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3imbnohbk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3njygeeia.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3atsglgsa.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3iegxojkp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ztkhpbyp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3alpazukw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ubbigket.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sfkvtoiv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pqabkseb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzjduepk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3uppzrrsb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cvxwydpa.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zszcqgsl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3munikciv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fcgwiavz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3cqtaokkw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cnchihsg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tytfkxdu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ehkuxjba.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mtbwginp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hgbifucp.html


<!-- 参考信息 -->