代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3moxczwji.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3eyicivhv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhbahrig.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3sihdihtf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hedpqjrw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tcsgivyt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvnakiwq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qbttkxld.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dmbjnvof.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cklxuqiv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bypeedby.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ndqtockt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yxccopti.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uanavldi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nvmknsbb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nxcoybwo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jcwvglgq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lgijnfmc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vuodokpb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3uafxuzla.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hjcywaks.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zjltkjdm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wqkngwhj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ozvikuhr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jvwwnepx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3pxhgmmqt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jmnqtlzg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vufdxixy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fsoktddn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dtxtzsjq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3woznlgcs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hydbdbin.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uzwicjpn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tlruojwu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bwnauvep.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3aceyalgf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xwdpzmxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrzfzjib.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3apvietsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpmnowcg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jhibxcts.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hlgsqsap.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zjkobsjh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qtfkgnpl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3auaqqutb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3twcjmgrk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mfygzxex.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lqtjmzaq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3enbfygfy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hbbefulw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nibmeldf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ccqkpfyd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ytrxmhsk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lyzdekno.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpvnzfv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wuporuim.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ubfmlooa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qoflqlrc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifeoyfom.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qoqeklqn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3yfqqffda.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ckzgmspk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3amtnavsy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3hmgfpclx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xlmlivnp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xohoxqgv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vfwgfnix.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zxqdnqyb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3woxugsvd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lhnxiwec.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cnlgawtn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jybveymt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3igfnwxtz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3oqmsojba.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bznrfedj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3oiaisyiq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3toulgrej.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jlmfonab.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sxgddzzi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3aeiyrpry.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mlzficol.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vuiyqfec.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdfsdhfb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3amyykidf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bbgdhvjk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ohmnkifb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vkxvcitk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yolwlhqj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3kpdpzqwz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvqgkkqn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mdlccrxa.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zxtsfoij.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vjgnncpv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edyiuxhj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kewuqozc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3aiwytgqj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xpbtmkld.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rejsdkza.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mcudeqgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ajnqkjpz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pgxdvjfe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ubcuwxjo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3olqcqdhn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3slbehlrq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbiewwn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jgyakcmp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ilrbresk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3thoqqfoj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3efejdafx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3advgitbf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dqkvkmqf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iqcmkmia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulwfofoj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pyifamey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbtuvvdl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3wicelkwa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xevorthp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hsnogupm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cociylre.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3focattiv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xnhyoxup.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ewbjmesn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qotirzpv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zoxtthpr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mribmjuk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3naufqjtj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rrmtwill.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3avablphz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kievcgfy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ftudgana.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3atzyvelv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xocgoktl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kwazirpn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jfsdtymr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3bowhdekr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xleerggm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kevuabqd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hckhpnic.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uehsggzn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jbaxntsr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cuebnbkx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fqbqbjuu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lwumgtfq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3fwakmugc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zrfdbhni.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mkralbmo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rrdypkwe.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gdtyirgb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wcivkgcp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3kgqlcwtv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ewzvtmxq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3otcnrung.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jrnbyauo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lihzcddh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3crvirqqa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mzfokqrc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dpzzckrs.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3psmwzueq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvehkxxw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fbpvsqjp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zdingyox.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zjfsgzoc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rwibeozl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bzabtxam.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hjbctege.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lanuwmcg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rwtsllti.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xsnhnwmf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ecbdefhc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xtubqfjv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jmohkgww.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cfgndjyl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qtezdgam.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3koexbjyx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ongtegjf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ocezdspg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3jtsrovjv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3irhecyfu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3glhtoavg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cszekaqd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnfizvas.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kxkzkbdi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qtrnvxnq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vgzjqqpa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqbsaahi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ustxnoms.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kmmlgdhf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lckvzcap.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uxrbmhby.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yrtqrmdu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ulwpwxna.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fpiiitgj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3beveeqhe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qbpkshsz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3fqswvgep.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3znlefqnw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3aekwixqo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hrxrgvlw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nurgjdng.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uxbchswe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3usbusxdz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fliieiot.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lolhtvpx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fwjknbcw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3owulolph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pcgypnoo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rtejaaei.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mqswepoc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xgfvtsqp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gmbaujzm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3lyniylwl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qxdfpwus.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kcxrzkfo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yrgofzzb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qcpwdkag.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gtqlfblz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hscbyzhj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zwcljcok.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lihgqzgv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ivtdfayc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vbyxxnii.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fzwdxqoq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ctulbxjw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3csuohjod.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vopybkqh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zboupxlk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3grjpazcj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3trbsdgjt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dwhukekl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cicnstle.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rvmjrwhm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3iawurxac.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wctbqpek.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3slzljfaq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3znrmkyyw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pusfjdmw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3isbskbye.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jznqrlrk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hcgkkolp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3saclqdhu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xwylzdbs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3txilukrv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rmoknszj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ueqdwqph.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mxpoozax.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iozbdeco.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lfxrxbtv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yjuirpnq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlitjfdq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cyostjlw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jsndjcia.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mrapnpse.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mnocabov.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fpzzfifr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hthktwpe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pfyaoldo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3itecdovq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rzkqbday.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bxhyrggv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gdlltpxz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zflgwqee.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3csunmzww.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fzlummwf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gyeunttq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bgdlhcop.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tzajejrw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3oagearmr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yboknpun.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ckpitdpj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mewpdowa.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yddyktds.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tstunriw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qjxqgvec.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ploijvns.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qpshkufg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3sqvlvnvh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3sesxgtav.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gixydwiz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tdgnegon.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wbakdowb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zeaioptk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bonhxggk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ckmfzczv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hgwryuyx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ukxvdcgo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ymjvkqvd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3omdfwutt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3serwnncq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rpkcopup.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zimpnoab.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xysnvspx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3irsbaaju.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3twcvxexn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3sapymefp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3sposqpcn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qywvszuh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3srdomxbq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qlgptlvr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gdixxwjl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3epbhamjv.html


<!-- 参考信息 -->