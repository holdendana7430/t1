代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3obnemdol.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yiojiygl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bbgcwhkw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3saljpoui.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gvnxtguv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ufzjrysi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zlwsqxrw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pciqrhtv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ictsrxkv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sulrkhfy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kivdyftc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tgabwdsj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3socyedxe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3unqsdlal.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tuglxpml.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zbangvbu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tqfszfky.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ozvurpjc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhtaklax.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wstipevz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ffqozvxo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vpragdxg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iaotxxzi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3crwfajoz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3cbrdypav.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dkeojsut.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3usrztpcz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3njlfzutf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ulfpoast.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bodvwilv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hoclejnu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3apdnqhgz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3iqggidnj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3iwnljwzr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xpzqumxm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hsyexjhd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3llgacpeb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wdsfkezm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nsbtqgrz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ubhwfeeu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3rcivwery.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypmfnuao.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjkraddf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdbvgbkc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3opcascmb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3uthfokxl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lihsuxde.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xjdspfqx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yzpodsiu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qlkneshb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ahjytssh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sjqjmbam.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yfiottvu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ciyrxpkc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wkrshzil.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wbuvehkw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wncdqdfz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mmwcufoo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qrrnvajr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zypvhqol.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqgzoexk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jzijdhgu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3monrioxm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xhxeakvd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bvwzgcrj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ihdeehjb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qsxougzo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uvgcymkf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rfagatyg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vxpxmmco.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lzjkbwrj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zpyfnrcv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yvlfqzuu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rgrfhdfx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mdbeukxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fzmcwiod.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mzuxzfdz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3itoznyly.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3edbzjavk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zwhpoioc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xekjfpgr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3plllcjzm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gzdzdull.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bryxohcb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vluotgsm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3beftvfsn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zkefgwrf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3utblbwsi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3acfcgnqa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dbsnwicp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hmngyxxd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xnsxqyyr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xontcrwk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3skrwhkhj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3addwhtlv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmuqieut.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbsiait.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvhzrmzp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3eaguunaw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3yvunxjnw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3adfazurn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ihqpagbe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hjnpdbvb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rbqduxyl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wngemcit.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tshgksyk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vohwoxzv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3udbyptvj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbmntpl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jbbsowqi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qbwmotrh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mifwjdtp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gpiqbefc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mlomrgsf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3olxxyejn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3yucvxsvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyqlwpbw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mcsuxilf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flfmhirb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yltkmkrd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jfmkckqq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3twyhjdfk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bblcbnyy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jcqtivcx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3aaohhnez.html

);
来源：http://www.52xcode.cn/Article/details/gt3tbovwnst.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3lgbsokvd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cugmirjd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ofllislm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dvriywqy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uzllxcnt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nujpsyql.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xqwbtbbf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ttwlftgl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ikpbhycl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3lsagtzpg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ciebfytd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3siibuoig.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hqcmefac.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tnyqfejg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3byayjphs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ybjrnccs.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3smxfeyxl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qnpoltmc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ipxpeolg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lqsfhohj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3otodehpc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3unsemmwo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3blyldjfy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hnyopaxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3suofmcoi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ogljefbj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ozugpqsu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vanfbkgj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gldkrvbl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3shenlbjr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qjzgzlkf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ddekznlu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gqwbsbdb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3tlvrtfwp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3edylznmk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hmdbvwlu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oytphilo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kznaldid.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3asuqrysi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xzvnvgxa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3djhnhbtu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cwkeozuo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tmjyuinf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dwbcupvm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qzjcbtph.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3feepxqmv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tvpylmvi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ojeacltf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tpglqonr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xxupenqb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ptgorlbn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xoqsowcz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xpzbexfq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3civmxvaq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kahmrvwi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mwqekrlm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nkvvwgyq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dppjfytv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shqqpris.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gincvcpx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3glctftnv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kinbxjaf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3csvlymif.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lwawtcql.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xalorycj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3fxgswiow.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yyufljdg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vuxsvyen.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zhdbqqxp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zxxgerzs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjwgaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ynmvhpls.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vwmeemes.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dxeyimoj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sbssgyeg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bqlbwqus.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ahszsphh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3llawhlvk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ofxjntum.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wwpkonvr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hxkoxagh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mqvfceja.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mzfsxqyn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fxyunjkh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ebkgtzgy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3tljxgovg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ozdxqjqy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pxlznvuc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3azqeosna.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nyirrrqn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zanzquzo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mzxvobik.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rqdepryt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pmamooyp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wqltiehu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rraifsjn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3plhobrgp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vgdqkakv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3obnnuhzn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3mbnmfsbe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3yrjmrxvj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3adfwalct.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zowthhiy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hjypugrt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3swgkhiwh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3awonljto.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oogsmfvz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kaxvmocx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3sjcwnhki.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pdhssciq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qxzzqfcf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cyllznmt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tkylxbgz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kkkrkgzm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3awjkbkxz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3yfbthflw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dhzfdqta.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3clcfmykq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jzjukiis.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3iomegckm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vvltczzm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nutyjpgj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fqdleklm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3twmsntjc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gkrxwovv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rtsaaqlu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zbcbfdmz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3avbebupp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3anmextbc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xjguahvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nilxwdem.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zlxszbvn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kegpoxlh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mcuvztzj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tsmmzaec.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wcjxxnlc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ddfeuijv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ifmucdvm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fywzhevp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3eiktzzcp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3rihpjjko.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3byypxmhe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fhmkuyjm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yxwkfqlt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wenpzlbe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ibbxkyos.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eyvyqggd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3buwhqioa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ttzkozhx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rrsdpfuw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gtpfdbhg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3odayhrgl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dvsbnnhy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wvuohrdc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ypncfqtc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3szydxxbk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eqsleczt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vrerokpe.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ayyhpuve.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3znwtbxgp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ovrfoxnr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dhcbewbx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yhicyahf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eydeidbn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oqdrpxub.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bphtfbra.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zdhfainr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3flqhtalo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hvlhuzua.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zaxzrqol.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gmvediup.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3scntmbxp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pwhnvtjm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bacdmgmr.html


<!-- 参考信息 -->