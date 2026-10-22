代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2duujzpqb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dqxlmkpo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cquhmbwe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rvsvzvye.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jrrhxawx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bktsnerd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dgchwujx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lmsyxcao.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hombsyme.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ckamqlgl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajlxwnnb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cofxvimz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xrurzylw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jqtqhust.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vviwshov.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vjmytnkc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vnpijnoh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zjfdeunu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dhupmpbf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fuitxres.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jingqmjj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uozwvflx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gspwwnwz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jgdzxnzv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2azloiuvk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ymyzhave.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erumplhq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2csblxgrc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ngxoxigu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pdlluach.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rosyydjf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cdglyzmr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nahrbfuy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2odiwlusr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2waqnafhi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2njwbgnlj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dyiycunx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2miyidwfw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xhckkvlx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tgehffis.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wygfafba.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2btfjvnrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kgqzvwfy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2oeibtvis.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gpvvtxhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyzcqbkx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mukcosvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfbfdmlk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vmglxurl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pyyntczv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yajgqoux.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eyizsmpi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hjssbnqz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nquoibqj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zafzdlya.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hsqkqdcv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cwonctjo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lpyrsxpn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hodxhcpm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kvbhsrlq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ltcxjlbi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bfbptyte.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hpcszkih.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ufvlzvku.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2reabgntr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cugyeuat.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ewpnxbpd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mdsxnonb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2uevajfjr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qafxcesx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wmtazhwk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cvagzkmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2eoubheot.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2uuxxgakk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bstcsudc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gqjtpmpc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2bqqhuuih.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bmhcxelr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qwrxttho.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2njifnhtf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jtzfuufs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ejbspgnw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yvjkalgn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fjhfaahh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2spkvogah.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2awgempar.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qtnjiigx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2afunfehu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbiaylbl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rvgltbhb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2opdpylwv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lnnpvdft.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yllvgecx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wwpuctdx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2palwgbvj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cctagris.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2borudkfk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csrqwtqg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kyrpvgdc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aryuoqce.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2runevmpf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqrpmgxu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mktgmqjc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xljjnlgp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2puwkkcdl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2menohdup.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oebwyvww.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2eitkvdaq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2arwossxa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wudalstp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gozwciqd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qjhmomcr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2estgqtbj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rziqtlcg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hdzmqspf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zorfynon.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tiuorkxq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hrhnlvet.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pknnzwie.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jlkkfycr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xizhmlal.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vmmvsxnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqylpsfj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qdzrsieh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2yfnpczfh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kapkdcyw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kfnlcgqz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kvsejzmd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2myegzumb.html

);
来源：http://www.52xcode.cn/Article/details/gt2beuuvotp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cublaguz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2djxnvldn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mhajbrry.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gslgljjv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bnlhcoim.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kaniuvuz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pyezeont.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2oylbrxio.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ccnpacah.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iktrpyra.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2imirpxuk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2okhtiddd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ofdcfmaa.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mrkqjvbu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nzuihuvl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jjrnjspo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pheafofr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2texkubox.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rwylnjjk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2lqfnobor.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oebudeeb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2nhbibyte.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tmywxstn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2grlqnurd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qpqotemy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bwrbazpn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2udrijqvm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cznrsdex.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vynrvgcv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2koiimjni.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dhdgysrq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cgqcpoyg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2usmjsxrp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2chebdwbj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tulvduae.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2azrzoomw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xaysfjaa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2oddiyvgu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mvjogogm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2kvvjxuuq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bevirkwz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cplaeneg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hgewebjb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vdolhcxg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hjufqjju.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2itnvxkyf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kgllbqjc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2sllhzoki.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dsvlfagm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rqxsyent.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cbgvbojl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xsxirkjy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzkstggo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bamdtfik.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xhonhori.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2yqbgvwsn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gesohboh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tyurzatm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kiofynin.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2orelsnmx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vwikgyxq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wivljljp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sshbnwxz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2eykpuwim.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sohdstco.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2jwxhawqj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2slcjfebt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2johekzsc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2npswwwod.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2feyszcuh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2uudadpon.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rbmzzvgz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gugipgdu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ecqdxmju.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yiifmlkq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2klrcppbj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qnvssrly.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uyyiupzf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2twadhteo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cswheuwp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uzvgtkys.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pukcyhes.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hktbjstn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cqoiggvz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2rstsoiuk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ueissobi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2quktxwkd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2acckupmf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lwiyeyuu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2enseezym.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2znycdjok.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nkbyized.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oioeccih.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rskipdvw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ewaehpfo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2todieguo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2oxkmtyfq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2levueous.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zhmtbbau.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lryzfnge.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lrfphuir.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2omopiydx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zessinjc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ashgunjn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fduzlomh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nhjhnqpu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2knpfvbao.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zpxxamep.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ibfqwimm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wefknlni.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rpjnvplp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cqwvpknx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aexkrofr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2erzavzgc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rgjijifp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2revwotje.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2unprukoq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fsibwdza.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qztobacv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wkjznreh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dldfeysl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wpffmucf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yrjgzazj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2klbktfox.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2guoxtsku.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wjqvgdie.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pnokvvif.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gxgddxtb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fcareise.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2aewkcpyx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ayjxvkjq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qbifadkj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gzxcydbq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksgyjxpk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qbezomqg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dcykjfwo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ppvmlmir.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xglhuloj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2kvhjopav.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2omuqrgbz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kzhnwsin.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lyngkuse.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2elbxdtvc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jbmhfruy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tetkdyuz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pvseqqeo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cuxfujpv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2enbsalvn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cfhvlcbp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fnzizbow.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pxmudqbn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ztymjuex.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ioslxdji.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wkahaewh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kqlvkpwd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2isksnmyp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2akxgdlsy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2dydaepbx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tilappwk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lutbdcwq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pyvbtpzq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bxhzzhfu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zfaqahgr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2crtnnnms.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vpsfpsdj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zbahmlvd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tfnuhzxr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vlmjmrwj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hppaeffu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cclsgxcn.html


<!-- 参考信息 -->