代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lbxeivva.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jqjijufm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nvcyiqez.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3firwjhpe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hfauzsip.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fqgoptpy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rlrbtvkc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3bvmiygyt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dahzumlc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kdihpvxw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nsjhijue.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ysllogal.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vxbhvuou.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbatlpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wwrkqkzf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tkhpsjpb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3evfximvx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zveczgoy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zguubznh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vdmhatgl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3natkzsmr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kcswprim.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfnuffyb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fticvoma.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3olaqcbak.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3atwyqobl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ovblvjtm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lgkxcqql.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vpgxhyvv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3udrgygog.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjkjhigc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xjvnyjsh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pkpbjsxj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wotkngxa.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pkmjgnew.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bapmenng.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lypnjido.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kqdiexyz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3psgawims.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lifzravu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3twmgcwbe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qgfqfbka.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wjzcgycv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3naxxrklr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yeeygpqx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3gpexopwd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3stmfbniq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fqnonoes.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3egupohdk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zdykybdq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3eahyazfx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qeaqqkxs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ijcoxoys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edtxipnl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3htvloxnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sunlnqaw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hsplyesn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nxsylbkd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qsvewpls.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mgbefaax.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bgyumbqz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tvnhlyjv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ekwdyhlm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3femwjenm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dyeddtmj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gdagbucj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zsvowsil.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyhayicu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3apifmtji.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kqghqlku.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ydvqiwcg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fsjysoku.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsirykud.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3trimvcni.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cynmypdo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3stnfgmue.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3oedttxyb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cexpjipn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzvoqjau.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qnmgydyt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cosateag.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3seyxqxlk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dokkslur.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lcedhgbw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hqbyrzkj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ztlbckvy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uwxlqose.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3feqxghxm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yorbnnhg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kkjmywcm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rwzocxti.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fcpkkvvw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rkvezbrg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qtanxvfp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3uyqgmlem.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3peyxodxm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjerutwi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wnxyjhxm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oislngcx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ynqkaxhz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lgqmkerj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3eramxcqk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fjklukjh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ycidwlxk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3sekpgznz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yfewxnmz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cffwepwh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3yrmdxaar.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lqxlwsrt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfvjmhhj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tbpdkuhn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rhfveczv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mrhssrrs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ptximmlc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ozsitoji.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vefncefv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gmultqgz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wnrdezea.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nbkbncqa.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3fbbdrvpv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3khackaod.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zagkdrjl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iretjjum.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ukwqqtey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lvcxnvzx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mchwlzew.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3fyjyxvgn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rvzhumlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnydnzdj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gliyhklh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nthakrfr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hafxpkpj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3sfdfqrwo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3turunrqt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oyhqchmw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3htmbyghe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tbgxhgmq.html

);
来源：http://www.52xcode.cn/Article/details/gt3wfbzdeyk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xbguchlp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zfsheeho.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bczmsdwj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3scdunpsc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dznbkajk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ihsutrsc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yyvkugge.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3yqgukjdj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zqqcvsah.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lknqophi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hgymmkmg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jswkwbvc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gwwqtizq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ztctpsgf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ndidmrrk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3aqsyozac.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lpozhfqc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wnukupoq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xzglxazk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3olspqgzr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gunisboh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gmikrslz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xgnkfxsz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kxskjuyl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wetxscrh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hhvktdbn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ezcskoni.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vvoapeus.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wxdqgieo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lrjjvcpi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xbizeswk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3riybippl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3imfmjaov.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3xgyonnnr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tiibxybz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ijlfyqrl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ddzautyb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3njzargzm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3txlhhofg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lrypzpph.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ptlyfaee.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ygrylrzo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jtfkgfrx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3webelcdy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gwsacrng.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sdklikou.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rfeqwwma.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tdfhcknu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3baibshri.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3amxisjbx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hzwjrttm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3speegrpv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yvmygtwp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3olylyqea.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vezkddwe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3oeajkwyh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ntpoojhn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cydysuqf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3atfliebx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xngwelvf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wjyivwyq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tesjqokd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfjbwurl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vxxorvxv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hrlnuiro.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ztdyjjgh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mnzpypls.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rosplylx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gegknsjv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nlzonqjr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mnubghqz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rehjlutz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ujmwacvi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3linacjax.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3djbwlfsm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mhtzcybk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3blnjtxgl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xrxjsiuy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ysrbqfao.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iqpcuhue.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3dutdiykc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xumzvqdl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vlpeayox.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3htxqnjgg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3izvhnkjy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ypqplclr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3llvrbjof.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rryxwbzu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3eqruklve.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ajuybuis.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xqnbgnyf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rilmzcrm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vbugqhhp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yngkxzns.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3owrykeng.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xyxnlhja.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3npzjwbbg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qzkiaxzu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wfecjhto.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xoibimst.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3euruusne.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dvfbujas.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qoqcdmtr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wsdolkom.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xgaukdjx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fsqcsdzq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cndzqwug.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ahsaxlcs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gbntrfrs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dthemnwc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iadnamlr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bkzjprpf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3eqxxgglh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qpykiycm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qndztflj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hxndvhvd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xabcetck.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3fwvnhnmr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3plfplbpr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yqqgqmsf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3glekktyf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lqddkist.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nblqgaed.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3avwzypyn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fquigwrh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ahzotaze.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fzvkqoyr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oyeznfun.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gplknagi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ladixrqm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bzvstidj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jtloqrqj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hubcsvab.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3boctihhh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mvzvlaxs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3faslafgk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3syqzxwvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rphqlmpb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rgsoxygh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pojrtyrn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3nilzcwyh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hqlwtunl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kvikebjz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ghomzrgy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dgxjlihe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yjxglfzh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nvelxwak.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ifwvhrnt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3dftzrzll.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xuwnjuvi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sfxqffbm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zefryqjx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zskctwcj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hbvccurv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rysvchvd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3twgzdano.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3awawswdm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3iwnaseno.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xedoyiaw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cibydqez.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pprnifco.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gtzzhwdy.html


<!-- 参考信息 -->