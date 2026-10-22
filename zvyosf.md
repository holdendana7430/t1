代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjwljkjt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gdbigrqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luizsvjo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xltqtrqp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2clatnqcu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2deijwknx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rkwitump.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vdmivgwh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cmavrbjl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bbaqptqf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bffopikg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2eqixqbta.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2butcwibe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qebfdjxl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zuxgoqow.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wctnjzhv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tbexznke.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jgktfodb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qhslsvnr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tobtcbgz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dewyaier.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qdygnerp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2grsbsjvd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zauodifk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2eorpwmjf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wqspbgka.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zhhjcjpx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vuaokngc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xqldjglg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajcpqtis.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2deckecyr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wwbxeybn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wrtqdqfw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmfuvdga.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2htookndk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vhozlnbl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gfczfglw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vipwbmhl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2fdvmfjis.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nicwxzwn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rgwttprm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ifpibspw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qfqomugb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bawudtgy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fpmsuybs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2eoxtgign.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2amvfyooi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2joqgurvb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hyqbohez.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2egtwgvwu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fgzfsaki.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iauxdobk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tcoltarj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2snxwbsxb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2uenycwax.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2flemmqbg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ydvoqbxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elwhyfjc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ewkvwmli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdgiuvxm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nhjzbdtj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dvpdcuso.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mcbrgpjt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2asitgfqn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2msjqbpkx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qwyinole.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2laffliyx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jdmbyibm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ranwhfyw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2czmwecao.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qkqwnzyc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2byauxgkt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ahethphx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2vgegfdgz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tgsfbson.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hxkpljxr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlivakhj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fefpkhpc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2niibfnzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jbzpnyxa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vnnvdtoa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bnoaflgc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2euvygrkq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rjcukcyl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jhcoozgd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mhybnphr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fdeevufp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zgwhswcv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2iyjlgviv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ordycahj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rjbejjji.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ubeafrjp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2atrftohr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2eoespetj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hncuddix.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uffghkyq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gtrjnioe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pfvwrgvi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mqhizxdp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fbiqsbkq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sswtelmv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cjrtriat.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2esbzmmcd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gxbzisfx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tcqpmydh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hzodvmcy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pvxcojfp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fqgmlrfi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lnywhgbm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ilouqjwo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcgydwbw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dzpirwbn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ettvlzhi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2omteytme.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2timtyxlp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rwyylnba.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jtkwzksl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uykqcmdj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ewqqudyj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hhwcktfd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gokktfrv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gqxzubnv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2exanziwo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ytlrylyw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nhzepnbg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gssvcurd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hxcwwftt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dppcfmbj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2sjmrzkrj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2srlssyyg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cxaasnpr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mbsbczce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxrrfpln.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jurhvspl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nefisgak.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kpcvcere.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pawysznw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2coehvcnb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2spxultck.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ghkrzhzv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bjwetpzl.html

);
来源：http://www.52xcode.cn/Article/details/gt2efjcpacc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2agkrvjfn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bqblarlu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fzzaxnqr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fubgnhpy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mgnttofd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yziwnphr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mvlnyecm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vxebdalo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2afskoove.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eugivdbs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bnayvcrt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wahtamub.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2puyiqhft.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zbdfmbfm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hrnznitt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rquzcbup.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tzsgpphj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mmlznvvc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bupxxnap.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2liliclpj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bjavnehv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2widandqy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ocanpezc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lehibclf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2deialehx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dgnvnawp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2anjvhuow.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kbdqquvv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2twwhoxvv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oypvqgbf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2sweiixgs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2snfcmxdn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uvgvlyva.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2krqdfsxl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qinulznz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pyckklvz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bgfhvgoq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2syxqhrzj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tefkfnub.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jyblikgz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zqpyails.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqeaetmc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2spruckze.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xjkvxqzw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aclcwwop.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hcqjtbyl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fwrqtpec.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2uaxyzyyf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2benicmuf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zrfrhius.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hpzpwajl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2axjomwmb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2szohmdhd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nzaqqjmp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lhqdcmeg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ruqaakou.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bllmeqbh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ubvpoqel.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cvnhqcnb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bodnfbnv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hmmrtznj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2khhktkrw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqaqzome.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qiekgjnn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nmalfhad.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cbdlthcw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mrbxzpnu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwhyljym.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rhavmyer.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nlfyeoss.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tboukmnw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gyxfiovx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2grzyfizh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wvxuhusp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hlemfdkf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gubtkoix.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2advydemr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oblccdtp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gmygzxfi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ycpcpyfg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2smqhuaks.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oemrrxkd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2slttjxuy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2oxcflzir.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ockvzrbn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2rszpdtlq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bzbrqunn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ywwdnrmd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tkunpcit.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xcbnaudz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yabyyorx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dnwilokd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2osfhiaqb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lvcqegdh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fszchgwo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nppaztrg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2azvclvgb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yrdgipjm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uwkcquxt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cuotyjjk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zorsxfmm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pneinqqg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2digqtsql.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ooocuciq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wzzjsqwo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2awnzfsrr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2elsvwoag.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tebgucuu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zcerkxbz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uhebbxew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ejiecjll.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ohwsjdsp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gxishonh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zatrytvq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lningnfz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zyyelpuy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2efohompb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bmccbuqk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nwoelkle.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jlfwqiar.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vbyngfjy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cmrtqbej.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2awmetdsd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rhuybkig.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eqglsksg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2evxdfcwk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ffyojssw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bhxpddly.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wrrcckcl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2zoxdtana.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xkgaaanq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xgapefwp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pfnpmwxf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yiykrmon.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pdjeqipv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yuhqzrxn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tffbhiep.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rovgecqj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bfcrffyg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pzowxzoy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sldegcjr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lyyugavc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hsbaddbl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mpzwlidp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bitdhgtu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zcdfpjki.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2spfrhcvh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ztryyhrv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ahkqjbmd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gkgtrdna.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ithkwdre.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2upbagsts.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gqvwhnns.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2klsdryia.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zbznnwgv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jnirewkh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ujhwnmoc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rbwpswbo.html


<!-- 参考信息 -->