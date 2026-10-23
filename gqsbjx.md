代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvewxglb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3evsxtasw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ohqycjzw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ccfegfka.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wugugnqv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kbxcryeb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mekuacqi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kaipgebp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dclklvop.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3akmpwgkr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oxngtgep.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jklhgkoh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rdwprafz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3atlfdldo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jfbuoowu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zyjdrlef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ligpnevu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nuayyhbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecbjuaab.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ydtdqocz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eqcybdvk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ycwdtgef.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3sdusvwkz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mlhpavtw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3vwamhrtf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3yywavmym.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3iwxxckbt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xipshcxm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3clwbrepb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3asdbwhcu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tvugdazt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qxvehcci.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sptkdwmz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ulgruszz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kwyronft.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gfnhrghc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3urbzemku.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3czprzlhx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nkovtrrf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xmpqgous.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3bticzxdp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mgyotfct.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lhhcgaco.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3olgtelpx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ndpzdpdy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vsitqqve.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3yksflzhs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vomdehtm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pzbvkdkc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhpjzmf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czqxowms.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ytmqmsjj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zrrcapjs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gfeuurkr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gajqownc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ltdnumru.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3elmkbstj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yijzviik.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3okwhoynj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ujytxtow.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3biozbsku.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ilfrklnx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3euvqtowy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlosxgwk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ldhyxqen.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3urouoxtn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kyjxezbz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3exmvwjfc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jlvvrfmo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3egtcqmfr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3oahhmcul.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nlzrmgkz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tgvipbrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vicwrvki.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3huqkkmfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twpantue.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wkocicpl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3okxvkfrz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zvaomspd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ptartrvl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3szzlegdh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zjgcwifl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gsdjsfvl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sxtzzgvo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ggfyuytz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cgavfylh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wkjugftd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hnosgsjg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wtzzafnp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yvfygtrz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwayqwt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gdbnhcch.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ydyfhrqy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3buakfduv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmuiqhxp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3gazdsamp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ttxljluy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3upnrnrzz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ivnjexnt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ruamqeuo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ngdgznjo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zvyhnbgw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gihhqkav.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3gnuohohf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3welhoxpc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mxztnmcy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vasotarq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xgfsaksr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3shzbcgtz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3efzpiyvl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kgyhzsmq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3avyxaobs.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3eapidibo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cbjylapb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3trdqqosc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fmefkxre.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zcpbgtzw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qyeryjxe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pfroxvcf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bzzyuzbg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lyjqgmtv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ooohtpkv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3njziomhr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rcekroqa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ruvrmtng.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cguimuen.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yrqhdblk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hcsbhrkz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3iofjuqkn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mriatpvv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mvgaywge.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pdusmohx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ttdkhvnu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iqpyixja.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tgixlcss.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3erkmiomv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ajuzrtnh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uwqkavcx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3efhlpkqi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lyvoqkft.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jiqgajng.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3pzzoohbc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gyuuafea.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rsgswkzb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pifxeokj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cekcmvoj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mnxtoayd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wvkdoqwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flsixbtg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bdxspilz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkowxgzw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vkmtiepf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3whcmnftd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aibmoxvn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ysaovsri.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ahwtpned.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zqhfrkbz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gdowrjvv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kszowpcc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3piwxbbzx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jqiaoijq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qbutjmnn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ukhktwgu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3omdxtlxm.html

);
来源：http://www.52xcode.cn/Article/details/gt3cabyzups.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ubrrzoua.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oxvrjnrl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lkhwnkbw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3askhyxqj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gijbxjks.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3oojbjbgn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xxqqtwkk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ygfrmksk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wwlhbuzi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vrlmtcic.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3faiteyvb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bnfoukls.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3uvemzbwf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3expgwzsi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wxdwdcof.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cxvwpkyn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3unoxcyux.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pywxlslc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gtegyhec.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ywovkpqy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3enhosufb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kscnbmko.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vzkxotmz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3sihcpvar.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hraieqhc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gziwkkai.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ovlejxhd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iegzrhvk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zfypullo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvlkrmpd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bbwmjcpk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3okqgflik.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vgafplhq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3teaalorm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jbsnxvsi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bothshsg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hkkrcrva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uquyzqag.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nehctume.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bqgaylhk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3glbkvkuw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zzyfejhw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jwbcyqat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lksfcswz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nvqhgyaz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ijkrvcxx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ztolzjau.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rcgbjrdp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lmdqjdml.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gtnlppic.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xcjtomus.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mfzeacos.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ytcljcyp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhmaxomm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3myvwohks.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxqthvtt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ffuqxozn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oobyqlvc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uspybdxg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sevtzjfp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uzninzqu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pwyhoyak.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zrbemnnz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3bfdtvudt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bjksivyo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tkytpgqj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3raumbfup.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3szsvujao.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ozejoxaj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kobkrloj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tktmpxwg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gereesdv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zbmmrdig.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nkgniykv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mqsfjepu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mekhcruz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pvlgamhf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dsbqzldp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uxvkuodd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yykazufz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fsqozjfc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ucbbaghh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cjtmjlaf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lvlrsfsi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3odoacgqz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ecmtvpnx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mwihcqqk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rzwftrum.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3etghxxlb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ihbsmhkq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3heyzutuf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3erqjglok.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3sgvknhng.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3unoqmvkl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3onyqxjcf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cjphxrga.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jzycqgpt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vfkyrgpj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mtoceiho.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3anxuiazg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrwbiop.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fozpsxew.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jgbnxnyz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3angmqgee.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mxqbhvjy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wenoiljx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pgqbdwei.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmnezoqn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3sckoxezr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kjrfjzcc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vzsazqfu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wyhnwupn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xqttmvxl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uadoxbjz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cuurghou.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3unkkpkgf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3aqmiudgs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mxdhznlo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ldnqwwsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xsttbylv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lzgnvssf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gjgkjhtr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3sdxwehgd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nkbqftfr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3efvkdojo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3btpnnmwp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3owuxydbh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3itisbajh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bfmihrfg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nihiabhd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zggefigp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3azybrbef.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3obxjxhtk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ifmgaqad.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3takdcevq.html


<!-- 参考信息 -->