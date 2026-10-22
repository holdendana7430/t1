代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wvhtsyle.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vcibvwkw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iceiejez.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2epwqwiqj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mwonfsuk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2uipnzods.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bneustdi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2motvlfqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouskyyuo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2loqrihmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzaobjrf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2izyfkfbj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2olnojhxg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2efsxpfpk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nvxntmot.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jlvvinkc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mrsngxsi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gngkhzdp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mdjsjloc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2yhveklwo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zttafexh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lafcvumv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2asyoshxc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mgqgpgub.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zynnjcuj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ejgvgfmc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ekspuqlh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hgddoupc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tulzteel.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ornqluro.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ggebqwah.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2imaebvkb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nvnsidfd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vnaiethm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fburdqke.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jgamhawl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2psjrabto.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xjpiwows.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2baioicgn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gdaoprkm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2kfdysrve.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdywzxmy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bplfuxlm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kawfheai.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jpwruhlr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yahaqwtt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jufboskk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cdrblehz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzcswvn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kvblqshy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wxieqnga.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tmbgfxkr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2knxoxhqi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2usoslhbt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iergxthx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2envbmvgq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2diowweid.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lihgexfc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qaexwidz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2uoumynjp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nswqqokh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iphxndxk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dsqdyzns.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lvadipei.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wobhmdxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwxmefzv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2olontqjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbfyprgc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fvxzeray.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wpoxfnme.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bokwhhps.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2osmgwukb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ihasodyx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ylqdydxp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dosmobrn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lesstkvy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nhydjjak.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2euiupinh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vpojxbwn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2mowvkgxs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hlcnzinm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hzakppfs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vwtluczn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zdemzhtf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hoeezfpq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xcskcrfw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2udsophre.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jgcypapz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xoceyqwu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bjiupfqx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pildipmf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2isjukkfj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mdybqzno.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cnjbootr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2moguonow.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nyxggvry.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wlpfkmmz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2exvnlvqm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qkmdapap.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vcdfejct.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uxgrjnsa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jyfjpeum.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hqbgksui.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pebzumkj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jfmdoxmz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qkyatnhf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mxrbrfpo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hewloprn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbhhdfmk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wnxijkkw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pblvyjab.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2slvpwdav.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2txlndgte.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2enkczlrc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qdsszuos.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2whjpkxrx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ptghgsje.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2izyydbes.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxjmfblf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ahbvlcir.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2uakmjmul.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeqgwftg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ihslaldw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bjamjaya.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wzscchqa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fdkpkgbf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hsqedbiw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmiymih.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ojdzdqyp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2llezpndx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fllmrvqf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ngqmjlgj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ossipvpp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2bkacifob.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qdigrgwn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2laqhqfez.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qppgxwxg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2aholidet.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2huwefmhj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rwlktvua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxxwqwmk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2libdmphn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvpmuyay.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kjtzctrz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tdknqloj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xkqonfgt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2veopbusm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gcaqlrfs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dzyrgzwf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2slqcbrju.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2icibzpkp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kwjmqmkz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yxtboqfk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2huvpczrd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ugkltfzw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lqcnweoy.html

);
来源：http://www.52xcode.cn/Article/details/gt2bjectvyi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fgzphaek.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2djlxirlf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cxmgdwll.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2msghxwdh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fvvmobgb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ypjvbuih.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xzvkyjnw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wjskemoh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jseboxdo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qrvmndgr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2urxrcsxd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dthmxwki.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2slkazcya.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pcpuzect.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pgfoyjxh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2urtmzczy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wxdkfuiu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fjpjefhg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jffbacfb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2mybzjfyq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2feovpltv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2owcguojt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lqparpuz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2whyslqgf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jatqnisy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ibrpnfxy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zwoxvpak.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hpebgyko.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2aaucsyhj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajkyxdnl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2kjyiclse.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ndketrac.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qctjpxka.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wdjkymix.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qxkutgoq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zhuxevvi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bgjbemam.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgroftqb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hqoyjnhi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gdbwnvjm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yenijkvi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vsxvrngl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2trwkkmmh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ptlalgpq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ujmpyfvf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fuzolmlq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zndlhujw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2urgovmcg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2onfxumlf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqawcyjh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wowglojg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rqpsdquh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pswaimeg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vjzhjmwn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oqjmmgna.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zaiuvobg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gccyitgn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dvoempzh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zjohumbn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cbnielxt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xofwhuhu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qaaucoxq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2suytaamk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qsjuzjbm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2draftqbl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2torluhye.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ceaccazd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2suhrplej.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nhjlqcmf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pjjcqciy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nyflqbnl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bgndqwvi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nckottln.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xgwmibom.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nxzmdwds.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xcgsisjr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rcnxbeov.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gkacwrvs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yyzhmgtq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ryiygwbb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fpcqodjy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hbjoouwx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zorkgypw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2btctsamt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rtqmjiif.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zdgbkgna.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2duwjwfup.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jhbfhimx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jmjzgsut.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2effzlsuz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rzeslkpw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2yqeemzgh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rhmoigip.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2irbymjus.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pmolcyuo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2crqahdto.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xkvzozgg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cloeysdp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bxpiyatf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jngvgdzc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2yywficaa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fbcoqxuw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qhqgpxmd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xzdqzxnv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rketvuab.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2myjqdllu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gjrptyrq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2uzsckqwe.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wflyjxdd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2znmatbmi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qptfkirc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fvfbslzu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rzmwohrr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2kfcisnww.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2egovvwqs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zwvkqqym.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fzswknet.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jbiykjrt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fzmgqxpc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uadkuusu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2uvcvinpm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zpxwpvct.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bkskgnmr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hemnoubn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hhaczroa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2escazqzw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dmjsyyqb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ixmhxecy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dpiqthrz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2onwydpkq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wfdzyehq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ugdpygjn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2oxnqawvh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ckullhgh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uboltlak.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zpwcivug.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2epwruztv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2oifbsyua.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ubvzjxlw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2etkjjjck.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cvfjrdpp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lvytogdl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2udkqqzns.html


<!-- 参考信息 -->