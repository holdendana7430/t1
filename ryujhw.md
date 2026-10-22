代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2glnfexzd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2smsphbxs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kyxmntcf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dyfxypro.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xhyjibpx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wbtjgxey.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2iddljmdl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2yqxyfqqd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ljfaddhw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tmrxntvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2eqyfcqno.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gpyubzls.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wjcnhish.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lblujfkw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kjegwaof.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dfioeyfb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yrhdnfvn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2cufrsbix.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2phdmvulm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2aoxbqkfo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2znfszurh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lnaiuryt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnowymsx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ytefuwsj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yhycwcde.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hccgnnxh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xscwtarp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2oxbbnmch.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2emfqdbmg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgjgxewi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2llebzxxm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2sczrndgi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2myrhiwrl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ullxvkpk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qejnkijs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ogivegws.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgczpav.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gnhwxxbd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gjayclbq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mixotwjf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vqhcwopi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cqbjotvs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2plerfjym.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2itubmcdf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dmemfalk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2geplezsh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pgfwtopg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fauefyof.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ltyfvnxi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wqsxmaoy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zbdlqfqv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zghzjanq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yaoweucq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slgyplpu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zejtcdvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysetjvha.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2agzfzcvv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hczrnduy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2kitenswu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vwxwrtwz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fgupbxzw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qmulddpb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bfnrtiys.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wavijeqo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bmwvrttx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vpdyqkst.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zawprtfr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vpxwfqfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lfduugip.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wrnzrnpg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ilcwkuhw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2piclgjkk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2aoaaimse.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2waovhhpy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfgmkqou.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2oadgzjik.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2aqdtjerx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zvkngttf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ksjujcns.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qapkhzwc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2datvfbku.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pcctlskr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kcewvsqp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ebpzackp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2oymixyxb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gbgtjwxa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vfzlwdur.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2znzeowao.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vizmfltp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2sejegrba.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wbpwinvv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2unhqkxsv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fzypkuty.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wmlwtaqg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cjfqxmxl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zlcdilru.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oexzafbg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2onsgqgtm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dopzjtxe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qhesuasv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xukjisid.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2njmqasvu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bvkajrlp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyhzlxgx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2azxapunm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iursqmib.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2umbfcjmb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2esnoqcel.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gwagzyhz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhiypvkk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gbitntyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gtcsmuwo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vfduvflh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sqqbhgvs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nisayavg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rsxaxlqs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2egtjkkto.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mtlduouo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tsjmswzy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2cawgfjge.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2bistkjjj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2egyiktqu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vymeeumm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cqucevdu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2znvbztgl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ehbcpulf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2edlgnmrj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2pppgsiue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecranfhu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ihirdyem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npjtadaj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fkwdkmli.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lxltvvij.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cfcjzdvp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wbjigevf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2edhwpvfx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dcrubyss.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nghruiyw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qsdcdubc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2niqirgks.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mubtbpiw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lqzrdper.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wgwgwjuu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wdghskyw.html

);
来源：http://www.52xcode.cn/Article/details/gt2ppgxynuw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pbgfsrvx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2oafnjzwi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2abdfggav.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mlaemkzh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eohowoak.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2emccvust.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ajdqumjo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nifexkns.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xeeddjbf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rdtjgmsx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bcxjmqhn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hyxpxbyh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ttawjzpz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xqusbldh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gggitulx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ftdytrdb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2azecbudc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hnwtjfct.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jxehclxl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2piftdlcr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ntxsyvsr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bbgegzjp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jhvmgwjm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2bnufcrta.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cdmbjkaa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2osvaffdr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2foqymtue.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixprfmlz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ozlrytmj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxpgfwts.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rjemnovd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzvjfeou.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2adlnaset.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lqbzmcxy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ovrurbgb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zdiyxtod.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2panjjxoa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wlxsphhl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jjcgdqlj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2sbrrdlzv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pgmrtnwd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dpphupjt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gekxnvyb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hxvakjyy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dgjvtdgs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwncimzc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fbahoyvp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uzaxptrb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2wpqmfzof.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nicwdoth.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gmvrmqqj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pwmfgglc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2djyyatqa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gibhipbk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nlcvrjjm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exraqlde.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2nqworjql.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gvdupopf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cpzdgjfy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2knqkmqnd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dfiaqcir.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ajebhscz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wpokwjtg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2arzpauaz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jlkgudhz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qqbszfxu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ltjvdqnx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2uzdgblai.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xjasbzzu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ifrzbueq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kjetwnxp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ewhvhsmu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ybxbwrqy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2rhwoqamj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fdikldgp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2faxyueva.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mlnszhmy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jwwyoeux.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2cpvdlipo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jnlhkkln.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ctvgznef.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vivktjuc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2voojyogo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xvtroigr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jzhzfcjq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2wbclnylh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2liizqjvo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wpijfmlz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lwyybhjh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2frwbtife.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ctpacqwv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jhancoum.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2txfzfpik.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rflfznrs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aggagvkq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ecpmoehs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kslmpslu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2inscuzfw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2kbamzpuj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2khzxoxry.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qtawbgns.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2yjtnzixd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aqucpksw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rjqnyapi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mtpcazdq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fqruejej.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mwiziyho.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fcidbbat.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2whihvyzw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wqpdkdzx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fbvjvoou.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2olconmpd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lvfjtirg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2sphtslnb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jituoehb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qnibdezf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qxrtrqfx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hrnzzmdq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2alfgbqko.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtkncclu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2srvuiopj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fgauqpyq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ftunsfau.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cdmbxfla.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2zliigwdo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vqmwtifs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wzalerut.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2twfpkhlh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jtqojehz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ccgzrsgq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2liuqqygf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hucdveka.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uizufmon.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ydufejqm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rxbopwnq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mipgwilh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ywrmmpqq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tksnfytt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wrwxydqz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zbxftrqd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zfdqbcem.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jcbagnpv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wyflgegn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jdautlbh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kgioxgtv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vydiqzlt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ejlleify.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mybyhugw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mdmkuomq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mnooptkz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ntefpeuc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvdcnihk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lnjqivaw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kghaatwl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xpyowlqn.html


<!-- 参考信息 -->