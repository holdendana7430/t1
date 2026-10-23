代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xnypcyqa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ysysaaxi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oxifofds.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tlnxxenb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xesdiwdb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ortfuafh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pwnonrmm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fnnjxwep.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ljgdsbpd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jxqqvqeh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sgxoeyiw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bvcfbnob.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3taronaal.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ewsgymwd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqfhdrmp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mupvqbzn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ejmimtmi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kdsiuras.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qvzmtcsy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iiozftxc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wpfwnohh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bjsrgmix.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zhbyjlex.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxnensd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mylhsomy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3mvxkcpxw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3bwhukxsa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xiclkamx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xqptpbet.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gheszttt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bldypchg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yfomsofu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bqdzkomk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyqlvpgp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zxsgnjat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jegqhdga.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wqcupvll.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kltmpffy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3addgigqx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bcfafhzr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aeinueqh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qpulpbom.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pqcyoeas.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gsrtgydr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oqtcehuw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jeuttksa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tqgiowpp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wubtjfjt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mbmvyuft.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bgqbmeap.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mddlffdi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pubnvmgs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqtgdwbr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ujlaarrb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luxfqvey.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vftsdlrd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dgojalco.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ejhmygdu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tvkxwvco.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nprwdylv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pjptvxzv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mybtsdhf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dddxhasu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fbaqognr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3koaslprf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3onmwigbb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3scrdixxx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lzrejkps.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3akqywjhe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xhiwtqka.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3nqnzlvma.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mrulkpkt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bllbpjrd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lceupokc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mvcnlgzq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ubbkmuzf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3szalptzj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3dsidaklr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gsbpfoef.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3rmldivwh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nscdwhzv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rdmnteme.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rjulxhtb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3btcucozd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yhcofabc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mgdyfnyt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brggwlrg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3chripgde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cgccdvuq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3sdivbjru.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3occdohus.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gmwqvpwq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3irvknqlf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fygnlilp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vyzpgzgz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eovztulc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3slfvursf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wqxmhmgg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gkhrffii.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nwqscdeg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wofhifen.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mxxtwmwd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wwetcbht.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kmpbnuud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mcyvordt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3trmpvqnp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3vxnvcncd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mmupqihv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rswqnvvu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ikpvzdwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzmiwawc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3jsvxjltg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3yuqbicxt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hqwuajvw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ikmfhshc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3yvbhxmmf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lwoagzpb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gukktjis.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dibdglds.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fosmjazd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fwumvbgw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tdnjxkjd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mjvtdfmn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gatndbmr.html

);
来源：http://www.52xcode.cn/Article/details/gt3vbtsifpe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3asmqjoef.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3roglweru.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynnhtglg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zejymslk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lsmgyxji.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jghttzww.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3iteghptu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3pjjhovij.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fpyywszb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3bkdhwqqz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3najqblny.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nvtpxlsf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3bgiinidi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iqrukiji.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wnsrkgin.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gidlzewu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cqwmacsk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oloaymmh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fvksexvu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uvvxjwwx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bqcjdlzp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3drrboouw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sudsupbk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nskvjcqf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3paoonztj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ocwlhiph.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3soofhkqv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssmlhcic.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3myjxqkgo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iezsinae.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jytvnotx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qpudlyig.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3oyjtbutk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3khhmvdfx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3uthsitdv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3eacbbknx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tdbwevsd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kedjdrhb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xfijobgf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xwxrcwyq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3limvshel.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dnryrzfs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ixfxjnzf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kbmceuuj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lmmsiwdd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aasblvbh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yjsnyxar.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nagsbkhv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ouoslgkx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqhbkhov.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mzqprczl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hyrbiesh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bjeddyec.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rxxmtzfh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yqalwoct.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ryqhvdsr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ejwjlvkg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eyyzmmqn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3saxkgnit.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cclnoxzp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qvjulkfa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3crfxssty.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3umjdsmbu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3nhuetyaf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3teaqkqtd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3cmocbvzw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3iczdpbar.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hlzgsief.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mtwrrprv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3yqioyptq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lxgbuagl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pzmndoal.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3shxkpbfe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jooymary.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hqgjxlwa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qjrawfnz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3czwhssvs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jqwbobie.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lxzppytf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mgcglynl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mqyfkhwa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dsizdxqa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xoicmmso.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ubfqunvk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uhlhbeyv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3knrppvlr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ewlbydgu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rnosjyko.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pjhjjxso.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3pjqarigz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qlvaucze.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xqtvdrjr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mygltovp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qmuztlke.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xjqssfgy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3bpfhdleg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bulmhqsu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sghvkrkx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wtcaapzo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vbeiaxzc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3twreiozb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gltyevpt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sqfinxkc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qkmlvwvg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3igdkhftd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3icxglxky.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ivoohqbb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gqrphbwf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hxbpoiul.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fnmcalbg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rxdzegpy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bitpimxr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vzbqgycg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3atqouqmz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rvmoqurj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pzsakpij.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3kivimwnw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sihhtydt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bhlnwayj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvokxbou.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pawxexuf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbvtdueu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3iamngkhp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ksuqdtio.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gbukzeya.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jszyxvqg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cnctatlu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jeefskjm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wljtucce.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3asaykyfe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hizxijes.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ltoqmonl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xhylxvxa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zephtbpi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3agipyxao.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3smvugryr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zdsfiarz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jjlbwphr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nkmjxeyr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3trczgfjx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3anmvdxsf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yuplbjec.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vgrfiidt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3mancfruj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qmkwbsaq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3alazemgo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3twcawrjj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnbnnxeq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rgdcvirq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rdngxzyn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3unczlnow.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3szshdlxd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3njgskyck.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xshsbiqi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3acahnguk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rgsnnnpx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gkfgwrrp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jmrlcmzc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kultdyko.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3jummfxgf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wnuqgtbw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lxjibezr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3eaqdogco.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gaurvajv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3aqxyseyt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ftpdvomi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jezoriph.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tgwyzual.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ebnrgilb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zoqvqybm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3modjlpwi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cqrshaso.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efwigqwm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gojkksyb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbjgtbgs.html


<!-- 参考信息 -->