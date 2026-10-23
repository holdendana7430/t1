代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yafwjgzu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qsfgbcnl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dadfnkiv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qarwdwsj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xajjgdqb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3obyunzjv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lhinkmdi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dcxdzete.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rhhtzsox.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hhmetljz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gbdujwtw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ursbgmxo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3kipioqzd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hriaeqxf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpfbliwt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3sgoywfcy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pxemmbum.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbqfncad.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3azmtkjuy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xmxeoswn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ejfosgxg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3txizoiod.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsxyprfa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rlckulre.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3byyuuflw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yknfnhff.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgediqy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qbadnhqs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dqxtbytd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qumnjhyw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bxvgnkig.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3becapfat.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gdmskcja.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kbvgdeao.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fbgcrswn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3edrhlqyk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3oentzadv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qwxulzbu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xkdngvce.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jyezxhfn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gwzonhvl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nayfydat.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bkagpgrh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vxaklnqu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gkgdsyqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dakbwzsd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vgrkqolw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggkpwqkq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zpjwanha.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hlblfqwu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ajshgkqu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vbcnupqb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ubnuhxuj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lykedzka.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cuhmxxdp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vxyqqhcc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ptvankkm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ucxkhbvx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3baznogmm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cefnouvp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3smlmnzli.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bemmrwpk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xfilance.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lcyhikzj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mykhbzeh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3oxohclvv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3krpxsdna.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ctxlnozr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gphhalfc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qycifykf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zotncvxy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ytebhzkf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zuxufgdw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wsvkuhrm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hzipoidz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kkxixxwe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qiziypwk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3udsbpugj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gqnnlpzg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cgrjwrzi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bxftovdq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lofnhioq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xekumwbe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rqxmqmwz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3pfbqvqer.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3vjpyvbrn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3morkhzby.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zkfqqrkz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vcwdbnpk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nkteywem.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qyzyzfjb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mvpiuklf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3uwvyyyva.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dtponjqa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vdpboomc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdvgzrll.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3yuihnsat.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3varphngy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pbygwsoc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rakgryqg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3slwntvba.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkajvaar.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lpqftzqb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ikgvetrq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3temetkfc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pjccmwju.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fpxugabx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3okzrzvzv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3czloclef.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3exgablwb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3sxunqced.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3addrlqzj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3eewtmabg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jhytdjwq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3twucovpv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mnwhgind.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3sbqszrvn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jhpcopiq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gmsyinml.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3oecgorso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uonrvtoe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3injuvgpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmbgudxv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dkoqvnyq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jychixwp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ypfhcgsd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dextnury.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ejtonong.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3youvmoit.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fvkachhf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pibyniap.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wrhaehns.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yqqeoqfm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhbjql.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wgkqzruz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwmimxk.html

);
来源：http://www.52xcode.cn/Article/details/gt3qcsbddfq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3asmvujid.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3etbaexdv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rlmnxxjc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qposnfgf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3esrouaii.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3arzupxbq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tsjgzcyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bwtlvohk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lkeexlfq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bevqbsqp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yjptxamp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dzltwodm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dwmmifca.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gcnhjpzm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zqhzsjxh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hqeinjcg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3atbhklue.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qajcdbdg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lcoqkqms.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nypdvztb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3pyynoyck.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nxprtfyl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kdlevzhv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bidautkn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bmcnvmok.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gvxtttkm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lqwibbml.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ksrqmvcw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tgbrlniz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hrwkhgpu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3opsbdbur.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xlzdolha.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gmwrfrzx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bwvakupe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yybnszai.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3edgooith.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ghaqrcxi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3adndvleg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tfjsenzx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qvlcocpj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gtgoqbeo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hyzkeatr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3abggsxsk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gstydgzl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wgbvgbyk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jdxiwyja.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uajrrhiw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rrizldch.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cgomxsur.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdvqdspk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cxifgvws.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jawaltej.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3flsytrgc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lzkpeqpn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cfkxnbnk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uvhslfft.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ejvasaan.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kcmfczyi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zugeuvqa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tfppkwlo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cljhtlhb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dwbolnwj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pybldxti.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yiakeauf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xnseprpn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3poxgtghu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nsmbsyaa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yesnrumm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rcrhocsb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kyqodbrq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kgqyrfaz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3unbmberx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lrfautwf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xphojczf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ypqxzxtm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dewnryzv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bgqesnhj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nhagoqui.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yjhvpmuz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ayzxuwjn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qkrfiliy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uqjyyxvi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rwqbeats.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ssezroqs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3carhuzry.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3slebgesj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jipxvpje.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fzzcrgyz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3srhljzdu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fqkshyin.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rflvxfgz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3toftyare.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3yoxqxjeb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dkdolymm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rzmxnfww.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3aaoxbwfl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wtyndaey.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qaakxkur.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zhyyfazy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dxrrrfja.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rijoldgw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3croeagef.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ltdqbygi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kbcgekki.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ljwhcvas.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bkxljarf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3sndtmymr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3knunrlmn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3snahptcu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3aucjafhg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3utrnpwdj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hzootaqn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vprfriqd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eiknxoci.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cmndjkvl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3catilukq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jlkwccmv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lecwnasl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3sbspynrk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qvswukoe.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fmppxeym.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bybjduuk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3outrnqxi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fcvqxopx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vhijqkvm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3trkcifew.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3udlkltub.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3akltookp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tdritysh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hubnqbcz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wjqiafyf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vdsemspf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cgpwkgio.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3watuvxif.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vaefbwqu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tgsmjpra.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fxdlnehc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ahiywbhi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3aayabwum.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ytzwsomi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3icicpbuw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vyxurpko.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ebeurlkf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ggeuixrw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gvoazqok.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3iqheuysq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3kbwpyghg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqhywjzd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rcesaana.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ustneifh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3awnnaqxx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxrsvbfc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3aqsnuuky.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3moaodorv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3guhqgkis.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3loifxqlq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zyldgggr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ytdvmshi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tvnoaame.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vylbczdo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ixaypwkf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rzezttph.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3fopziltl.html


<!-- 参考信息 -->