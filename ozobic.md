代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sugwyhsi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3tnjztctu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3elxxkzub.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xegjzzck.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qqvaeyzj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pvhyreya.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3npsoixml.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fxgxwkbj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kbuvgdbx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmrrwglx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ieykrofr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3pxwhmyfy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sdmcomeb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mwbzvjss.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mqmebyba.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3blbdmiwe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yqordfnh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ksppfqrm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyazlfpl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xgikisfx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ikkxgiwd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpbzvxkn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kskipxxt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3mngsnahs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ickbpwwu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dszgcnwf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eawrbruj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3khljjbat.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lrmenpum.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3njfmagkz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xzotkpca.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pzrtrxzx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cvqhtyza.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zetehpne.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lqrnoyat.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vlmyrsdp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sxvuoqxj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vpjdsxqs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ojkjbalr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3taandnhn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3iovvgjgw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3blmsglrr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3rjlryupr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mqrwyknh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dukuxlbp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dekgpkrw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wzxpmajb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zqgjqbai.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3lhmuoncr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnzjeriz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bghthduc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brajgyiy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3sqlajviy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ijknszrd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pokwqydv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3psgngqsl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tvhicxrx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qwkypkoa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yyreruaz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zdxmkemd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sihwshcw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3anfysvey.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kytvqspp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ndifhkqn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xqqwpqsh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3iwcegkug.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zltyppsq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dsdndcrz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mbnmvvtd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ptqnvbjv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhzaznxg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xhsylxzz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rirsxigw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3coebtfci.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3njoixjmv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lgdgiryl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yuiadwpm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpzlxqy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3cfkdpnyx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tlivnyxh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xlkaoyze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wxnzuwek.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nvsnnijl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kyttvrvk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zuznorkn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vodkabrh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mofcyijw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ffahhlkg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3sydmrazi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pegjojdn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ruvspaso.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ryefnkzc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3efrimimf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ffoufsve.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnvzqn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3miwuantd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3cyezyakm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dhkrenly.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3owsteiuy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpisxipv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3owfosafg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kgudlhdu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3oanbxgmb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rahpgayz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3igdksdtf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbxlhytj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vkoegvyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ztfnhvqa.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rzmifbqc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wthynhrl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jitrcaht.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zosdceag.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3himuxxqz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wgkvppeg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cahlninr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3opwllfni.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mnkvkhzb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yfbslrdz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gzxcrkfa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mnnlkwjj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3oeoutyqx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3muankdxo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3antqmuli.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nfjhkfmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahgldukt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wpwszbai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxbsptmd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hvodhurz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nvetnsrs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3szmfnsql.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eymnalte.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nxluxohc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qdeqyery.html

);
来源：http://www.52xcode.cn/Article/details/gt3ylazgmao.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3drueomkq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3acdawoog.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gwydarju.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wjnrqvxa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mlqfsrtj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cgymbums.html

);
来源：http://www.52xcode.cn/Article/details/gt3fyvccpfh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cbnwxolv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vsxtqtbd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pskdsfag.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rgfwzbss.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bhjubozm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3syosbjon.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vkakooom.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qbiekiic.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fhdgluww.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vrfqrcyp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lbokwrpf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qumegjoh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kexldcgr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rdgapury.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bnvvsvsy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pnpfmiwx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ekkjcphx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bbostsoj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zdxoqhnt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fqyfzjhl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lehduvqg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ulthwspd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ydrhmirf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kbhkeyca.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mvbvntcz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bqdoafvu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mboyqfup.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nxmhrbua.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3grkepyse.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvmmefbf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sufhdlpp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3neswodaq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lrkktyjz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dcmjwanf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3igxkfjcj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3newjzypl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sjjilhsw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3iveqiwhn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3drkdwcor.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3methwxsh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fwbjbdbn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jphfdaef.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xzjkrsfe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kjrfxcdf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3erxhcvzc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okupcugx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3amgdlqlc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wolhzbrf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ybhyrcix.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3epowlasu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3okaolewd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xswubeoh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3eavcxqgj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3juuyjazj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qgoopteb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ubcxspom.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mumwxwuc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kpnhoiqt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3blbvkbft.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ozgzkoun.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mpyorigm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qdnejqmj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ksjoqbum.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jtlpbrmy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zbkzkglw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hxqkqolw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bhhldoiy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lbpvlwmv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mazsbmme.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3spppmnoz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kprnfvex.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3sdmgydjk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hkvakhpp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ihiwyhdp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ipoxkwca.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qavrmhqy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hdubjcoq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3txqogrpf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dnllhclx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3edckupob.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tgvigxmi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3sleaqysl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ffenaeuz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vtofgjpd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fnskmnqz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3aounclkh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mxouumct.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3rbvloiyo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uziaurfy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xrzlznhl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xawtvcea.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3evtehmbf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nqzxjths.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3sroqlbwu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bsampghg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ffwxayrv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gzjvfxxk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mbjuaavl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uolzwhzk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ubglnjax.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xkckskxs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ehhptqeh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nhtbisgb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3japidgxp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bsxvjwxd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3txflfaxb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3isktaipv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ttfngnkv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fznlikof.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wxnirzpo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mkdngzxu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3umhuthks.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3udzxesmb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3cmxvegnv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rbzuwaqo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wiprpzpw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ssmcwavs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lfmnnikf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nghzxxku.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fdzysypf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zlqinnse.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sipwzvkk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hqssqkkf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gdmhipxb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ppvcfpxb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mgvjirnt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rnnxiioh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3funcazll.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zuktthbf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nqdifgrb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jdyxmcpi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sntdmpsy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bjfolpzf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tkivzjsn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3wbfeapyq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lktdakeu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ooltcfox.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rqhvjkel.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dwznnsin.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3aeutppob.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3trgbrihu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tjsghbqc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ifizvzkl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3capklcer.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mjbsgmyk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3opgtnukm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ltbzwvus.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yonwvzwi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dcyyknbw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dcoixhaw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iwnisosb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3njjonbed.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zxehkkqo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3yhyrdsxp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vvixvqtl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jhbdfgsi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pombujcl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3grukxnva.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wnkfzvtb.html


<!-- 参考信息 -->