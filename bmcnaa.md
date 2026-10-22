代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdqofqkg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xthbmiac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unyssrnj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gdedultd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bbvmiwog.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zlybgohv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2axdczlie.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dvfgdiyl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lbdsaupg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xscmteug.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2agcbetqu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wskshger.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2drkpejhy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kimbgjsn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2afhwomym.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zcymlczc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yjsbmhpu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2avlbucqy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nzdnrtdw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xyssnvpl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qvytdmcf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vbyeokbe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2aqlngnws.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jrdzugie.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ydnpzepq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mjszbsvm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fepoffzy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vymeeica.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfkcagyr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dkkjpzhf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2japuwpdj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xtsrrrzv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dqreqozo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2doeizrvc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ooeluatr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xnkleooj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2argpecpx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2scvygqjp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xwczruqb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dcxolouq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2shwnghzr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2phentgra.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nwhlfjfg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vohdlnxp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2tucfcivd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2nrdxquhs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fowmrtrh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cubcgxce.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ndjswioe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lhltqekp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2eppggmbu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ucodjuta.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eyvmsdyj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gtqigelw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xrtjvtrx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tbiktwpf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ulpxcfoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztgjoxqt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cwmkkkcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oombgwdw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qavipytu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nteaecgs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tdifehuz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mevapnof.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2udocfiyn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mepucefl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pilmpyeq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kxwcdiej.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mlmlebbx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bbysxhup.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wenipsiy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dypzbuwj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mjdrkbuf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2lfyvdcji.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vfpzhbsc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ybfvaupi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmeasnho.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xzpdlaqw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hwdbmvqb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tjcajzlr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zszavqip.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qwyzfpkw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xqbskkko.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rgbvqgde.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2pvakydco.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2llcjtphy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rmfrlpsl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2aadaijen.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zkblgkgg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2caegzhpo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xaaptkug.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2drfvwwua.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wcfgmear.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zighseue.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qnmehmjy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fthmrrxe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uduqmmhf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2koocspvx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qxglmzsd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dqwmzmwa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sdyjkysm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jtemibau.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tkjanyso.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wihmubdi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kmzaenzt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fkqgzirr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qkhfdyob.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvndohyf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jlrozgrh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jbbvziyh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqwnkhcc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2rtxggdms.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vppwzwta.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvqcgguq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rpsajxif.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vlkqzvhz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2gcudktir.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2spwgawsf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lfwnsvsx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xujcjvrg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tunosmsk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iomxiutg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vertttkx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bmqkanoy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gpfahxdb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2iysnpdnq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2edqmvxha.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dydohlnx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2kieayaja.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2towgqyal.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sskwtpgd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kqgwwokp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otomdpjc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fayjedvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amwhbysb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2gpibzgto.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cebzessi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gjqbeqtp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kzckcdti.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qhwqvlqo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vvgzrzfg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jpdwdyke.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wsigvhsz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2evoflofz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dwljpudt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uuxkokjq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vnwupwpv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zbixkpbk.html

);
来源：http://www.52xcode.cn/Article/details/gt2veymcfyn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2imlnrvxw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eokgrrmo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xjnswrbu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2azrylgbg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xyhhksnw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hrfudbiq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qnmylqcl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2aznwuqxw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nhnlkuuv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2obwtzxxi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2qykbrcbt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cbrvjuiq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mzcngdze.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2phdhfvxv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ejcespvn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2twoxjfcx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jupatayb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nqrhcmww.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iizsxzdf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2emlrcerb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zmnvdmth.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2olthvzjd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qlwoekmh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uzijrsvg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2atofdeea.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2agfaaktv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qhfdktrl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iyxjsxms.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kijmjapx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brddvatu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bmlpencw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2atoxmbbc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lzatpkdo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gzxutkaj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2unpjlvyj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zjvwluqj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2pjqyebil.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gjohfday.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bwgpxmzi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pshgidql.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kifokixj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rqyzlriz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ljtntzww.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2snbvkann.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cbukblvg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxhdtegx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2bktsgpcj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zwtwdgic.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ejvarofx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxtgwmmc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vmatlphm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ieygvapt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nobaxphd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iegewzkb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2suenfyxu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdmdhuba.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xlacndek.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rkpvvktx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2badvcwxw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vpvvbvco.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hhvvndph.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hveeuirj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xsqhdpyd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qqjvnomb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tfrgquoy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2snrzuozo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lfnputgi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wjzxqopq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yzymenuf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kvtbifom.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wykifpbb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2soneeler.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ciqlwdig.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2afnneunl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kruibjlr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hsrioqyl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2murvdrng.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wwxfqrpg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2abnuiayp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lpccashw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nqhevyny.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2idqvmzix.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zliilptb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2smcqakpe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2sqmrfmhm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ikmraigb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iwtocnie.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jswlcnlg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2kzpwnctu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uyrjhhdt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2hlzsvsbn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qdejjxdm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2woiykbim.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fspuumdb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vdunalde.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ozjheljo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yjyhsekp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbcxxdwk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2onruvhrn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pvgmrqil.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2frrqlxmo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2iwhkrnwy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fgvzefnc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uhbgeocc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bbbmjvdx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jxisxxak.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2iypmhkug.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mjsuveac.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cceojocu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jmzseuxe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2cefixdev.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vzdagfvc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tpnrwisv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lkvmzbne.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2awsxoaqp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rookmskz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gwotervj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vrkkktst.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2uzukstjn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trbyettw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dwvnlizo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nepjyrzj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2unrkqduj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jrndlgvg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vhmfohuw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2doagbmzf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hiqprebt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tmzokvbw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hrwelnby.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zdzbwqhs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vjiroijc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zydwevxv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kyluyiwi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zgfejrbk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2osjydhhp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uspgfnaa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sokgszrg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cfjofart.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fumizumi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2sccbkjrf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2flnxatzl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2udjvlqeu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wawwxqfo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lajbwhtv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vlognkfh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xgixmbom.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lmmfsocq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zgxohldz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lmtcmwha.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2glvcgism.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kwagunmu.html


<!-- 参考信息 -->