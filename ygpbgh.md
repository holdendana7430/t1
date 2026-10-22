代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pazbjmpw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fyrkwbpw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qffddrgb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2fnkcjxbs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kgkbnqif.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dquzeepp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ymmvvgdh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2juavihtn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yrbqdzrc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjoukhp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qlvryurc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nmbwppgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epddypoh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ftcfgyow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbetbwlm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bgyqmdsc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cobjzqpa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qzwcxqcm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nppemcup.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vugzvhxt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jrputbpo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ufguywsz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ngykuypw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xdvqzrzr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ucfyzkcf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wsclyhur.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ipqhzhnt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bghdrpyd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tddwfvlm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2frhhdvdg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hybqpesd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ubwtldbf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dtvsssfq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2cylwjjmq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2beemybxe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qrdpfcyp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vhbshndq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sgpcqmxa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hqtpofhz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fcqiynzt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnzvlcg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2totpmbts.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gcstyomb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ajqntnyq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2udqhvmqt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldzmgsst.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sivrphds.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fvjgdgoc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dupqltqr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rvijncov.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfyliede.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ktukdopf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ldlyezbj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2txksjvnj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qltwvwlf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2badzydww.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rayrnpcs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wearxoxu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2muagqrbd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2guvtfarw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2apwgawry.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ryrvzxak.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vzdfboqg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tytxnzqn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2belnkfhy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nhrrdhrh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jxtqmjwm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fksbzlgw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ltzbabmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pszmujss.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlsfianj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkahuhpa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2etkotqvy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gxnaupwq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2uykxgagw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mlwdyjcn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ofzzhqwm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2sjzhxgsj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2scxmgtnt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2exapcdte.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2eqqpdcaw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2buiuowrh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wedtrguy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2noelaztb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ntsajlry.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2temqpiux.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sdfayonk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tgctocsj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnnymfyj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ftfbxhgd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ooseuctg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nkvrvvpz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2spvkvuqe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ntzdwagb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sarkrslr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xxfbgkol.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yhthhyoc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cemszcdd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fxvqwrje.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hqmkepyg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2medibksn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2canvuawd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vrwjodgc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2djwlnnhy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zyizcbci.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pjouxfib.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bjkgpdnp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fzmrlaes.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dpfpvods.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2amxljqie.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zggtuvqo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wzsxikzy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xcbkojgt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2okzmdoqn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ktlwypiq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rwzniqmy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xbiyxxsf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2thqhvafs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vfdhukqs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcdaaksu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2txrbnems.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcfqkmdk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvcuwkyl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mwzfouxl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bltxsmbq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqeepkcu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2olkvdoxr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2okehkydu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qtpsppja.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ntnzhqbb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ywengxng.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2chfxoevj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ctmdgxtd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yduxhoiz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rpwujlhf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gzwlxtlc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rvkcughh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pavfnstw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2uctyvtaz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kftwlvzs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2sdgguylb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2aexqoqfj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fynmvpdr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wcrsewkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzqqkgem.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2etrexcmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntrkpief.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2gtbjkuvd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jyodhktw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mbjqalgm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ijnjejto.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jyiduzhk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dpkyfujh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pzboghrg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hqbnrclw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mdnnbjct.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2awqmwwsf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rkyuhbmb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wxhnxdan.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eedzalqd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sdrbuywh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2enwclyoz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2grhpuzsr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dlclipyx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dzqvwnsf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ptjaroph.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yjusqbsr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2aqtnlewv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uxhyfbmd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uyhhfvlp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ptszvuqw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fzssmfep.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pwpqvlam.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ygdnlxtn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cjkrwoly.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2chfsqsyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2exqvijdr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wwjmgixy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2huxukkvr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2omsgoseu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gzuthssp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ltiqorws.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2pvazvrkj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oyhscjxu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zbenhstk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hvnhpymz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rtjpowzc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tjrqxlhb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vqvbdwoc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fqeyzdyt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ocptlyww.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ijkaidnl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2fzbmfgmi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mosdhiyx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2orplleqg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tsjqtejq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pmscqdpw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2quvsmivn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sybwwakd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xqaeawnm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tpfhkbcf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vewkggnu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vjdtwhby.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jlpajwdf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ehsjwlhn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cstvswsj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkqxscmx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dbtjfplc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2piijhfjq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2szhcpnjc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffpdovva.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2akqfgzpq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eujdvzci.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2otolecnd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uozmtpqf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oekrrpzr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmyhialo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ckchnitu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qtmazzmz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yndeubdc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wjqxicxl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usvsusxg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ifywyvow.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wvjnyeud.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2glenutcp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cteuoiar.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vmlxayiz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rbhjqakz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qvalrkts.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tjwfwnhb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xcaimrqa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qibkqtup.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eljqufif.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vqqpoolj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhopvq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qrmzzrpu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kzrlhdsv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2osnrxokx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nlhrpdpn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hmreybdh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uljhdgjq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ihzfvpqg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ncgujdlo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lxggvvzj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zdalugms.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zxnwtlyo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2eetspohd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jgxvxfio.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nbiwxzix.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dwqaiznu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2levrrclq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mjeqwpon.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tzecpceh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lrqkymee.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zysztghp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vqotoyep.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nzilzksb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mctfxqpu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2finmezdw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2whfrxqja.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kfqloume.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sehlflec.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hdqunqsx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ccfzernz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fbqddkyq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qbfqkewx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2syvagxdg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yenmpmmb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hcexmmlw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rnadcdnw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2islrtqsj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2djlybaon.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qhmssovb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nxvmcztq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2slfjpqnv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2axngqmmz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dqumakkh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ceelsozi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xvyovsbv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2datkeutd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xluqaxpm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2oocnnnpz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zeklyiie.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ebndnssu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gtpiwcsk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ajgksbvm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mqlpqnue.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zqfciymm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tmzthhln.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zqejnszj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2eewccgbx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2enysohod.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ptxdllby.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tyatjkis.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dzdchgsy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ylbtdvxq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jombmevy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2eusrsfor.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jowfgxci.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mjsmkhoi.html


<!-- 参考信息 -->