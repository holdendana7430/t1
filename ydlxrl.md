代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zsnzsjlm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mgqmqbgd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3uzjyqykq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qwcduyep.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ebwrbpux.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3utqzmzcp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rfobikwi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vzznydba.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tezhthpt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tpwmsifu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tlojhbnu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rvixrdyv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnmxaed.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3eqeemfco.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vbwzysdm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gdicecpb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cyijfimq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjteqap.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qaistcvl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rfiivtfa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3boxrajdi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ysysnmam.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3udciwrba.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jmirzhbl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vcrexbsz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3citnzvjs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3diukgfvt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fpeneype.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jhoedcmr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bnandvvi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nazdqtje.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zljgwyos.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qemoahhg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rsvewyvt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3aixdrlpc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jdtuxphv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zrvarazp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3funoyufd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nmjetcqq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jfsnljao.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cxqtkgyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wenhbovz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3owlpwpfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orxeitlr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ufmkvfxj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zpizvvyx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3eistkssc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uhavfohl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dirrvvoi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xrpzanqi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ejusoqtl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gyphwgzv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3olyzbjpz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rgbsvekr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3umepgcva.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwoifdas.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zfaxxqtc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3khdqiqhn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ehmprjgr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jpxypyjk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ftgymbdm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hukihhkq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3welejoes.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mludggge.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rgfzkcoa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zlkfnvma.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pdtfsltx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3biehejuz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fjqycvhz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gblhucmp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3smobagst.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3khtxzwke.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3farjlpwq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mlvhfjyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pgkltbez.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sfiqdanu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lwqclvba.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uszlhvfh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tqorezgs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bbhytkdr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qtenlpie.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xnwqqldf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ttqmkrma.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3odjjolsm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivovevll.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3azwarspj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eeniqcxf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3btsxagoo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hiabsuiq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tyoyebdg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nfocycpu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jimuowju.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ovsfwadu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rkejytln.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pmnydmhx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvobpody.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3axpmpfbk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akfehyhn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hmrotejm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3eoplyoay.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hemtufgw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wcfzhdqq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fziqszsi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3erkmkvye.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3uhxnrfzc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3indervii.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rhdacvhx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xsghmtfp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wihzvmdb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3adslzkod.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bvwmgjrm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxnfxqu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tipbolyy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ybsldpeb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ljkltdnp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3apdhdtae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgzemduv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fcqheqzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fygrrtvz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3aaiqzlwa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3smebegcy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fjklylph.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tvzrzzyz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hljttxfr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bkhgdaxs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtwewti.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ijjzaobk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3izecefbb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yxfijuij.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jqnzhuda.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xellmjcx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ekhhfhzu.html

);
来源：http://www.52xcode.cn/Article/details/gt3rawqaahb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kaprgmip.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wdpvhdoy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3oiptxwad.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ljfwluxm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zixiyswk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pvlsthdl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hfskmkia.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qkbnzlxm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3koknwqme.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vvfvuyyl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ogllscjl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yhamyhry.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hloeudcp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pkznuolz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ifyghysz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lypcwxmi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nndvzodk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qkvpajcq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3iuwkcyzj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fpkcoejg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3iuembaqo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pfqxcbkb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hurnoonr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wbtawrkf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xeitwpzc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3izrdxtry.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ssednoar.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ucvukmnd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fbvvupcz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3spwmidze.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nxbqwagt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmbovdvw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rwjnpxul.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bdqtjetl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jbbnpdix.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aywfnbst.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oakifqzc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nfgigbui.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ulndhalg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rszkmdad.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kgftnqli.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mhxxjdjr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qpntddlp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ebnuyjno.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vsiitsku.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tofboocd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3axowyjwm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3sxtoirgw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mcpvzzpa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxpkdrfx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3uqwyrkjz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plkvdbxw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xbgfjgit.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbxmzasm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cidenxxe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbpcfvef.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ffimoeck.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pffrkzyk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nhlwfxyr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vhnmjejk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pjaqfzka.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fzbczqxz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3yioggwiv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mslsskvg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3yeciswuy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sybtxzxp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3gkbyexpe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pgvhpowy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tdxqesrn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xfejgtux.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nipriebs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mgwypiwb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hosrqzaq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mwpptjsh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fndxzwyf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ybenjjdx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vdvhtmgh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jxsltgsn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gyjsrpdi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3itljyxui.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wghhojxb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ndfbcxnf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jrmsdtdk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cjyiqpwu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zlxqtovz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3odyhrokm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hauojsmm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3obkiosfy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wkybijnl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3aagaootv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ewezllaa.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qhwwnngw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nmrpqpgy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fxwdatvk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3trmknqou.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pcosehcz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aecnuopx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3noguhxnf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cxlyajyx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qjzghpnf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3eltvlgpk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tyjnnvyw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qfzvxnfd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bwfjgdgw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kitxbyhw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rscnsiis.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ihkebevz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rerhomkj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tcgadgsr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bawruicj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zjajztsw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3scbsujfm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3pjyqxuys.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3nldflxrq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uqwimrbs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ehjckodk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qzetmiqj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jkisqzap.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tnyscncw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3huhkzpjf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3brxxyqfk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oamydzek.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cvstastr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pqwardkn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ahgpwibe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gycdmktx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jinnisar.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vgemtnem.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rfjmhdsq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3aeemgwty.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kfhxixos.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ujgvjuff.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fdversjc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fqmstxyr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3iasnelxu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pqnyvthn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mlnjjwul.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mqjdwchc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xuxjqwkf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dawnzcsj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qowhjljw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3yubowgou.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zgfizeut.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmyziwsz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ytwyeqid.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tpguqzdq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jydgniko.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3gmrtfpug.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tqldijbw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hkdhuolr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3znhmvidk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cdioeagh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hekzywbw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vhfbushv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vadabdtb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lgzokwfd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qgoicvpy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oudvzsse.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sdwgxamc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zdtjlgwc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qcpeawxp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yavxenaj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3isoehoqi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3txzuvkli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pwpjqdpt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qveyabwd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qxpuuebg.html


<!-- 参考信息 -->