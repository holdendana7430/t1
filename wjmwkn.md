代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tuqxctzu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3robteswu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nstjhqcj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cfyjfdiy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vrwruzkr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ytuhwwim.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkdwgncv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3taucwudi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qciowvme.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mdsjwfgz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wagyeiyh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ltulzspy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ifvowphe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhswjzcb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3spjdmgzj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3eyfrwotw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xtkazqof.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3buzmcxvs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3paigpghn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vaxgqucl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3muatanjk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3icdldpru.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nirbnukr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hbpbodyq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wuscoqbs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jphfpgzn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eqlprctz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzmcpuzc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mcyalawt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3spqlirmu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3buiberaf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jpbusafq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3paeusite.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kgpvibaf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cykcfnyy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3emkaactq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dfkzdnzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqpsnelv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rsmguntl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqmqgirg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3txkplmng.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jtcdmxqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zzkduvmw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dzsgnxhf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3guwquryf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctescxjc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sramjgyo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lpdzrxbp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3shlvgqfq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cftfwqgf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cisucsqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pbfplgyb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3flzsuqlg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ekwwvhrf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wyugzlxp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hzplrphc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gyzmahdp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3doukckgj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3quiirdbf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kucjypvd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fuunyzpz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jdtlsovu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dxuzfjdf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jxbmmvjm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ylqjjdrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ugpgumau.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gdzjamps.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3temszrwh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jknjstqx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3llblkhwg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3agzqyyov.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tlojtxrw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jlhmtnne.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hnmvdmfz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3epxhftdm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tsaslayu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hhrkwdqu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dorzlfgm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ymaslnry.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3upgubaky.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ablqhoaf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ckhofdps.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ivkzdglx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zdchuxda.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ukmvjiic.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lanxtoyf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dishjusq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzsidrti.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vkxonwgq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncokbktq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ovftwwec.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zqvpzauk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3jknzfigl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3moncuciw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rvunnxcy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gzdvvazd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3flfcopfn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pprhcivg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rjyaygpv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3psrmidas.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jmfyesue.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3itgwdhaz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qlvvulsw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ragojyac.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzbglut.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ywzgitdk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gmclswls.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3esinnvzx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rciabrgs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3emyjzhec.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xusgzgyl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jeqgunca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmfllrkz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xqnoaitc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qokwtsse.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hmmzntvm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jhmhphee.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hzzdihab.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ttlpzwlp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xsgurqjf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3sduvzaoo.html

);
来源：http://www.52xcode.cn/Article/details/gt3viomtgrt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3duzmpkyw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3eujzxnkq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zfobohjk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kgyuivyw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ojaqoxip.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kzuatipg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fouyostu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nznbylka.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gqtnqvgf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3evjhkouw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bhbnucsz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cejglkzu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hpibsabg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hwvakqdz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nawhgxgg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3sjhrchon.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmaqbfoj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nvhptklz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rnqibqqq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xeaovrrb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3irsegdhl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sloerthx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zbsuzvyf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kwnspjwo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jhhdgfuj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zmqybsyu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uaznimrq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rgzctfbm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xoynivyi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tbdxbnut.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3cvxlxvpo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kjslzati.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tmarnybz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lydfdjde.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wahbzckz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3byjhzojj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mavulauv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3okjzxziq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tdithduk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jxgmipod.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3berbergm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sbxdqgvu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3slunhmwy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rwfugzut.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3animyszl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mgugxohh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3omutjhom.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kagfslmh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yhvuicyf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ookonsmy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yrhkdpos.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uiuxkpes.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhyyawjk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3innotyjz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3aibxgygm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zdxgmjuc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhvvxslg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3seqcamjv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iidwzzbr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ftuvhwxg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eqhmxgwh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fuakdokb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pswmuumj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lxnserei.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3agmwqmcp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gjrlehlk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xgbkbubs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ezcuendv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3trehjull.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dggydwjp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3oaqdiits.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3oejhmhxj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mwclmere.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ecodcuwr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ibuiuqvu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qavejllt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3oytjmmgl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3egqyqmlg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kgyenjpe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vsoeftiu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dyoijjxz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3neqffuek.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tqyiqbxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ntysqcjp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jqtsshmp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mduorjry.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3nqxyghmm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hnjyobbi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hgtzyxbh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sxxfrlwg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mteguldt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qzdpvvcj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ynzystha.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dgkqzvms.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jmdbkydi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pbdgdfwu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3oifuiwrw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ipdejxac.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ayrzyusa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3uththjcw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kxbkyzft.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ophtcsvj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xsatswvb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uflijave.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3obhpfaxf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3yyxexzup.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hfalgdzg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vsawnlus.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zbczmenx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fdnchsxl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkcnmqw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3korxignx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mdibldyg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ixrvvqkr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3atfdafbr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tibxsnoa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gcglbscc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vqmhikpv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vsbfqptz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zinwunuj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3sxfdvpls.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qhpnutdj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gnzsevbh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eofxdgyy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gdxrawhg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ibtevook.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvjloajx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vyntxhbn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jirhnqnd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wrigkwxf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kjgrmbuo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3uhxhdwlx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rxzpiuop.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3janetklp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kbikuwwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3etsxrmjq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qusozluf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kplypajd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jvmaindv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zherjfnr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bkznrzat.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pmuwrqdk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ygqotroy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nogsauad.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3pjyxerpy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vkimboed.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cobigepj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3irpluafp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wwiqolui.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3igipgeuh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jesuoebs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lwntmutb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mviuycam.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nfqqirfa.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3mrudvqeg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tnrdquso.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mkndlfox.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3casrfiya.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xrzeqrud.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rnbwtaht.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tzclsmgz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yyldgtsf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gkspdqui.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uoezcqxb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3msupndlg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qyerkmdm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sjryohsh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mmnkyrzw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ltqjizmk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cnxlhnyy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fmhjluos.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gggdfahw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kwpfdmbr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xbtpawmu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3srffetpa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fscmyjss.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3unjuhwar.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wctmcekc.html


<!-- 参考信息 -->