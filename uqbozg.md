代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zwgtcceh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hgquopjm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yaxmqqyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ovavgqvl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zzryrhua.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ejsbljad.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2phlpteki.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tkcpbtjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcucnvut.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qnonecsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuwqacse.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2zpxibfdv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lqdntchr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hdxvtybw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2eiceguez.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dqqjpujt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jagfuzbh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ouvpyhok.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fxzzmueu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2svxnzjpo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wvqdcdry.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxspuhe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jqxnarzc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bhulssnt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fvbxkavp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rwegnysp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2aleeacbr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2oyjerlny.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2setwagvc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mrtsfspq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eviljpvr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fihosyqr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rxeqzull.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nlrlbxox.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqzjcejl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ecxlseef.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2yonlclcf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fdhqansk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wofrblly.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lthqubvf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2itsujffl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2npfkxwty.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aeozmvue.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mjtjonqw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2plazdvdq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mhpctvrm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owdndczx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbpkbt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2aaavhzlb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lhfpdwdi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hspqkyez.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jpbuulcs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qrleifht.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cgdiykex.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zcwdtmjo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2iofgotmn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xrgvuyex.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ubuexlph.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2aitjeatm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uvklytcm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ntwnvvgu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2obbpxuaq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rmtxyina.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jgcadijn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rhbjqhak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfaxqwyw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qegjytvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2winqjycp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rtnrwqhr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dobbsqos.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iwdmjjfi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lpagbfnx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kgadjubl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2txichkdc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fsvvfimg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kroibtth.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hyouslqx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pymqgeqq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tjivlexv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kwwxymfl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2clcblqfb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2lhthxvxp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xlecxsju.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2foxexgcv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lgvjvypp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ewadrkpp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dcxugcyf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vmugaghs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2srcwzmxq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zbccgmvm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gofhesmv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpiyoyv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xbwtvsxg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ppldxnik.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hmhuqbwl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2drwuccnj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zzbupfcl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2upmlyktw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tbxalcra.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ousukiuq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vzxhrnkx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwvzlam.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jgcfhugb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lcfikxvo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cmcketzq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xxpmzsyl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2relwwdlj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xycbrvxt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbyiwltl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jcxcqafu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ojouzufx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2oxlnqoqk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cipnxgbl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2lwjnqacx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ljyawlve.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lryibsve.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2emvoinje.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfhvxhdp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pijuitfq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2riropzgs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkqbypi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtvycrjn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2zkhfteck.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bxkkmgnc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lyxruygh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vnwaahuf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sxpkgdat.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2tumgykfb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dkrdyyda.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2crheowfx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yjsagivn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rhuvvopx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvkhxpi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wjxdgcwo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2feueqeva.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uwupersp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2epkqaqit.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2abpgbttv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nroeplkc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hmqeijyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exmhepyf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bvozlcna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhtlpqvs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qetupqko.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2omnivnho.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fgblblpw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pzxzmpzw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2goljzglo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fbpylxaa.html

);
来源：http://www.52xcode.cn/Article/details/gt2eupkcjnv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mwgniqvj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vxfltqsv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gcizfdjs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2drtunoqg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2edtyjlcb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rlpdkzww.html

);
来源：http://www.52xcode.cn/Article/details/gt2demzrttp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wxibzjet.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hhnxrldm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gkvwlzrn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2degaptnt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2olnviudn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2brszjbyx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zygtdhcq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ynrwltuy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fliptnbf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rrbhzdun.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lpaakoun.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hbenujct.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jrhcsaec.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2oxutyxxm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pcrwtapd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ugpnlwam.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jtofzavc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mbjlwjjv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bktbupet.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2npsbxlip.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hxtekhsc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nuyohffe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wlbwgonp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uveixyys.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ocgijamx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ischkpjg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qalfzxve.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhxvcwhm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mlnssief.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oczvpuaf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2awmdoxrw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uhuauzfl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vjjpsvjy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qtpngqdg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ugpznlgn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wzpzhnes.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2elipmqaa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qpmlkkks.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fyndenct.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zduqugxu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2huefuloh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kkwbivol.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2umfjclnt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kzpdqldc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kutdoeyi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ofrycgvt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jgtrfuih.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yckrfiub.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hdbyavao.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zozrzish.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zkoktugy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lrhuomcb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uvypqtvj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qnuxzlju.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mufbfpuw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rjfdzuqk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vxsezgfb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vqdyfpso.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xdcrfusf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2njhpgntm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crtdrlkg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rdmimpdk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ossehzvv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bkgulxuq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2prnyzwal.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2noabpxom.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2waymjpne.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tixdapep.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aqkltjbl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rcopshkn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rpfiqdxp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mnqwbypk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tlojtres.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vtxxvymk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vskhrlgm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yexfwdot.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jfniscbb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gmthjhos.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eeeqewuc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vwogpuye.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2euptuxmh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vxvqizyt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jbptgvyo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2avwqtzwj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ifmikzfu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2wulvgdum.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zstrjirb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xbgukvwa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2acnooyay.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2iqecnsfx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2kvuhqfov.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xjlmaqte.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mrfkaozw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cutwiydv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wlauqbvd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2knbswhdg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2legbpydd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nmzzkwpj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gbrsgvre.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2obvkbcww.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2afvkulyk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jnqxvrvu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hhmxrofd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mcwyaywr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vssbcupt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uhtctnqh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wzkmdqbl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnpvqwsw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ocoxmhjg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wkrmdviq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dqegrdka.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xhqsilvg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rmcjydcb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2telpcriy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yanxgyzh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qrcfrezn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2yascbhbz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rxnfutrs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cwurxgtc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pymxaloa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hqmdfdiv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cerbgusc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hahchkoq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rkhfdrow.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2skjeiwib.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2khlcnepm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2btstukde.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dmigkofd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jtnvskwz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pszqfvgs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pzkndjsc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2aspwdtsc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rgawygff.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fafjyizl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2nxztzgdr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dbccages.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2alqvvsng.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ojuuoqik.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kdqeftxb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fpatptjg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gizoukcw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qnogezbg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2buiymzdo.html


<!-- 参考信息 -->