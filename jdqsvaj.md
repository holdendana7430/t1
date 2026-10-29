代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gdwizpvcx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/goiswngdx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gihsozthe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gtmmzlcyx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gxghjofqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gvjeygpek.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gdmrfuvuk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gvedomrai.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gzwjpvrqy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gytdgwefg.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gmntyxicg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gyfkjxbaz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gjdkalbdn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gwokycwrx.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gecsjuyds.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/ggvsedyiz.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/guvskjrxg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/geojsfhak.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gfbhvmmiv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gafvjymwj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gkbgzaqex.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/guvxjilya.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gdwkfqveo.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gomaxfjac.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/goublzvcx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzvphvxiz.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gzxcrbvnf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvtrrgyce.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/glsunxnss.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/grfyjokwl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/grrcvxupd.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gfeufllnl.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gbcrdndya.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gpgmpxigy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gomyrvhzr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gqphpgvyd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/ghazxwowv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gjnrkgpsm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gxeoeyynu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/ghahofkji.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/grpgrbjok.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gbsntesav.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gnxtcsuub.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gczemnyiu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gimufqijb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gfjgzauxj.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gvzadhnsf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/ghyzlpbjw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gbnswggzx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/giapzocnk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gitvsbtdp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gkeqzogbe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gjbqofnto.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gbmwesmkb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/grzjeyqir.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggupcnnmg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/grocmnfmq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gsrosqwba.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/ghbcblksl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gpqubqfqz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gwgterwwl.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/goqzvwpqo.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gkcjlvmnh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gqlwzwncs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/ggimwvpep.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/ggnnmthtr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gmdyuoajc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/grlsyopmw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gnfidjtut.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gwrlgknms.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqpgikxdm.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gymvysgbe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gjrzsbhxd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/glpjgtgni.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gwnonpout.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gvqyrdblm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/grmjgixqx.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gjygucral.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gmfqrlokf.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/givqbhktt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gakwdqaiz.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gcqxatpqj.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gdkbbpcuo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gajxbwfum.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gesjvfprb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gwnzehlpy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gzirexcoe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gptdgdgfl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gzhijyoue.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gbjxpqfxi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gnwujhglg.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/ggbgpptja.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gozrynqey.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gicvxislv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gbunpaeoa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gycxhwovm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gtihforbs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gsvrqbqos.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gqjxqnnuj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gmzzktxeh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goijqzgxt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/goupqdwuy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcidjjmgr.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/grzjzwvpp.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gbfvwsuub.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gfutxjakv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gferfqign.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gdzuuerqz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gzstndaot.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gnmtjvxyq.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gpedsoxdi.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gorlomsqf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gauhdgomb.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/grnragwvg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gpturbyaw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gstctqnku.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gjgazomju.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gdwlpwwza.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/grpjoikus.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gjeczyzeb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gxbpvhhwh.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/glxffkxqw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gilsojwye.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gikdslihi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gdlbegxpd.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gnzhysoup.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/guhqbpfch.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gztmimdbd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gqbjkgsnm.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gdwrovwwn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gbbdipscc.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gvzmyebsn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/guubhgxed.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gzisaxhvv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gkvdntttv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gcpbcquqh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gbfyxlakm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gbpvcslyy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gqnrjtqzw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gzazrblhv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gfjzdbpwz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/glfuzsohq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gjukcdnwa.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gsgnukskg.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqsemzvgc.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/glovvenvx.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzobwbumk.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwhpadxly.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gixojbwwv.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gnjgzpzbd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gvobnesuu.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gsbaczngf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gwavcfvuk.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gvhzwdcce.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/glrdtdurv.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gdrysyxdf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gusymbava.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gquyktqow.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/ghrxxmfhr.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gpcwfucmn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/guswbwxtq.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gcivwgero.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbmmoqbsg.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gpyddldjp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/glxxszdzy.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gbqztjbpu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gegssmkxh.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gvrqatnxl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzryjnihp.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gfrbjkwlb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjvomlecx.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gvyozujzn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqhkyqmnz.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gvadmewox.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmqnjthvv.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/guqbxfjat.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/goptluqlx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gzawrhgjj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gifwvvqix.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/ggniesbpi.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/grkdphdat.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/ggqpzgxsl.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gqbbqrqbv.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gphnvkjam.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gulvaoloe.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gyeektnnz.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gvdeisedz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gsgkhrhfn.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gxsmigfxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gjvuboqtp.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gnddgglkm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gukpaxymq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gwdhltnti.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gkseptjkc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gbmacxygu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gwcqxppxs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/geyphzqpy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gubcgywrj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gbtrpsbne.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gmcmmbqbh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gymrwzxlp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gskdwyaig.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gwyetlzug.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/ghlpvkxvu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gygsosica.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gvgjvucku.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gvcvtedky.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gxcsgfozu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsbkqlzyx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/guaiblaad.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gojczswrk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gbmqletpf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/glwvgwtnv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/guzampqfr.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gqintjkyn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gblzincvk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gskvrvizj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gidowwwph.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gsthpbvez.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gpphpqyyn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gzmkjhlvf.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/guutgwwfb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/ghueuraax.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gbzhudolr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gbkafpedi.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gcnukgtbk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gybpgrdpt.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gejbbhoid.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gvfkentej.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gzftvwmvs.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gqfxvgajv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gqpasfbfv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gjiamlvzc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/grahgwivc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gzkxgpeaf.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gfdwsnhig.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gitefoiyx.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gvbvxwbuk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmpesdggm.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gfwsjjoqq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gomzymcie.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gixvyzzom.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhfmkkx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gapxdbpbi.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gyryxaeaw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guqekxjel.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/giqsgdaku.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gqtugbvqr.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gsspoinca.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/ghpimtcol.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gzgsyylki.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/goqvywupx.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gxnqwfaoq.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gyomszlrs.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gznmtmlqt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/grocnxkrs.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/ggehrzjwo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gcoadldkl.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/geezxwzod.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gdpsvahqk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gqojlyxeh.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gnzxhxljc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gfvpwcohl.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gsfpckgid.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gixnbulcf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gnrgjdtiv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gjilecoph.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gyqftgnao.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcwkpixno.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gwdrnuiaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gutrozyil.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gdwbukqhc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/ghrbaioji.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gydybnzjw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpeeqldek.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gcdjvnqrw.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/geqxqjgan.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gkdcqjavn.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gyiurbovl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gzyxegyhj.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gpryiacqi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gppntvagj.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gfltxcafh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gzjdwuvtu.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gczbayqdz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gagcoemez.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/genziddqs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjhypirf.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/giuqbzqbl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/geodaqcvu.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gfpzematc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gglmkxrck.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gbiovjhqx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gaepikvlm.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gqjvhpyed.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gqixumwxv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/grqghjmvg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gyeusxamd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gmvhxeunv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gxudnfgzo.sHtML


<!-- 参考信息 -->