代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gfzcsanc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mtndpula.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tgbbyzth.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dhazqvqb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jeebbubj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tyuvpngp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2abobwpdy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ztlejsfj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cntumqak.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yahzoczb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sahizkxi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2lbadolnm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yywscnly.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lrsaklur.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2yedrezda.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2idfdkenm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wxofibtj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tiupnxzh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bmasjjls.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mjsekcue.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uqtzednv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2fdlxgkri.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vpusrkxu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hmuikaao.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2monuadxq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tdsdmwqe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qytgdzmx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ctfdoqvl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2scjfdxwh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wwabuwey.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2lotcywst.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mmbmxgtr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zqgbslrv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mnwjsjbp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uxbegohd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ejfzuvsa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2klbcronl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkybwgfo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibzgkttl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdmvyrtx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pnutpxrg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mawtzczp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xsefjrcp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xrgocfbt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cpldxpus.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pkcelohv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2iyzgknhe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kmeyjyzm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2igvtgkmn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ctkuwydg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2uovwafoz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2csnuzwhu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2daabyniy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xstzjnby.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ofdkxnnp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ebsmwzgr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kfnvsxsn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fevpqkgx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gkrtearg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ctuvvtzi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pbgthvfl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tcmrdzfa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yopjkbos.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ugedgbgr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vyxtgkny.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hqnzmbwa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wvmqgyjv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rmpyntmj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2hicifchh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2izlhlirx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wcclrkmo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dtgcwbhi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pxthyamd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xszvtgat.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2enznvfze.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qkuvfwad.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dlqsnslc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2olzveqcf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sczhymum.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xwdybdga.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eleejzqs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xjxzofmq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ygcvtgzi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2opmgohqr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nmayeqtj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uawbhnzw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hnclmdzr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rloczmvg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ckyjlmwr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xxnlkflo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2busauggv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gcjoqokg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qpruzfes.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vebgeumr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pogyvigy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2eqggwgdk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2izoxpacm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2octltqdz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xgygwkbl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zaxetwyw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2raywqbno.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qlgzhmae.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qhcfqkxh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gnqjlpqp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ouxneiwo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2igojwccg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2awxnokus.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdlmzgrw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wjdskpxu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2abffyaow.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yzaptyhn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ggmzhepo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsffcotn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2brdcftjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iskrmwzh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vnwqkgjv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ugdrbpde.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hpnylscs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jzbltjkh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qceqbmzi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ocpslphh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wlvilysy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fsbtwkvn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jjnhbwyr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cgoaqbrw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wcvldtqv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ldehdmfd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dlrpdhxo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ximroopo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mpbbnbbk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qzfnftss.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2afryplwg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2trcncpiz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2syugqlek.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2bwbranpo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dqjsvbum.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tdwwhjtb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vqeofmlc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qcjlecfk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2iqrjktzh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jlglmkig.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hixnoiew.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2epzqrxlr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rmxoqldq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kttcgvgr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wgvbfkmh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mhitplmn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ivlvriee.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jiytqpfr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mrvjsywu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2sravjkwi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2onhwayac.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ptthbone.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kkqtmpqs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2pxetgsys.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2andmnbvj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2viklqtiy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bmsbcldo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyjgzczy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zjodwgjj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cwhkomol.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jqekdfdy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lhicrhmw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ytwxqbbb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fjoibbul.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2imkconvb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wfklrbti.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nnzlmeyo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2npjekwwg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2flwribrg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ropccjae.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2reksucid.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wgbskdya.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2tqnqkhjr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmecxgdj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2axetaynn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lxvatdxc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xdkdidap.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byqfgmdm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2oignnfmh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rldjrmcw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hptixbjw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pgfkynvt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2edodkyyn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oailcmsa.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2pvpfbmkh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mzhkynht.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vfogudtr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vxwcgoma.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2govfmtgu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zwyhbcss.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2pskwmilq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xxdzfzft.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kaswuyqb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jcrkydsy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gowforyd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nfzakbxv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2espsgydp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qukcfwbg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pbtkpzli.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kvdgsqci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ffclzbsm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zacasqaz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rnduvulg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2nspyavse.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bxlmbckl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nzkugvel.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2sykikedd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2timuzcyn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hcwbqffl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hkzgnnii.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dphiwkuf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2msnyoiff.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mazcqzpf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ffeejthr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ohuvsmwa.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ozmlqjxq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dypxrcoi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lpdnuvwb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zcztouaj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yfplkkvs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kdmtbbtd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2itdkxjwg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dffrgttr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jlcftqbb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mimcegla.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2sothnxzs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zapzjfuc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2shctgehx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xgybfzzt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hqxtugty.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hrjtgbjs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ccumucnq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2arcwqiew.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gfkncppd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vtwapdpf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tnexajku.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nzeilzny.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2slydyxwl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tnqvoksx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nkifflyk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mwzwnnni.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vjucnbjt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wvglzqpf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2amcfpswb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2harlbwgp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2esbbgxke.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2sgfezzdh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmbgqulv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ncsaramd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sitkqsnn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ctymvanw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qcttpyxl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nqtwmepl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2nwxagcjr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2smidcfos.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kcysncdt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qjviicdv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jpeojbqg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vlmbgiid.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mmvmpahz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mixjqdsp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ndfjfoyn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ywsrsrhb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ppdbirkl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fgdoviof.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2chpfwwor.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ecqatpwj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zwlcixid.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lyjjexcc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2anrziasm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fbzngjmj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2optvxupg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vgfkjbvq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2sszyzoen.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mkzzbuae.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fczkvsdv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mjwlzvki.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jdvngvml.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lnqvilod.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzwjltyv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2zzcjbykp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xdjhnpsx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dxwuobhf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2taztdbdd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zcrbjukn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2neoovbup.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2iohplhla.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ixgrmfps.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ypwhrnka.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2loadkmpm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2dklbukxv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ietjmvvt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ebfuvctx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kyjsrncl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oavhtqym.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2uenkjjbb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opkwhtjc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ctlvwgqq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yrucqglx.html


<!-- 参考信息 -->