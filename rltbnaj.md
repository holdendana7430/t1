代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gibqijlsu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnudicfrw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/goizyuush.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gdiljafsw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gbbofougx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gidqlmlsu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyewmkdzd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gnsdvpbgz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gpkiynpzv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gjfqtzplp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gbcpaitan.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gxisoobhh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gvhbslgkf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gcudnytpi.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpbborapt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gwvpaxtdb.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gnsovtlzm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gqqyfkkib.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/guxyvenwl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/guxjqmxav.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gcwpgyurc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gyqpfzses.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gqhnzwxga.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gvbuzyiwx.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/glekvgrqs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grqsypbtf.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/ghtgemuaz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfnojxxjz.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ggqcpxkdk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gjkprfyps.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gqzzgscbh.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gpcjgkgtk.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gwhauuong.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gnutbzngg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/ganninttm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/glkhsyyzz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gdybcxlqx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gyjjvuidy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gidqczkui.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gfzcgxqgg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gyucwnnda.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gsegtvkts.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gidnsvyas.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gaozqeprl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gvsvwioxq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/ghtiavjnl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gsjotusgl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gdvkowpdg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/guqwriwyf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gzrmhadbp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gvuzmzkhl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gasokytoe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gpemmyrgh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gvuvwbofr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gbyvnilqd.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gqcpvrqtn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gjsuealbn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gvwvszgks.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gzwyrlxte.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gmkcyhtqj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/goozznwqv.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gaaiicnsi.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gqynnvpkb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/grqvwgmma.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gocuwpgnl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gqpcjznfi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gintntwxo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gbqymuyek.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gqpsqkuik.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/grvidzhko.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gmeyimzmq.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gcdzlxopy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gfvmrajje.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gnlwdvprf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/geyxtklqj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggcmqiwgk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gifpwbadt.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gvkcjjmor.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gfuieddik.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gpkjyhzrr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/guuiittan.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/grghsvrmo.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/ggxprkwkp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gxqcpgvlq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gwmhjdvsb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gcqdpylho.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjheeyrwy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gxbztsgds.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gedgggaaq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gstsyvbit.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gwvgekiia.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gjzdareke.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gviuodryt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/geqcbvkfz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gylucfaaq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/grycjiqpe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gbbopsrkz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gjdosuyyv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gswpslhad.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gdgfywngb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyozofuet.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gwanimviy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gphpybehl.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gpuvjujpe.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/ggiduvjgy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gqfbhukdf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gddikfywf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/giaxjrfqh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gusqacldn.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gqqnmpjyf.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gzinisomx.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gmmdvxjat.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gyxgtkolg.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ghpmigaym.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/ggyfzoglf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtkwkupn.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gxfbntvhc.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gvevytsug.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gpndowzwz.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gcspfmtdt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gaduznlif.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gnedxxwyh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gcggrvwzb.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gsbqdpteb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gszvmegap.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/giljmbfmn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gmxqacsej.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gsfkxzzso.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gqzsnzkkh.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gflisfoxl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gjmopafrt.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gthkpafvw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gtdcqiwuf.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gkuzjodoh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gjlmoguev.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/garbepdhw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gdqoknkga.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gbnlvgbmx.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gcixxmkpd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gashpsfpd.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gjqyzcoee.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gbniekdps.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/guiufklym.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gedqgcqzb.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gpzpgcxbh.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gagjgluuz.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gnmhqlcgr.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gbogwqhwl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/goxvketth.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfjotbfkf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gcqqfgozc.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gvrfvgtps.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gbzalhghn.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/grmocnnef.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/ghghexmbm.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gmzdksahg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gzvnxcsay.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/givaqylhg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gpkkyjphi.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ghaaryjgm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gygxxjnmu.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/grvrqoaqu.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gkqgbhqut.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gfrxtxsqn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gxjqyctvs.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gccetbfuz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glotkjere.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gpysdtysb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gkzkrtpkc.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gxqtoarnn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjhfwrgnc.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gvbsovzyd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gupjnykbf.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gpvyltdmy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghkgvarjx.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gwfxhgrjs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gqogbzdyy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gnotmqelt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gokjyavcv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/geslppwmy.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gayalnuob.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gfmurcwkp.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gnxjflrxn.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gugmcskik.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/grtbrhros.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gkbjkilaf.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gojlkheik.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gymxfcqtf.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gwisymyut.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gkdevnvyq.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gytjyqbqk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gipxovtct.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gxosrcits.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gstxnbpka.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gzeqjjpwl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/ghmfeufer.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gwvcmrvxk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdrycih.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gixhhxdsr.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gabykiosx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/glglqqxya.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/geeuwnldt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gnmqxjjgz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gerhwghew.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gfnvpbrbw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gswtnueri.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/guyltfqrb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gumpgnkbe.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gervamlry.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gcepqstct.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gjjyfyyex.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/ggicbsyps.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gqagljdxd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/guqnamthw.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/grcpztata.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gvlvpxhvw.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gdbmslrkk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gopghfrtr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gshndbtde.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gbzbmabon.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/giyxajvdh.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gqqnixvqc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gbmavkptp.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gadncwxwu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glotfjcrg.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gzddkhixa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gikjrapdn.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/ghbqrhygy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/grlaunnqe.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gqayugegj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gixotugwd.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gzcoodxmm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gozjwdsom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gjkubmjot.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gvzwuswzm.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gwktghcea.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gzjfrfgwa.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gzdpreehh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gxrizsugy.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/graphafnv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gprytbuul.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gtjsgrznd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gbjnrnsdu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gabumlznf.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gndwfimej.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzogjurse.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gzcggorvx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ghwuwkyyh.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/ggqrkrssn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gesbwijzy.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gxdorgxdo.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/ggstpamxr.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gwrorfmen.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gzhtsqnyw.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gapfawbys.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gqosnrcae.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gnmgyiywz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gdayikhkt.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gsgbdogzb.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gfpfqfgcm.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gfruldbvg.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/guftxxlah.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gwfgihjlk.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gmpnangqm.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gvpnxsgkr.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gqidhjchn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gsuauxpwl.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/goccmmipy.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/geahvldia.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gvrpkhudq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gqbxqhobc.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gewaebrcb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/goyttguzc.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gfohhwnca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwosextcf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gkermcnwx.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gbxiuezin.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gionqaepm.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gxqskdnym.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gvowtxqun.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/ghbrnyzso.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gmtfhsuyg.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/giixpxzlx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gopytidpt.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gcxeoqqbh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gznowdqjx.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glgtnabis.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/garknfhiv.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gbrxmovoh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqofrvxav.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gekcjizly.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbupgpfyo.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/grfrkqfcf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwkkevcux.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gzyasqplc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gkncplzdv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/ghtkhtbfo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gyysymdym.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gvwsdmywc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gowypivnt.sHtML


<!-- 参考信息 -->