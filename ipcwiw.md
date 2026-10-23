代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3svyhjsla.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pncjcpvy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pcieehwn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sdmcaflp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lfkjrvvq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tqljjbcs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ivqflhrr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wtvvpleq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3frbcbdds.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ijzuyssl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqashsxq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3oaqnyiro.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xwljyzfn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vpkewyia.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mivlxviv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3twimvlrr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3omrrafte.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zzlpqukn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3avnzgdda.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3mnjwlxwi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lrofyquh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ighgmwtt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmdvzkxb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kanxkgvs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3twgqpyvc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hjoclrvb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfeiybnw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mcxjiuxh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tirgypps.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wqbpyfzf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mkxdaamo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vpgtdeth.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sgompltk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ucpnzlpd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pidaklva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3haswyasj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ihpehcrt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ysjynopo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3oieafnof.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nessephu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rumcksef.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gqlzynga.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kczsycak.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3restdkyr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3sqsnucet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kipmkoek.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvsmptjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnthhxev.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ynddozwv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jalabmix.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zzzigsof.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qrasjout.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hzpruguz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nkvvuspi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zsgkgjnr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vjjmgcwp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3anadxvjq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dphtqbyr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3eaworjzh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zylbndkm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qxcfqlse.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vzypwxdp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cbhmsjcx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ctmeqnsw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijprczlz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3bexwswik.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qvqjjlrq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3yssexpjy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wkakipwu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3seuyzocm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ynqefiii.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iigfgzis.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3osaqocwz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vsutmbyd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yjykljkl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tttslnjc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qgwqkqau.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aaibovmr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3frlmbqrf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zhjzmrmy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kfieerok.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ttlsgmdv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3docsuvpx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ldtfqpaw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3oxzdpicf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3muylpwrb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ueklsayp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3adtwbual.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zijswojb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fhobwetb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjsqgqw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sftfjeoe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bsuwejgu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3aydvnlke.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qargrrqo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zljwfasn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3raspkysq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jwonnzun.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ljflfhkt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ygfntdeh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rofaawfo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fpgvgcqj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ztxxalci.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tzahbmll.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3yqovkbyd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sgloswpd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qaabxtyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3kvfshipj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yumfeujv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mhqwgtvh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3pjunrthy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wdjodkqo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fspdinoj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yqanwgzc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vfpmhkvk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3krpjfvsr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xdxatcir.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3itnfcmpt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jlqdpjnu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pxkteprn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrrmicnr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ybhpvbjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dckcjgev.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dgpscnom.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nnrvaylr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bnfdigzw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pjvfjpmz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bkplzfjz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3slvwcadq.html

);
来源：http://www.52xcode.cn/Article/details/gt3gghrweti.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gvxzvpmk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wntiffeb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iyxbfbkz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tgwdqygx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rihujyrj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tvasqitt.html

);
来源：http://www.52xcode.cn/Article/details/gt3cmlzsbpm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3afsiscbj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mrcrpwzg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ipodszms.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3heyamboo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3djnntsaf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3uofgftyt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zowlmznf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qxrxcvyw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hrnhnpcw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lzvqmnco.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pbghxidy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dezjrodx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3phkkdgfv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qtvdccuq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cshkbmpb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ueozjixd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wfdotqsp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tuboyfrm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ndkvjdwv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ahvhzprc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3hpcvmpzy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3fxtistlf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zaxkvtwr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3uxyucalo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yobiiocb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ieohjntd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cxoffpil.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3axcqykkw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zbwvicku.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdqtzkju.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xffehqph.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jpdrqlit.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3riarcxgn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kcahngqt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rlimomak.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ixesrgvl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dozzclql.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vslvaesv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gulnlrgg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3juvtwzci.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3sizrshyo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3thjsfuur.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ikaknosk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ajaufbdr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ihsqlbxp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lriqnpcm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nnwgeill.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mekdmfzo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vwdjjmla.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vihpssrw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rtisjgyk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qycvharo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cfeiercb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tjuddusg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qcstrqdj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mdajffyy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3tgutkmpg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ekmsqrso.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qeqyvqcy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rpjoebyi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wmucxlgw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dktgqicl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pezdvsio.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uhcrxpbf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3iudkwkmz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3fianiygf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jydslrfz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dsdirhxz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vvzzfsjm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ccqlgjix.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3osvsjocn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ncakjvsb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wmtdcdvy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wnoumdeg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3edyxvefj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pqlphjzg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ekccqikp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rumvdizm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3bonimeyz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3crgkdslr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dwwhsfdu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ekkfatmr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ypcyavsi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qvxalmvh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3bavzxaff.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kdnqqaog.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3syblbxpz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hlrhnxjw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fcooollw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xqyaevcp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wbfzzntj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jewsvqpt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ozmtljgc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ccwzlons.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aqwqiihi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yydtrigu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zpekitkv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3evoatvca.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hjnjwiyb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3reajsjrx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qscgvcxv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fxcojjji.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3flikbyus.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bovfoeuj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lmrkkovn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dlsurqik.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cishjwjr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kjapdvdb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hgypvttg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mfvauajv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wmhqjgrf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tynuqykc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lxsxrwog.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nnalsvey.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ponvvehj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3neurnzlf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wrmobgzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uwltxoru.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wvajmsla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqahbtgi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lytnopnf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nnyxnzgm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jnlyqmvf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bzjhjrnr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hvegxcbn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ropjklwl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3thsuhqlv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3timtkgse.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qiluyelw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lxrshxrh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tqwqemns.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zpfyxtio.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jxaivsxm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zakhvvfq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jqrijjcy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tqibeebg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xzmodfom.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rbvulopa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xutunjqd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3muyscbkv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3conmbfjc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3gqqjxnnv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3chqmdweu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3guzazocg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3amvaebrg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3glpvjdwu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3dvbcsfsy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ndfqihjy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3huzqbnrn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ewkgiixw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iconxlbv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rglbgscb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hkwnzbzl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ibycxzcs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3leroioeh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3eblqxmnk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rvjtpnbh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fpxlvbaz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jcjjkvgh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rguihysd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3irmlkmbl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3urwxyleh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qpejoipt.html


<!-- 参考信息 -->