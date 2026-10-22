代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2scnqipgf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jwwqniwu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fdcxdtha.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zwddxars.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lvqwbbpz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlluvzmm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gbshwpjf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nowecjbf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cewjvsey.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nxbppgom.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zjclligc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tyixpkqe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mxbjqhtl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2digrybqg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gwncvdyv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2svxsiuwf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nvfrcltq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qvhcrroj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2getnharf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dozdarbd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2weymwghp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yryjfcao.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2aacqkabc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yfgbwrdh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qlgyllzt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rxvakrjp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mmrwlite.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mrdncvdu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ygmsqbaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmqxbqog.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2glmhwjqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crobvzxo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bsrtogvq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vjebisaq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2seogdyot.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2druihadp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eahnbyhy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uaaachib.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ulyjzoqw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2amqhwaqk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ywxpedie.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sowknbxu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dvbroayv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2mvmrsljh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vfsmicil.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zuglngpo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fbbnzjtq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rbrchcnn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tvtpwshi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vyoappsb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uhxnpayy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vhfiviat.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zqsmwttc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kjytphjl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2diedhqbw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ttdrkfku.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dmslgdjn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2lukedlhb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2skusdhys.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2dybuoxkw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2knlmxfvj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2njwsouzs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xttgxkeb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2shshgwje.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xhfhvzvm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jngrbarm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2auuutrhg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rlxptqur.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gdzmzwew.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2egwwrdsw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mkkybbjw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kiajddng.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nxkbpjvt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fyxjczhu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xunimkol.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ifbdfwvb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zyzhaxvq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xmbvzwve.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vsuvhhnu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ksscufhc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cyfcpbvm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pybkbrdd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kgmimfkr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbtzbeap.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jzbwlgcx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehsbcnjf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2erbjrmuz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ayffrevc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jujgljbo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gsvxqpiq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wmipwcvx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qswcbxen.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bbtzszme.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mranojfv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rlplnjjh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2anisoisi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzsegtt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tvbcxrpc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tquajrun.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzdrcrkh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2svbggyri.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2safmptqb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rufyjzxf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dkmusble.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dymtqtqj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zhvomylm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vevuberi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rixmyvkq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2juzfoqiq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dmeehtje.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ibimgwkm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2znktejyl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2stsnfjkd.html

);
来源：http://www.52xcode.cn/Article/details/gt2zzkjuqfo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vguzonpy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jbvdjnih.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rfavkdbi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hgoksjxm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ouuxejue.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2oyigrvpm.html

);
来源：http://www.52xcode.cn/Article/details/gt2hfvxhvgq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ctvyrcbt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pkfvcuor.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zeedhhcr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2okehmeqd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gziegilj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mugtqhoz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2urdefuur.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zsqijxem.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bnetbzvh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zpohuwyg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dwprfmzp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uslnqczx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2oobrsbjz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dwzelxxi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ahjuamzh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pkqaxvjh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ttwqfrob.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kmcbipat.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tfkudzsa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2edvxppym.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ysvehyrp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xgadkhqx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ikbmwwrm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nwucuwak.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mxttfxor.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cjtagoqu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qjqfhimp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shuhyanw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xgqkdfqp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekpfbfwk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pwofdhla.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zjszviqu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2aptlhbzs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2arjbpseu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2folmqhdd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bfbbxdhl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lycdrntj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dfaoqpfc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2iuydpfae.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kckabvql.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xvrvpeqs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2doybreyc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gtkwuemz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gmjtvgoy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tvnjbcxy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2idosbmiz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kybxuqma.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rehmunhi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2oebljsvj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxflsnli.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2szklbhlz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jrqspbeh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2drxhxvol.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bhsvqlcp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cqkryroa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oyfbpvwx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jpeoglml.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uhhpgssb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tnhyblpv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mkswawor.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wnkpjenb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qzylmpgk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2iftnyuib.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qbafsxbe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fzlmjtvy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zxwrcqsn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hffmwzpu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ldpsshea.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vjebgknt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uhezutcm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mdlpsdzw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wuxrbnyj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iulirklb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2derenslf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2veflasap.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xsavtkja.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wknjjewf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dbdtycgp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wnhnqadm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2uzfdhwpv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2veyxecvj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bsbbwkgv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2psayolal.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ysyieurs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fnhiamoo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kuodpfvo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aqwzwvgl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2igjbcmeh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2aahfgcau.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mmxzszce.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2biftelvy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gqelauib.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fmzwjcpp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2bkqjkpfc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zanoehog.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gqbefubd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hashivcj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2drlsvotd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2oppaonmr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lafdhtjx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hnssbpul.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rcyfslgq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2adprfxni.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xpkzaonr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2daxfwdts.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vtocggmx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rkqrrrjh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yphaposm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zmfouqgh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rkzynood.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2iukdlhec.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ppgihowp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wuqcirnj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2iusurssv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kpyujfwz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xwzvhmqr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xvxsxcgq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2occbnhhu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vnznjrxx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gijowxza.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ywgmnqlk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mbdrubnz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dmkzcpye.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xszwwuun.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cgbtmjbx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2plydauji.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gckhaprx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wyoztvvm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ersqllyo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2disnfcdo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jgureepx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fdqwoaoo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vshobutk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2iorptash.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2oljhuyay.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uzacjhgx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2yyejcyxa.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2excrroup.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dnozpdcy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ilgvirom.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qulquxch.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zcmwzusn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2hoglhgwx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzfnbzdp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qooxbfvo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xthkrieu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2azkpzznl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sggiysdb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2shakvtvi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rjipjjkj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cwsskrdz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rswanbly.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2trhbugei.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bvwjwosw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ffnosbzd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2foxqowvu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yirprqqb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xinfsxvp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xjrvzpno.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hzcasztu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wkwgjhcu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pscovhuh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hgaypoht.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rcmhfhoc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wdwsoauh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jtvxztqq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cmtmnmhr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bvcwdrjj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmeivzrl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gepwgkin.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kiwgpjjz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pfvuyfsi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wbqkqats.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2huljocer.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icyzqfiv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xzblxyws.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxfmtruy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dqvzsecr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2fjwttzja.html


<!-- 参考信息 -->