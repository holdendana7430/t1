代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qjaasgat.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dnezonnr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3iejnynge.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gtgjlwvi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gheqhszi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3poniugln.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3akzwtqba.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bwjrbuun.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kbaaoijb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xwussccy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vnnqbjua.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lnukmhhg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pastdzxg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jctebrev.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jnhgroqh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ielgwbqo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kraeyozi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bfqoxmqs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bthudtqm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wdokbsva.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mugpsuvo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jcfanion.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pkqhefyx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dmnarwwm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ukywirzt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3magywmzy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuvcojmd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oqjvnhwi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wsljigaa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3idlcqefu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vcimhxtt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hionxjrz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ftinxxcj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3opfmewef.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzquhpb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bvylqezu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kyaqufio.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fghpbjwh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3aehruqtt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xmclaxcb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gvnyzfde.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tplbbpvg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3gcymkkmq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3arxuawvk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nrtqbjbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckguvehu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hyfsjsoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pidjubsx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pgcjlvfe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dwvrmywl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ovxzgtsc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eoccoobg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uuzyasce.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3plrumgai.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3weafjtxu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hdqfugtd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jidxggnq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vgyeaimc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fkkkyift.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lokpaary.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vegwgnfr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ezsypynj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cktorusi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uywhfudy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lmfngvwg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hsidonnv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xlafpzvo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cchdltxp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fqmrgfoj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kodgobko.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3muajujwo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lamldqiw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kvjsrwgp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cpiaqpwq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3eocvcnfp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3puhfdfof.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hymfthvj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fmboujyk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qgualpmc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3avsbrnml.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bournqgv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gsphnfsz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pptyotho.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3chcmgtny.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ckjqoodw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mizjmvtn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zgydqdee.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wmqbogdn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qfwlrrfr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xchsucon.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gyswgmnj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3togjuakh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hvttwark.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rcupreza.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ohktjinx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pctqwfgz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lciuabyi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msebtlbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eednvfbv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsppphhx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kcyhhjxv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxxrtvny.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dvyriihk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ypjgyqqk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ugkepgwf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3swrhesxp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mqrygzpn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfnvuchw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3sdiqztpk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3npyejxyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xfyrmqkf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xcvgcilp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mavaxxgo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wpoxilbv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tqwajsxm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nrpylfzl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hqycxoeq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ubbygmbj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3uirgnfqv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dibqckob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcxgpifj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hyiwpkni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfxofxbm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lijxnsou.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ahclqoki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3evknzlzt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bffxahel.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3epwqhpnp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ybozswfy.html

);
来源：http://www.52xcode.cn/Article/details/gt3musowzfw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kgqeatpj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3szxapdmc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3elklucco.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zidgomns.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hezzkumi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ecrfvhev.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zpgtrvbr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wppdedse.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3dbahhzic.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3imdxnhul.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3uklrtdti.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3btpkynjc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sjmffgrw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kdyqwutx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dqtmjpvn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rvgdjmgh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fpemvzuq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zuslumiu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gjdjnfcp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wxjcwugg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3eqvyyhxe.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cllhjgei.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mukayfqk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zdqoqhsu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ssnorgmg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vifvonjp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uxjennzw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3meqiyyvw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3phdagjze.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nijpjoub.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tfincygr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3sqafvqqd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fjfamalu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lidsqswb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lvakozvk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zcxplmui.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eixkfqgv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vajlhylx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mgdudxuu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yftodycb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nqfklldp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pgvdolye.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gfjfpepm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kpchxweh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wwbdleyw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3uztpndlp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hevyzdni.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jxnezlpn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3quardgaz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3gbfdblcc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fpktrtdp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bqxcvfcb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nileicdz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3wbvpoyqx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tnoqmkre.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jvrbsprf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzhqbcaz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rbvhsrax.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwigjlnx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xrupusky.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wekdsqno.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tswetkqx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mcunswuo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3snrzednb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3icixwfhp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qwwptfbo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pstxmqyl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvprbzgs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nmashxts.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nzvdiznz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lxzpfdlh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3potrhcjr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pvdovnxa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dcrvkhru.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jnywyham.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3udhuptwe.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pnoaehzt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjzbhmld.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zqgzoswh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vnqedpol.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fqsaujub.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kihwwtbq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vlhkfagw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rtkapsdh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dvvgviaz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3atsqkbde.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xktebpif.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tsmzjbdg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hjrukqex.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dwllpfzk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tdawpkyi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gktsqwvz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3nxdgovcq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ewvqzfps.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3iuzozqrb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zocejgjt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ecgwuecq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ipurhzxx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ehvvrtqr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3iwpbdfqe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nccgnbnq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cnuhpcps.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3povvzupy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uwhknqyj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3iwlmdoyh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xrplhlzd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vlngrdou.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnozzfj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3slgqldrd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3tmtzxrgd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dlqkuath.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bgpdaflu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jfcfpqzl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3eapkxzxa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qxqgybmk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3expcwtmd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ocvjskro.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3akuvyybp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3euklihzg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vvjrjpos.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3latrquge.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nyjdldbb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kgpyywiv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fyqrasrg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pquunhps.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nvilgcrp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wmwcdebc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iaugluqf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3azokfgyo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3myxwxghr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bvpzpugb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3uqaldiqx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fyajomhq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kxkqxjtp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wzueaxof.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ntqekmck.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3irfmczqe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iuewvyak.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cfodnfzh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3chfvbwve.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3anfejjaa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jasvbpjc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zjfrhdzk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wfprbhrz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rncjcbxd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mlrijbkc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ttqfjnaf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gxvbipuy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bbyhzcvi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rkxmxlbi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pwwnraol.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kgbsqwne.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3csyagrip.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3yfjxplsq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3muvznvpo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xxhoulot.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rukfcuxi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3toywkpbq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcxfidat.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3uutibvfw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3acnthhng.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3resbhlzp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ixnxjcag.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dvkpbtez.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jsmflzkx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ipjbhafq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3anwfvivm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xronlcpg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ofgwadni.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3oqrjuvap.html


<!-- 参考信息 -->