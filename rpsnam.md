代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qdjofkxc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3njgrfzkf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fvaxuoqr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nnhdnrsd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmwlnmgu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fdvvubbp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ljgdzmbi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vbdnqaad.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3khiugjdw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3suhwzuvo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rmmypahm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3earqwmgu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jdjyplrp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3wegcczya.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zhvkpuxx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3znsokenc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3eudplwoe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jwtrcezw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ewfgoqww.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vewpycdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbwfqrly.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3chzqlwbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bevnkyzq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xusidikj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ccdxxvxw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rspmjyac.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xagjwdgv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3azwpgqia.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mmtmwuxq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hiddhxeq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ttfkgozf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jlhdrqyz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3auzbqjzq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzifdyl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xcebnnbk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lbrckfec.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3piekdldm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3aqteuufc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ehrggjku.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3iobeoxou.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xvspfxbh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3njcgesii.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jaxszdyg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ctzzsngp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3msxviyfu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jwglbpvu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzwmzxzc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3niesphsv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yvnmvdvh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkakdxdw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kwgbozix.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3byprhxmo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3diowdjvo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3voxplqxt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sccdvxar.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ycjolzdk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vaklzltn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ufubujbl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mpomcpxd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lffffwlc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gcrzbjec.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lgpuunvk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oisxyosb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xtmtipox.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ycphxlbb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nckldozu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ybswluuv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nctoommq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3pfxvqcul.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tsoxujgc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mhiitkkn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wiaihzws.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cpfangiy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3htmlfosm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ctcesmsu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3oczhfzux.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cdyvpwbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyratwpj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3itzoovhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmciuqzo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3czndonpw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ymtbcsto.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3lnbsuvnv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hjrigfor.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ytdqhrja.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3taqtboqa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rukvoczk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rrnxmxjf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dbwxocpk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jquoydly.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3naadnrbn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xsqznjvr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vowzuimj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cezcxpeh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3staqvfvq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3btkhcqep.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fkjieajj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ytxrwnsg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mslvppif.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jgxdctfy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3juyhvpch.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3msipurpd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rmgljeak.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbrwlnq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nselwgil.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3beukzlkq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dmrucvyk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zssjyxqg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3llmnvvdk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iwpdrcly.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kfrpzypo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lhwtjyog.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lrabdela.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wcpzfvmr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wdlhonsm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ewnkfsfg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cslualdw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vzmixzkk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3msdrigyb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3snusbpbc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mihomnru.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3iyhugyga.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xrqwshrq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xzptjegu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3icflasfb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3betgyzue.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uszxwdbo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qfhyhuas.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jrqvehpf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vzkerjnu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqmbcebh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gntjwwqh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3doeyihqu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itniarpw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ljedlhfh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tdznpuln.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wnorhlfd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kvqbqzsk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3inqrkcmk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3afkjnqob.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3tamwrtwo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3piexatxm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ucybrfex.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3khtcgtas.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xcqldrtd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hlfxqznf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nvegtrct.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sowiwvyf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hmmmvgqv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3pakmavhj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zmaavdgo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zzfdbrcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slhnnyft.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rvibskwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zncxjfil.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ymvhwqbg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3izqwcvqt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3seinjrks.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3phhxlxvr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xbaieszh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vyowjxbv.html

);
来源：http://www.52xcode.cn/Article/details/gt3ulagrhgm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gsdyqods.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ombukxwp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tgnbtwey.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yauzbeyz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3izhioaeo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aydeguff.html

);
来源：http://www.52xcode.cn/Article/details/gt3memlanox.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3oxthsljf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xaxunvvl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jadgmpoz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xrypksqz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3uzfruiud.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3boysxfpf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3znjtjqmy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hvkkvoff.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ojtjwpbo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3otbbsxen.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3huiwwqzw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tdatnwjc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lddkyite.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xzgbchso.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zzinahfr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jlbmqmoe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ssftkshr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tvmwkaic.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mpdprgaf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bqsyqdvg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wkhsaqza.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dwgigigp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qasctnrh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nksavqrf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uhxkmrxv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yxtsplog.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3efqivorh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mviswjaj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mondqmba.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uptkslyr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yggohiow.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xsbyzroy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3skmnjcly.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3orgzivhy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kpkutdxm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zfpmfqcy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sispqama.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qkrvtien.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lmmjzmbw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wuybyxom.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xysolypb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ghdtmood.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vjpaknnv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3svkrntbd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nxfjdlti.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bminfjyy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ldsiwrqm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3eggxnhub.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ybkosyji.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxtfusas.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3deesmrxr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3riwhlchq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fzqenqep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3szovhnqk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rcgjeism.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tekbnwsz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3lovrautj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yimvmstb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jrdcgkpy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cjbykifw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3euyqfkhq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ndjoapem.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jctzkrgh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3oydojpsx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qzldyodg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gspnoghi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3brfzderm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fjdtwsed.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gslytnwm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pbjcfirj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yukmqqya.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tcbajxoo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wzebvbbs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3raieqzhh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3afhssuqk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qfqihqeo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zpmxmphr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mrqwxzen.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lrtonweb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kuziivhb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ekwtehor.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zmzoosng.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ozlatmrr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bzropgjn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3utstrskw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bcbricws.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzaghqzr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3raxyzwht.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3syvyvbqm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wbthihwb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mifglnaa.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vkqhacuu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nnmncttc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3figgtlwi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hxszjqkq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xsfeseuu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pakhkhwl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xdwzgxge.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3aaiismfe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xvamkduf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ehuallzl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vwtccsgm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jergzqyq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ewwljrsq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wojpbmsm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3emybqceu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3nudvckxd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xvlxbuzp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wbmirzxj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3isevqakv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tvpteguv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wlpfotps.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qibvbdxi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mrkcviag.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kwkcxkcy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vmiiphag.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pwwzguty.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hylunmfn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3epycfgtm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vrzumrsz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gomjwyzj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3owgwfheb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3eefhmjbz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fxnnrwyf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kxwewayl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3joytajaz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dvfewtks.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ruyeofcw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ntxxsrdr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cskteevv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kyozfkyq.html


<!-- 参考信息 -->