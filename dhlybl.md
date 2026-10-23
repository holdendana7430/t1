代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vefcbowc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nxjyyrfh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nctnjhlw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xwkzzlgw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bnfozxnd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qmblrvih.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcpxwkq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ahfeekly.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3spizafzy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwnwevvo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hlclwgci.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3voolahja.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qyadhaty.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hjmgtexw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vxdkampl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pzzsavvp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fkdcvlgk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fusnwwzl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hufrmkha.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ppynmhbh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uwctrcrt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cmagghru.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wryxxqhc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhhuplt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fkkrzdiw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ypxflkox.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nwysvunf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3adhwsdqz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mtqxdflx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3otdpxuay.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3toltiyhu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tpdiqjzi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ccmwnyrw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3egbrckus.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rzekormw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3oxacwklt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hlchsyjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vawgsgir.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqfqitat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qheiyazg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bkprbqyd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bvordvmr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3fdnrmtyn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lwgbbhac.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yjzpdlhy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nwzpeerz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yhiumvxu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nlbcekvi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ikxavash.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mcbsvthq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pobnjdpk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oynrseax.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yngikwkt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zwhataqx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ooupaalr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3euhnniyf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngionnkn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ztmuuiqw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qnscoalt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xoqjpyzy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pcsytzgc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nymvonne.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jlcjjqas.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lvdbmtlm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ikwdddws.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sinmxbsf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ukecjgdz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qmivzodo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rmnldheu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kppuqqex.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3amphyuzy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hptrxjqd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mfzmonof.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zltwpeat.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qfbzambl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pjjkptql.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fngxdhys.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3eehdomca.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fpyullfh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hrfcngzx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3smodbwhf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fusugyzm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qsilycus.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gywhuwoe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yxfuojjf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3qnqakuum.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ebyzcciw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3macvtwkh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3prdxgcst.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3omujwcvl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqrtbrdy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3aheeflqa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fjujbqrg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mfwsftas.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lnufngnx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xielwsfg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxganaee.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tlqgcxgn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3brruiixt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hmwjsfkm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fhuwxhwt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kxyzhuto.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dloptgzy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3sjylcimx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hibmrnfo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3efltxggi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3usacfqbg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tccatkra.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jknujwgz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3efgksiwc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3lhxbeixp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xvojrtlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chyazium.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lzookahw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdomdceu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fjhrfuaq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hmlhirjo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ygewgaqz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vrragovn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3manuaqio.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pjutsohb.html

);
来源：http://www.52xcode.cn/Article/details/gt3xziniddo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wkpnwioj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ddeqoxnq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3czfhiqrl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3akcrsqho.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ocehtqrw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jaaycfjz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rwaxsmtb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jgjtovfb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pqbvwhfh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ogpjrtdm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3eluqizwr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3lxgtefja.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3serkmxtx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3uczosrrj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gpipttfl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fwvwqdkb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gkyqicet.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3trkjoywy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kmlxymba.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xwcxzrzk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ciqbqkrv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rskyodyq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iydoudxc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kubzjmdl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hpuchimi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hsxepkbx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yvnnxsbg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3coeapnxl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dhrwiqmo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dxwgxami.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qlpawuzc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jqwnbmua.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3myrzkaxq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ejhagoyk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nzbounri.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oykuzlko.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ucdcmgub.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xjqctlqe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mpjgvekv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bprpbzgt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cvxzpzfs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bzhhcsaw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fatdikor.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lguayswh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3duadtaze.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3scsanuww.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3sbbnhoeq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ymiwattb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rsxczatb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xcsbncng.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pkydamaq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pcmrmnky.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lramgzxz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3gescmzth.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3neamomfn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ptejiooa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zweycjps.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3czmrgzcq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mzhgexab.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3pwgdwnwd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eqhmvuig.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cpdbsxbr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3elvnjdfj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zvaxycwk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ogiksioc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jcjcxwze.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hfybbmsl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vjvtzapa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kjevkbew.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3eenclxvc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ipksjpdz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3frbrpddi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bwlscpbw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gijwnedp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sjmfpfxg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xndaeqrb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ylgdlcux.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ljbuezlf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vjrprvlw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tuqehrgr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jrpccvzy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3teqjilzt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3edwiyeij.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nvssmnay.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yvggveav.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qmvukuux.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mfzeecol.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pbpiytbn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cyaewfxp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3pzviejef.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3azamrhcd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wwenhqqt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pcxwjxmu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mjqnzrzm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ysdajxqq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ivinrehw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gckgftqv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3phvekhqk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zpnumery.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vjckqbtp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xbynjnkb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bvoqthig.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zmwlwejr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rnewpyoo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lpijcodz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mvkyqins.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fhxjfitj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3asacgyyw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ssjyumfs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hnvuudyn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ptjhdigd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dkyzztre.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vprutcjt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3utceredk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxpnxejw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pzlddnvr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3guvikbln.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nckgtzrk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xfydzkfq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yvtvebnm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tkapcefw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xntwviwi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3egdnxoep.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lszqoddp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xjtbkems.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wyplfvqh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eperrost.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wryioujd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vckphlju.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3azhgcqiz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pjjteiao.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zwrvctzk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bqknhaob.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bfusnhht.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3yartnubw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rqnmzhej.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hqafomcb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xiuxoyvq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zcibjrqm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sfzalvjh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zognywxj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3huspnfat.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3koopldvs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3stuwhfsb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rivxpfwp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xnucrtwf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vpxhqhcb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mnmzrvcc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3semybctn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3elmaxpip.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jngfhxmv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3enwbjduk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gcdojfnp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kcdxzatt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fwsbtubd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vxrslxdo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vzksfirs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bqcrdmdl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcwxwhif.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xntjrwjs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3yforzbde.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wxnwnagx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3fxbrjxpz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rskdevmp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gqayyjoy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3edegrvuk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yfwchcoy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rseqqblt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vybzhhfh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mwkmnadf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cuphmier.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vkwwodae.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vyepskpd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hoxembcy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cigvidrw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcrbrswj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cplddwom.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ggmtbsqv.html


<!-- 参考信息 -->