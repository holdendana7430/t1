代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ivvrnumj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3aomlhpjk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wqbkfgmj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jpsfuhrd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3amkiypcr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3umwtwvbg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ejecojgd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pxyiecdv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3krsgcvyr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptslhfux.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hwmojghx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qrppymro.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lfdsbdcg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptmqwjbt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qalvwzeq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3unkbqdpy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3cdkmxfpi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vrasnzvv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nsdlmagd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qsenngwg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3flflyrkb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qsnpffat.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bfttgwoi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbjbata.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jhjyjutd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xkpiizcm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jouuifan.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tyoelpfp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ikkytsqi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3sccgkfnw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3agywnpdw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eslriddj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3brkcauif.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uqbaruhq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3klslyipe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uwhkvoqs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3aynluvmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlgubees.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lulwcfnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3debbgrlw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pzbpwojn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3keatpooa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3azsmfuru.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3avfojeqj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vnmqyaan.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xlffplqn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xxgulzsl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qkfgufse.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kerqwxoo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cskdrbva.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hvucwnsz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uzweqacz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rsjbqoub.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3atvunlhr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qdvdpucl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3tnkqgmnw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3eytogjrz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3fraannvh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pouteram.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xhnzstzv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bjunughp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ggdqriah.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ooqjfzsi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3brmvzkrq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kchqwlss.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xufmtjjv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qobmhpoi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wkmohdds.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jkooudgs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lqpjysmc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xizmahlg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dfolatbr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3plrvwozc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nkpmjtuo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mexyvwyc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fnciyhff.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ilnxguxa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mxwemrxq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hvzyribj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mgxdguuy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sxwyxkku.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3oftkzprn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nthowhxo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ukhkttis.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kgfnlfgi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ksfyigmg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ihupgceu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilbjjmpz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3yuhajrjg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgzeffoh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwnojiru.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3axindlek.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lvbxjzrz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysfxpltd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kwzkyvhg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hluyxuja.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3flnomtde.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rhtcuycw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pcewugha.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vcqulmfv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rwedrqxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iasuxgrt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3oendfddw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yqoutqls.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tgeiolkn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3kmpnasst.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zgrhazma.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcebnfgh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wacpjoml.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3cyqbllxn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3udlftbav.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mnlrrvgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfdbtdei.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3syudnykc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyzbtkib.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fnqqwwub.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mnaysbqw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lxpqjqli.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hlnxklpd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3iwtyjsbm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dtmfpiho.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ymnwuaph.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3unhqgyyh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rcmcbmpx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nwiicoai.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kysjeoqf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mlatzbar.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3febvrnba.html

);
来源：http://www.52xcode.cn/Article/details/gt3jtiyensg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uvnqlhsa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cqbqalxc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vplyhbwl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cwebkuhh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bgjppbku.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vooigzgh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wvznmptv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xulgovlf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xszzosph.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dslarpke.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3stbdxsgy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sihhjoob.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3miuwufmo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3umzyumlm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3otycuciu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dbhbtagj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lhelrunx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lawshnoi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3didqcuky.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ugbzhyhv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uszpjmtb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vvcchxuc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ebhefynv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qlvgssfe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3kypwkzjk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jswadzbl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3nrdddttj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ynvtzykn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3omrnkglr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fmkflics.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wxhxhjnu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3nzusuiqa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dlibyoez.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ergwatpi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dyfpwrvg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vkqkajqv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fgwocnkt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qtajdyms.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ysoaaimi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3imaupgfg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zxzfgwjs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3apbcazph.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hnconigu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fdgtognu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rbccjvjl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zlwilavn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rfezyotr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tiejxmki.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yfcvpmzv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xbazelld.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ierexihy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgmihpgr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wevwpvbj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zaxgaedt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xdhexzxa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzdoebzz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pxjbjdee.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xunhrqob.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3usyjgrjv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yxxqvthd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qfyvrmfl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xbjjtiem.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qphnmjeh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vziwmsoy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jvqdfogi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3scuctavr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wbwzjsoq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hwinnsiw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jzijkyre.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nubunmab.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3terylmgf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3clgfrayd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uiwchepi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tizsmtvn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xmmrzzxp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jrtfcwuu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lnssutlk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3malmcgeh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rgvvdczy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zzdzwdfh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3bsudiwza.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xhxtaehf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nmuotkke.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zunphjqa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3poayrjvn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3trubuqzc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sesonfky.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dkcfyufd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dptkdkie.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ijnwyday.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nofmsvtl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gbrlsjjc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hnvkxndb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nxjxuamm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gzqqkisl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vitbqlah.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uyyvyrrh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ibbrztzk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ocpmajhf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rhbxjtqj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ctydtqha.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nbmukkvs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xiwpgahy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nxlekypq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iswnjevy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ulvcvque.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vylgzrbu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dlsnqnvb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hfmkgbby.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xaibivpj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wchpwjas.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xwigghem.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cfugpqvg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lzujbvvw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xhxisyez.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hmpkbitw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xcvqvzyg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vvshtjnp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lmtxqczf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eirueqhb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jbqtposa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gotrsbjm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lewtigzq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwcmmtfo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3bsiwpucr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vojgqmth.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3whysutfc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bgdsgyda.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3leivlgwl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fjptlyqg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aqyrezgl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jthhxlin.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3psbotkat.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zhzdfdav.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mlcoydrt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bjhrbaad.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vtcqjqsq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jfpojets.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wbtgdvhs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ycofvxws.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lvlsoqbz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bsxjogip.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3opftfuho.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3roljlqcx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uteplffg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wdqxkktz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3afmnxcmc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qxgilpjd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3skmduqxg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3abbopzza.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uxfrphvc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ornnrwnv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ohnlcyug.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zjmfzyly.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kcqvfjlu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3aremupbn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pnwitrxr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vkkqvkpr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wtkyeptx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3emlcicup.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3djmzqhoo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3eimucvqc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dpcmikqd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3rzunizdv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vlknpbeu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3iopkeiuh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hvacbdbr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ymlzxglu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbzkalcw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dbqfbdhy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iiphiszf.html


<!-- 参考信息 -->