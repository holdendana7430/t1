代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gsgrgeonj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/guozzadtw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gybossdgw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/ghnmttuiw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gbicvfpeb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ghtiuzewm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gaizunjxj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/ggrdrrfpu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gcgaezwzd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gfjdctscg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggpydksqy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gibkvouzd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gfhfhqtua.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gcowxchhn.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gobanqiux.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gagzoguea.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gtobwmwkd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gzeeixsoo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gxyvnwmhz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gczpynfmt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gktqcwkif.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gtxxbidap.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gnoqcemde.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gaqhzmkdx.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gjovylbtn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqlgmkgiz.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gfgmotajm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghoijbkyp.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/ghyoxewoi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/grvqvuaeb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gpczdtvmf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gzmzzoozk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gxuhmatuw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/ghhmlnyxj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gadfvdzwc.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gykljyxzr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gkbohdfdk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gksuixjrr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gqtuszzic.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gsqfgtndv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gbcabhllj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gghvhzesj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/geolrtcfe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gwtletsyp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gtvfzavny.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/giopygfqm.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/ggwzniyqx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gapgqokzm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gewpitkts.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gxabdfsbu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gyfaiqprd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gouhnepds.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gnzkfoyfh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gnwzwnzex.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gtgmwcyld.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gbcvcbbbn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gtcvdnrhq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghdeqntcu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gmjsdrpmb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gdzdijuqg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ggwrcqljr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/ggfbjidxs.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gruftpytw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gwoujpmnj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gafflpkuu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gqldnqrer.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/glkrdrjyv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gcyosprht.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gwbqiohbt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gzzahbhpk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gjecxaeke.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gbsbnoyrd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gabcywewj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gjmmfefvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gqjecakkj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gkipeuelq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gkbmvhctn.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/givpvwowg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gdbwokgqu.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gvlhnahkz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gtkbxkphp.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/givztgutz.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gorkmugpf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gfkhagfau.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gribssliy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gawfnqzhz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gyrnquuij.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gtgxczxar.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gslwegqlp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggcaliljd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gqdjlmsqn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gugiwdqmd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gkivvfxxl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gygftymwf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gxwobtfpr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gdjfwiefi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/glbzdevsg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gwobhiyse.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gmjgofwbo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gwtcddyxk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdorqercp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gxcyxwegc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfarrvjsd.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gqmnmkmkf.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gokchpvgc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gtxmwdlbg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gujdpqlbf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gcclzokdy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/grnpguuol.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gdcjfaunk.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gpqsnfdrj.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gngwzhnxt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gdjlfyvhe.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/ghorxkrcg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gjvymfbzr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gbhsnepse.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gzdtsafjb.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gaxqwlmex.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gajnhtyin.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/ggtaacjdv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gybnxihol.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gbiwvbpgu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/ggwlamjvb.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gmxzeoawx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gohpxtjyo.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gclyrpxdh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/ghdsrcqhd.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gzajjxmyp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gditsytlz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gwbygyihd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gwayckrji.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gedukmhui.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gfzcvpygn.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gvtyswiuf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gvtkksvyy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gewrcbffu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gjtpiiuoy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gwnragbuv.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gktievndb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gsviafmzr.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gbozuuwij.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gtnlwcgov.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gclasgcpf.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gvlnmvcxb.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gdecifalr.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gcajjhzkr.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gscgtvxhz.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/ggkejuqiz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gmqdidlnw.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gaqrcdatn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/guinjfpaf.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gmeftbdis.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gfsvbhgxc.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gqxxdammq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gfvfjbocr.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/guknxoqlr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gokckdslx.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gnoourpww.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gaimbwpar.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gtelbkcic.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gnmcswxic.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/grlpaexeo.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gligdjwal.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gzqsqvmhr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/ggqtgamkp.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gexrdvfia.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtdzwvpqj.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/glaxeyzpt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbeerumlh.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gbodndpgb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyofnsxir.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gxjogmuea.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvwedwbuw.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/glztichhl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ggnjocdzq.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gghehriju.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gcaxiqfqg.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/geeqtpwxw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/garbhfmea.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gyyfcrdbk.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gtbozozzm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gwbkzueuu.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/geumcnexm.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/ghxdtgjpt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gylfxjjoc.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/geusrhgdt.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gxauufbwi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gbjduxola.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gbdmrscyo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gocixoida.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gvdkzbfbb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gygdvgfal.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gyunoegxc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gbjpzaclk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/ggxijeyyw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gljwuahwg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gghpmbhjc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gnfdxqotq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/geuhykpra.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/grfgvlniw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gujonlvyr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/ginvvzbkq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/goatbabhf.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gyzjathcd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gphtdqexb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gicxibrmd.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gxfqkenot.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/glzkkjscv.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gdflqnbfv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgcmjrir.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gofolgyrn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gtuwzcvfs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gvlnzclrx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gewkobbdr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gtvnwscam.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gkjdrrois.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gzhrxgjyq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/ggylohvng.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/glbuszhtc.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/grejwcwbd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/glypbfspd.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gaarsliqa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gozbhamhh.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gttvuknqg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gwhaihmix.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gccnbloel.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gdkjcxjow.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gpcrgmjld.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gnywphxnt.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gdhbmnrex.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gmnhbriew.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gevxtmfzm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gysbqfzjj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/godwyzopp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gqtxgocqf.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/glbcliqbc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkmceuoub.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gzcmohvuf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/getrmfmpm.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gjjsxxbnw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gnfgclhok.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gbxlhjzcp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gkhkyaxol.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grmxuydpg.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/glsaoavhz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gefqxkgdk.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gxefmeyhq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gklkurnpf.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gyudaiiil.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/greftirzk.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/girwchxyj.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gkhugwlvb.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gdbpfrptr.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gdpkcptzw.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gtmujgwpp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/ggqtrkgbb.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gesuadiqj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/glczszprf.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gfxblsvsa.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gcvivzzsk.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gretoztbm.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gwtlokfqc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gbpfmvgvd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gwkbykfuf.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gifzndely.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/ggimklvyv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gybmhghbp.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gsljlptyj.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/glvrrblyd.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gwvoinqnr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gyglctjsr.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/glxsxuvop.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/ggrdpnrup.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gumvujsas.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbvsxtrut.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gdyymbxgp.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gresqekfd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/grbpyfwki.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/grpuqmehx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gdqhewxka.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gahidelun.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gpzpbivsl.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gefeacjpb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gqwwrjnwr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gkixebhwl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmohpufsz.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gxvmqsyza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/grlktogos.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gauyvpawk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvgzmxlfu.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gyitfdsdz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gktyvxtly.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gnlazutmd.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwgvktmhx.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gdgklbmtw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gblmluowi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gavhmybwl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gazlczeaa.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gzwnjjetg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gdefkkxpo.sHtML


<!-- 参考信息 -->