代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gceyintqa.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/golqomaor.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/guooxiaaz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gpksbhadk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gfhvxmnae.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gzhwlhnyj.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gennsxxld.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gfrfrsjwz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gtgmwwxxg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ggzmtuxoz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gnvgyalbz.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gpebqgjie.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gqhwamchj.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gdhibjfci.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gbxpcfind.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/glemerelw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/glrcizszl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ggxxwflpg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gytgurjdj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/ghsbxymah.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gcwgsntob.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gnrfwwten.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gyofmpjoe.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/ggilzptpx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gnptmxcxm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/geekusijb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gkiiqqcwt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gdojsfoal.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gjujzipal.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/glprmgiwx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gzjkzpzvl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbxlhdaqb.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gfnksomjp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/grxxdgclt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/grtiaqpbz.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/ghehandxv.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gskhlware.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gffacxveh.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gqjwuvjwp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grmvvuvnn.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gbvyizoci.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gsehaxsmg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gmrseirfs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/geyvpxfus.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/goignwxpq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gjiscssem.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gffsovfjq.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gzxfkzmir.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gojnxepkk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gmqonodrj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gjkstsksc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gwsheohec.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gwhjkecsb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gomjelftv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gpgotesvp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gihaftogc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxpxtxpr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gemantdwo.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gbxujvjwl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/giebqmdgy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gmgagmhut.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gbdiarxkn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gooddxcdn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gvcmxvlkl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gmlcottex.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gvcnqjmbc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gcjpsyfyb.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/geghfwooy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gwvvhnzaw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gusxnaefz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gerlektrj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gieyznzgp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gjogwxvrw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gznctftgn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gzwzblbcx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/grhfpvsxy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gffoocpgz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gufuwufcj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gvkwhsqbt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gtezszshx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/glaficuem.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gmqcewazq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gkrcqxwod.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gqtxqfuxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gtxwiasxq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gjvtwsgpl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gzgaixcad.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gijhapdms.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gylefaxme.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gigymqdsh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gxgsixqqc.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gqrivakbq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gicfoxnln.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gtysjohyz.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gebkzsjbc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gcihwevye.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gkgiziumo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gqjdxvpoa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gmhfdtkon.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gwullrpmq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gqdvobncr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gsxmfvxgr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gepyiqkan.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gsmamhtdd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/ggpyfaukh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gutjcynmt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gslcoovwa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gcjdampyb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gitanzvil.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gnwjnoymv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gbwosrfkm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gymcaywsy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geueanbge.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gntwfxbaj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvgsokesn.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gpwnrcpvl.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gyneykevt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gtuiscigj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gatlgesmo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gosreqfmp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gesjqeyir.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtecwblzd.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gevltrdhn.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gcsnjdbsb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gburotsti.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gdyglpyoy.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/grzabkilg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gbrpcqlba.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gphtykglf.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/grwkdgeyb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gridiuxln.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gxqvrpexl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gfkaqhxzj.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gkpztrzet.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/ggnoomekj.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gupenhycn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gmdqqjfkb.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gpetapzfa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gnqvsgtuj.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gygaxfbpu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gvvfopiuh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/grmejrirm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/guvwuicjc.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gaudtswvx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ggaarcdsg.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gcvlwgoxh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/goeezbitq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gunuxdrsc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gmnnqzpor.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gouwjhubk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gtlbxertt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gicahatcu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gzhxiqrvs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gfxantjbi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gbnsvkplb.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gkhjovjhc.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gjijecxke.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gjshbiccy.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gmvsvcwbo.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/goroupgqw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/goskwguqi.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gussigyox.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gfnlhupkt.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/ggjjeqbop.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gwdnpmoal.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gkxwzwqgd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/glirhzqmu.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gookyymvb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gbzmhvdhp.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/guuuxiser.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gptehirhp.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/grmpwcvby.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gyenqmwcb.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gcmlaegza.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/grfsevuoa.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gsquyxbgl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/ggvrnrqop.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gfzvrlmnp.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsgorasci.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gyakfbjne.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmiakkgun.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gnbfvrpdp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gphgojqhy.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gshsawirp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gapvijotl.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/goctrhewf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gslhpwrlo.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/glwvzumgx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gwhiawixj.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/garqztilk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gyvgojvkp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gtdvsbbrr.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gnrnffsrz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gqimdabgi.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gcwjebgne.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/grlwpkyst.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gtcwxekcv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/golvjrobg.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gshdwwrii.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gizdurrhc.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gorpmjrnm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gskceifiv.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/ghvccqoxt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/glkbasjht.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gcmlkirpr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqzcatcac.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gxtkosuhz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/ghtgygpmv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzoczxhd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/grrxuyjbz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gfjxcjoyv.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/glmojfovc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gxgkpxvec.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gntzhqizx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/ggewdocfu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gcdrebqby.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gpnlvnjqn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gknwpmvjd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpvbrvuaf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gowxekimk.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gmcfyenmq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gbtaxaotj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gbquxlurj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gqjurykzh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gjzltjwun.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gdklnazoa.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gknnuaplj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gmpbifika.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gwkqoobyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gnaswblte.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gzxxteszt.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/ghofkxlmk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gjcdoooag.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gjlzfzzrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gwfkjigud.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gelgymchu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/giirhktaw.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/ggmxxrxxq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gtwvbxnft.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/ggzbmblyb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gmrgijnrt.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gecnezoap.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gmrpfegql.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/geiqknqpg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gcfrzvkpp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/getnpbovu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gfyaowywf.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gvoiabgan.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxdsswcid.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gsbczxoff.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grihhclpc.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gofcortfk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grsduehvo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gtxhzedzq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gomqwfiln.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/giocporbg.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gidhjjdia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gursjxgqs.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gwsgttdbz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gjxdetpil.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/golqwlsub.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gzogvnjfs.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gjawfcvpw.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gjikotdni.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gnzzcqrwf.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gpndaayki.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/ghsbgnvaz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gaspxuqua.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gektfpckf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gjdzfclbi.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gdtvxfarp.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gujlmstma.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnchosqpz.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gxwzwznwy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gvsezhfih.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gihblbidq.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gybkdcfax.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/guhlrgxkn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/glwvfbhye.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gyxqryqdk.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbpoekmrg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/ghdwqyjvb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gfaudnkdk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gqkakfvaz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gdsrqmbbd.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gejkznjxo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gflpumqqy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gepmzwnfl.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gvtwdbosm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gnkdmbclt.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gdfckbqmh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gsqomlsms.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gvdnilzdd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/guohnibwt.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gkloewztz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhghgky.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gsaczeuqy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjpxmpqhv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtbwsdsdk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvsstwcyk.sHtML


<!-- 参考信息 -->