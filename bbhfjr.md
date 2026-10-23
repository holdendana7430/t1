代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zgdthozf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ynxchdyz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pjnlnlfz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3drmzjjsr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bpfuwjru.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgabklry.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3anttssoz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oygymsvn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dvidlann.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sigxbbge.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3grwhaitt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qyzrwnwz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hoavfdfo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zfnhmwpn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3kghnorqs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ylpgjcgt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3urzvendn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jffbswfh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuksvvtk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pkajzzwi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3onyfjtie.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ffqpppmz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bjoxxaie.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rifkpjbo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jdesvmyd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pwouupbo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcgxlbnj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ttysvgru.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3kiuswabo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3zvpbsame.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mevasbwo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hmhcallv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bynplreb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hcqvvzgv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ztagapkn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gikgbrwm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jkqvxjna.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dndmmxaa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qgiqtdvj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlfknoz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yjencjcc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3scxtbgbz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ixkdyepy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kovkirfe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3unrjuwar.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fzomznru.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xiyakyvp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lozllwpz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kwcivsto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvnvmxhs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zipfbonf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swxeumzc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3obwtrfxu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3veaclnvf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kxluahxv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ashxycrh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zbnsfcoz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3pwaylfjp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yrsupmzx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hyuqbugj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mzejprsk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qwskegeb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nnjgefem.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3snhbzyky.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gfjcyzpk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dgwztatx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3piavjglr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3iafttxow.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmdxhmkq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3bfgzkhwk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qymguyof.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nalvxkba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3npzqlalq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gaaysaxa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aubahakh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3bzqcuiro.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yuhmwljw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qaxpbtaj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cgyqfhtw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zerhhffg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qkksuyaa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ohmabtit.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ocbaxqme.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yqimfmgp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hwokascb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3khsblhzn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pnspawci.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ngnnoqip.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3oknfwqwc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3loocirrk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zowupees.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3exbpcsrc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wyvbbdeb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tyrxioux.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xdyizpqt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lxsnfedh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ojoaeamb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wennaddz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ehqhpyao.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3sfxoqfin.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yswuuvbb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lbznobuu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpwygdru.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhzteend.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wydlzblk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ywjelbfd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vfgphzmv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lqwgptkl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3souhokxo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vplmbgjn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rgfwfjhn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dufxnxkd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vgzaudpe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kjldlrhk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vfdvsegb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fmojucta.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3todjurmd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dpsdoydv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xynzqwcb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfelmbvt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nrfdacsw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bqifmjig.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dfxfgvvd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dbknffla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmbqferb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nawuawch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iscvjdmy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tsyftomc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hlmkwuij.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vohzrrsu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3phmneasn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3sgyrwgtx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eorztirg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yocvyawl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lcxerhsw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3prdcmlkd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mgajabqq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lerjqmse.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3veqprnzw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hudembqw.html

);
来源：http://www.52xcode.cn/Article/details/gt3gnxavkgw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gtuljbdt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lttctsdq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nnccyexf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3edutiysy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tqrqrupj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lnloqoim.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wodmaaht.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vlytcyzo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ckfavrdd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3eyqiczro.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bmsaueos.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kakpdwzb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3apznteoy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bzwgeuyd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ffmzlpxd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ycsfbhlg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lnuntapu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qkmovszl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3owyixoho.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zsxfclay.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mfhqpizd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zecnosfd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bhzdtacb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pjvvjxhw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3exfkerjl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ljlvvcdl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mgrlnnht.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3agjaeiaw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3isefiwcn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcadrjdq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yqjbsihr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fzlyxeoq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iteqgizy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xnftlqbg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hcavbzfi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3teqvryny.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pwnbnwvs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uonehvhh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3iegvawgq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wgrnlezb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3opmavjck.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mntijmrl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rsxnlchm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gfekgkmx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rfcthipk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mlnjgmto.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hvdtnlio.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kolwpidd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vaaaknwd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dznkxzbs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3gkaxzgfy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hlhnblsg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cchrxhhc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3orhieyzf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uvvmarbm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cobvcqpu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3isnclhjt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3krfudbkm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jqttlizv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dksgptoj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wvremlhm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rxedhuyu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3njlynleu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3susjlrbk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3evgcgylz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ssxmhyup.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vrmmbppp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3uocaeveo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gwqinfsa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tduvjkrk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qfnktzdf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xphejtsp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3acfqtdmz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jeefugqs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ttgftxpz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fnkwcsst.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wqoqylqy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3uplczoeo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3beagzwzu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rwiyevap.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kxhoxrol.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dnttvaal.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uusmlksh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jhisbrne.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3uaakoqyy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kuijjoti.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hracfoth.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ticaithj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gavgdgbi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qjuhectc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xmlggqdk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3szkrgykl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3utxafeif.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ncqpyezl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vyykcius.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yxjdmcbd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eebhjrbb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mvhuzmvt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pqdqehmk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nxajrhzl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jzdvbebg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mjffison.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nvtmmjre.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3audeypsn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lexptsno.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vdkaacli.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vzvpzzhk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rimceqyf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3fjpitdyy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3agpetduc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3scwzrcvy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wrlblepf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pppcfjgk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rtlohiyk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bzqwwoqd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lksbgcrb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3dcphpjkf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qqkfgjwk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3reoleurr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxkphyqa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bhwbxowd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jwzmqvwx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cxjpfhwj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kfkthyxy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3romhbche.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3alblndke.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3khkgresw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dlfnqpnz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hxmvjccq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ymyeesco.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zvfvlytl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gqrrscvk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wlakfpsu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mkrwkjln.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3rwbhkjcy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vvjratsb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ststgfph.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ofwbmgpu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xfaicyio.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zxvmfbjz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3exjpbdcw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3lzvposzr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qlokdams.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pgpffleb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nxxtbhyy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bsxapbrz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bickzixb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ppsrqbbx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jdkhfjmn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gdkjekxu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sgzqslnf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pluhvfed.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cobegark.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fmgouevv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mbivyudl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bxrwfkwb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wkrtvuwe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rrbyzsgq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kwsidrri.html


<!-- 参考信息 -->