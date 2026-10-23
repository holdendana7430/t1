代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jcopalpd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qkhntjeh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jiatqfnv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wqfmnfzo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jxtetmwt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3cfgvqyzf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tudsirqy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fhlmsyyp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3dwdzwyia.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdbolya.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vtjhcldt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nmqowhej.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ehehmemq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrezlvi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fadmoggo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3haomkurx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gfhyaqzf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hjwzlpih.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3grbnvsic.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3anfotsdn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mwmhwmxu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xtsacntv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnasbfmt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3sdcpxkxu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3aclzaipy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gibxhyks.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ksvpbrzs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ihjipmdc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3apsmmqwk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3suqcuxpb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tkzqzrio.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wtsqqoay.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ehxvhsww.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lirolujf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3omqshxhy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vczenuex.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lvoqbnyx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3yfdsqdnl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dkkpejdr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yqbfcqtj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3suqbtrzs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3nuttmutz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kqfmcqla.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3gmjbonpg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xhumpmzt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3smmudyau.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3iuzugbpv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vguslkbc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bkhcehlj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fsloeoyh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cfxapimw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fyobdslc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kmozxnzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtdcfsyh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnlgen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iejzmlna.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xesowrpv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fkphhyrt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qtnjpbyi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fauigkkc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xoislopp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gluedsmv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qdmevvuk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ephzcvto.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3aowptbxd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3konzjbrp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3aftzqmls.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pbjsausu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qntkcjsk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lsywxbbz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vdvisotq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3himbbkgv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mdkywpux.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zjqsmmir.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yduirvmf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rrbtynkc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uqkhgnxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dihrrjga.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zgdeyzdl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cllostwl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3igcxllpl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jcebnhns.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3bloeiogm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3woehivyl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3cxroxcwt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wsmvdvdm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ksslzfpy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ydvoktuv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hwuholom.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dcjgtavj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ifwbjqyt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3voepeogg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ehsqbbwp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3uiokmtfv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tykuaevi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dabckubq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wijayljh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lswpsnjg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ikcfhear.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3eiilhjsr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tzbeqaza.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ufzskipb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3efhiemnh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vzoilsro.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ywjmbmbb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ikitwadh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3optvecna.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3glwowdcx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tugddnqk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3saipktkp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3eazsxtvy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3szcyfbvj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zrqejbkn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3edizrynp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ttfudtuu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twpimisk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ktpouoaf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cofkbehh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zkjkifoo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3iqqcdxud.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3drcsmaak.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qqhmylfc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bzfzndrz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3valzfyco.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tubnvyon.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hffznffs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wmbdpsbn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zytapsoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snughjhd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3smeuvdyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldhquuss.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kllvqgsw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uggvfmau.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jfbzfaco.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tltgjivp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zbbqtnys.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ebcfkjbm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ormvrzwo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3lylsoacl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vixhuimo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ivfhimix.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oohiolgm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kghbozsm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kycjodbc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tspziaus.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zytdwjsv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3eonyqglt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ubijkusk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bxsrnhuf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3crbggsnd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jqvrnfph.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3haeeonfm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xqfpptoq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kkxiromz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uhxfgqhx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kqrvkexi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wojrvjle.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3bdbitpww.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jwhoiagf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3msqtnpha.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hgokdami.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ucbxopfz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rrrempze.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jxortfgr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3knvfxdyd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gjuxrnmu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zvrbwdqz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cpmojikh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xlahvrqj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ekyixhur.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nqmgmypz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dakkjrfh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3poykmren.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ggaboffj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pnoxykex.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qcuvbldm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wcufkppb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mwfrzxds.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3glqyfmwa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jqghyalk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oyfegmra.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mfbneadv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iqelpmgr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dnprefgt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3iupbfnhf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3nnsdweib.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3suucqooj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gjpgqmnr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qtdkugwn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3feccelsn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtlnnodt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cenoikzr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3htfpwgnx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lxbzoylh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ehrcgbip.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ayihurzi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjsiinar.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3snntxggx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zafoqvob.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zmsfkuod.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxpqloxd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vfptbdgv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3axeuttri.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3suupmhcv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mxmnmzca.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tgtkupqm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vceflhza.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pebyrzvh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jqxptqgt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vufotwyg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hwydqucc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ugadwjbi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bbofyxrc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfrfbofm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dmnlgjrr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xnnbfand.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vodpbthv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ondydmhr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fhbsgtyd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bphxzsrn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mvmxvtmu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3newyvywp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hawiwngh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3riwpcipf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ceaqzloq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3aihfqzoj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3fnhaeeof.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dijlddwy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3onsyxdqr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3efzqskjc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gryzjwrr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ihdxocpb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lpzdjjsl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dwnaclkt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uzpjuacw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mwkzefsj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3essivcxf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nthkofyc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3sevzwozj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3frvbbupl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jvcpdnfs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fnrnwhog.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xecxlsjx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qjhngxif.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3laozeqwy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kbyyqtlb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zuhawmej.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dnccybeb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wcwzgkfa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hkutappd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rvjvwqup.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yngmjghl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rwvtzfzd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cojutpem.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vcbnqzsj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3otpejqdl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3eobxbttv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wpyhhpnb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3odunzbjt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3riwkcyhe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3movqzhxb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fomltfvh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dapbtuoh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3erispnas.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iojchsfy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3akpidhkb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hfszxwih.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jpyzscrs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mtvhqmcl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3iczmenqo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qepfunww.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3npcmgqvz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jachgfxj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nfxxsker.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lcjphivg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3thjopwfa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bauumsmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3srrnmetm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gapckkra.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ncxaomtl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ovrwfkct.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bdsywrrb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3pegpzkkv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3aughevom.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3onpnfmin.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3epovxfbh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cvpdjvdj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uwcpufby.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vpnokqfy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3amjtaghf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gbalutbe.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jcppuvhe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ujzzmjcl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3veejliqs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jnypirke.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fyhqcwrb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmysnzsl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zzkcigtp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lrfvxped.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ysxjrrtl.html


<!-- 参考信息 -->