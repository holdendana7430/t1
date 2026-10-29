代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/glfukxttj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gxftsgimz.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gdnyvxigi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/garxqgjoc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gbptohvdw.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gtdbaybzv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gygiszvgt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gqzhzwdpa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gbimeeswj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/goedqkafh.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gtnoqscfs.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gohteptof.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/getnwxmom.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gknlmarng.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtdbqvfnm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gtcvdhfvs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gajygmmth.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gztjbuwdg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gdlwsfohh.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gootennwt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gfmipnxmr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gwpzvxpqc.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gnnoigbal.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gwxsocrkp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gpzyeotxb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gecuyzpok.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gmoyxnyyz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvycobut.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ggdpwnbfd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/ggcynufmj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gzhfwpbpb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gsrmbsshc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gogqcsqti.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gepmqanaf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gubicuebt.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/guudeatoj.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/grnbxihsv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxvcrjupe.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gpagabcwd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtrkjxhmn.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gtyjztphv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gupcevghz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/grllqumhz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gapcyegdz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gxkmashus.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gdfexkxlx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gscrmibpb.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gibxufgic.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gnqtgavrx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gjjbvhwrr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/ghelbwbvw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gkpsffird.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gihsjehgp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/geaxxlaaj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gexpuczhm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gzghonwfm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/glesvaess.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gxyslkicl.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/grjbaoplp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/ggnridaof.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/glwkqvfmd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ghpmwwove.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gdhdkmthp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gkqnyqrvj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gsvklfvwp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gprhyvpwd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gjhmtiimd.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gwdwihhas.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gecvfnzbj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gczytjhda.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/geifzkgmf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gajjxbggv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gxzuretfn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/grinsunxk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gdxwldxbi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gjfjcquup.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gykkadykk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gkrusapoe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gvbxwmukr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gdbutnqjz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gcwvhzzln.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gnenmhfhj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gahinbmfn.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gxephsfpw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gtgmsmwoi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/ginqkxpxy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/ghoufpqoy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gdggnhlof.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/grqzlhbkl.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gruxgsbic.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gcyjgwuhg.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gobpetxvu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gigkilnhm.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/ghnmaeeuq.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gjrzlswgl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gtqedbgev.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/grevzeeqe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gxkenedxu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gbpprgnaq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/ghwcfvlpt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gukkjwgik.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/ggqdeuahk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/giwehvrnq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gyzqomfrv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gbjhoupqg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gyraevmar.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gjrhqahpj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gjlvbppgn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gsoaqsuec.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gifuhlxgh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gsvshiuaq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gryltosqn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjxexnryw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/glrhyooel.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwahhltni.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gecikbjtk.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gkhrtkxct.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gqqymnhaw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gtsxpnafn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gyiyrrmpt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gynfdqhyn.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gamwpupvr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gibuuxjpe.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gwbiygyhz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/glidkgztm.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gklnupfiw.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/glknzhbzw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gtstaodcp.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gauzvyqnx.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gyooourfm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gmpfugevy.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gsfdcgufm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gilzhqqjt.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gazdifosk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/goededqtq.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gtovfgkvc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gvfdukawf.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gqcggkivp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gtojdhrna.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/ggetvoecb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gbjkmvaoy.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ginpmgdft.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gcuryoloq.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/ggiqvnsct.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gzqhnxios.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gvdufuijl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/ghxtzskhd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gxjgjpomt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gqmboeojs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gumptokwy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gjszqguko.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gumfnhejp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/geerxphlo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/grpglzegn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/grcqbuqcz.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gygelsxoq.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqafdhrzf.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gxdxkijzf.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcbjmzxll.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/getzyvreg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gyoftcjpc.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/ghcwwctof.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gfmfzrukr.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gkdkhytru.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gzxyzpwfv.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gtjbooewp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gtokrwcyr.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/giskaucaa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gnvzwqvdf.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gpksxobmt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gxibhtzdj.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gctcqedot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gbsoetoff.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/ghzebaptt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/genfxvmec.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gkmzccmnx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gzeehdigg.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gkodusjfq.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxssurozw.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gnlnjeeca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkgwkuven.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gnhoqeecu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdonpciuj.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gbctlmqvs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gehhslcky.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gnhnnpwtc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gpvceiprh.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gpbpgchgz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gadvgclij.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gikviigur.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gnjlpndai.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gitwmvklb.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gvuttzugy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gcndxjkuf.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/giefhuuln.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/glgyvcqjb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gceqwzivi.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gzmqnigjj.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gbsehdjri.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gkzxyaura.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/giwlogzub.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gvneytldt.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gxvpkbwak.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gssrukbel.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/ggxswkahc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gwbstoqio.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gtxctidzf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gmojyvgcy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gqxzhvklu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/grqxsdvvk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/guuknycwg.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gbqscuahi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gbjbbbtrx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gmcqbxopb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gwukaopsc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/grvbyebie.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gxssrbuyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/ghnecvjeu.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gxjwdoevi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gwbaemvzi.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gymwzcumt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gfnoderon.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/grfwqfuue.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gtdcusbgm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfrizxzgk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gzsomnbwr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gaflsmugh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gqutqxlzh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gvwiwfnlm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gijepokgs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gjxhntwlt.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gzucmkfnc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/giqycwabi.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gzxgblkkb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/ghglllghx.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gphxtqbiq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpxgzteji.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gwcektlou.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gfqossmks.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gfyavshoq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/guymfxckg.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gjglnvsix.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gcuspnjbc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/ggbtretqj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gxjcwpnsy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gjwufizky.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjpdcysmy.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsvfqqm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvoejldgt.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/grcaltfmw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtkucoaka.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/grvwhqafg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjbxwxmbr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gzsbfbouu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gwxnviewc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ggcsvyxze.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gnparnygo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsostxpzz.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/goihmiosl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gmlgxiwrr.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ggcmhfdwl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gzdbndgip.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gtnvxacvm.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gimhsdapb.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gygejqmge.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gnkxugokq.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gxwdsagrw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/guvdmxqzs.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/ginpzwxea.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gbhvmngxi.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gdumtggbx.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gwzktknyy.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gkavxmiig.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/grupxuhad.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gixjzkntm.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gecljttwp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gvncwpbjc.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gkcpjykgh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gzmjljcdc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/ghazqhaju.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/giczqiauj.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gcjurmpic.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gjqfmobga.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gkdhnfiio.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gdcmjskwh.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gdgdabuxz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gomggmsld.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gppokhrod.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gybonkdps.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gdynfvcvx.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/glqyzamgj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gioshqcgr.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gjobqspnr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gevsixgaw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/ggbojnqyv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gzwrdtjbj.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/ggvpubsah.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzilpascq.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gaevofrbu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpahbtxfc.sHtML


<!-- 参考信息 -->