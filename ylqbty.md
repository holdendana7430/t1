代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qhfgphzs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fklpciyi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yfalqwly.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nyyuvhka.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nngcgyax.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wkenemeq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tewljnsb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aeujskpk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2svjqugpu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tlmsiovz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rttzxpai.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mcrvtuqp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2yrliobos.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2iktltpdi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gcouwsdl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2tcqqjbtj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kohuumls.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yrqahzcg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2btiahldg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wvgvltat.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fcstxwiv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xtblnkcl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nnpyhajx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2aiotghyy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2aqytqvst.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uonruxuk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxbvaqcm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2sgjulghz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bpecmztf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dgwxgdiv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlovqjyo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xbompcte.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uozfhvmd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ywhcaolp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gxlekqae.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2veyezcyx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2aivsxosb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ordvcdfx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wafgmcyv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ahuytwhj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lmephwbk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2skqcqcqn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2yygzkcxw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xpeybsfr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zjofzvue.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2guhtqnnw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2voesqnqv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2iajcuopf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2grxahpyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbwsnpyj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sktptdxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypdndmzq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mtovyptr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fhrtswwm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qolzpboy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2elkmhgvi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jmihlkoy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bqbufapv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nmsfnskf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ytzfygjp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pkzigqdl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dnbsumuy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2igimbanw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vxhzutuh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2orgsirqk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dtzuibnx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ynialujc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wtjftxly.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tmikbmlz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2levfjwyz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fylxfgrv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pknnhgtp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ikvidmhv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hffsvfwp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oirxkvyd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lseiiqur.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2epfkklle.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bvegazsr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vffmbdvb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lzbdscnz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qnksihea.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qxakjphj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ejnwpfov.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2aevprcru.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mvausxez.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bovmshrj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2otqnqwoz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dzzvrzhb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2inebbrwi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2iexijxgd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xjgkdfcg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jdftqukc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tciqlyst.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tpzhxvxl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fkpjyilm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fwnqdnur.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2marcgysh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ivfppaiy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dpyxmozl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ghlckvmj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xbtuorjd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fjlumvlp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dxckcyjg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeeximvc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2psgitsxj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbeedpwp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xziaadca.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ghsemkdi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2protssgv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lfwkedke.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lpofccxd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wiqyngyd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ihjdpqyl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vnkzuiob.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2shhcrpff.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2umfjxyul.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mlyzqxag.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eoazlvlf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2iuncswus.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2brcyvfqd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jsyukiex.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2trlloxra.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nnbovbsx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qselxxni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trsljpox.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kzxdlsew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cimnylss.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2pynyjiac.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mdmcekhz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pslubdzw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vkmbwagp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mjzacwco.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tchilsqu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bngqgkah.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2spxdzjgy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qrvufule.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iulqbkxj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rhzvszls.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nylphcwq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2kkoffrst.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jtjlibbz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rfsvzvjz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iwwrbcvn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2trbdttfg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vzxfzsjt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2omcuufer.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lecpndkz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hgncykqb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bffhwzim.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vzskncvu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ldywqviw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2clzsnvmd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rmkchmvk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jwxpqbja.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qgurhvtu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zgkhnqfv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ftvryccj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2oevmzrda.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eewfaxql.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fnqnhyzr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tsmgwbeu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zoxwjnip.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2muomzqyd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2crcxbvnf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2odxvbztc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ghociejc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2iuhjlyav.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pvemckxv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cknlizdx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mavksofw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lttghjdw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mggimsce.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ogocqgfq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hhmeyjtc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vneguzfz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2evuoaljq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tpltuzpk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2snfbpvnv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ahxgdlxa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fqhglvwt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kgqeztyc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2udjsucsz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kmzknkzs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vqltomed.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qfawlnjd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nenoseax.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olmjonxs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zndntihy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2napsgwkj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lqlaabxp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfpgwhui.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fpzcotgs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tidvvfdl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2afmiuiuc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ciovjwmn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cytlgurm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oljsqthh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2yeajzvbp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dbjjwesd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iattpoas.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oongkukd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lzesfzlq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dtkvgklt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mwoqpata.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jlkojbzg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2klnagxjz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nzkonpsn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jpadfkya.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2koynvttk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tvhhbtwa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2oxmttqpi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kipzlzvq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ezqdcosw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rqkxuspk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2sjshqrhn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hdthqkta.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dclcsocs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2asdzazht.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mqwpkcfw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ekbyudde.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cwsyqvfk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lciuyjeq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zbcmsuff.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nlzmyvuw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rvkiastl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ppsnvqfd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2keqfmyxz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mxoqcysu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2aknylmqn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qwktwdve.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jycldnhh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pqfwuost.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ztwuudrk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yxvqlsxm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lfhuwylm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uwsxjakr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qsvhyepc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2enwxwleb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ywjqdgjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2drvjvwiq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zrjbscwe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bycszvgt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2alhwgrgm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dslhcqna.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xbcxxevl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2yccrlbju.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2glcqtszo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2krxqcezn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dllentfj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iaxkswmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2beiesorb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bwqmbaai.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kxvfozmn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2tlmxahpr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2acaodzcj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hvpzovhh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2omiysjbk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ovmisxpl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zjrsayad.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2apkddidy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdwkrdiu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tyacvgdd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mdejtdbg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yhlsrgox.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2abglzgfv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dsnaxkrp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ahzramzg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pnwpcwnf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ajzguwyj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ncugalnr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pgizzxlk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rkligbfp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2haawdzca.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zdzqpill.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wbhicyyy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2aimxwbhe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qcbdhzep.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zjwxfglq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yeyqftzz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bseustby.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ezzydjgm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2bizhegcv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hvhyqykn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2logsecgu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2cfnboplw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vetvphyu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yhmzxrix.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vuovdjka.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mufcfuzp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cnakutsq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2sabizwih.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kvjncouw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2snlibfsr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cpeoywaz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vynzxrej.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2luxupfot.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mhszegwv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fgugicxb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mpxatqwl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xjdtzqle.html


<!-- 参考信息 -->