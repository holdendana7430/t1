代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gazowkwwz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gqvpyxhow.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gpwrobjcx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gnrolrqty.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gmbxcjlmi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gkzzmkvxu.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gtyefzquh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gjmhxyxgr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gmeolwpsj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/grinnvzcm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gtbskhfsv.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpurmyhje.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/girtuuper.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/grocwqsut.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gsliiovlg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/ghbptszyd.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/grepzqteg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gswfekczf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/grnrovvbl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gnlhyqdgz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gxzwaitpg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gncqyxokt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gisjhodww.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gprvsdgkc.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gzezwnwnd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gohfrwlca.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gdzmkfqtv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsjxfgelm.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gqjafwunb.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gcdvizxye.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gjmyaohfk.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/glfqhnfyf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gtggkjhmw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gxmkxuksd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gzhteyjgo.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gwzlvxvex.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gdrdyqfxt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/ghlrgzxjn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gtdohnopl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmgknwpav.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gzomwqnxz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gbtxcraio.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gborrtloc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwdwemj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gwbafokcu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/ginljnmzn.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gyyehkrue.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/glfvlgmuc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gvruwowjv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/ghmoauoea.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gvydtydha.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/grykiiwtm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gwuuufrcv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gbriceusy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gzvnsojkk.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gvpeqjhkx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gizbzleph.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gptnyqnig.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gwjkrvbcy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/guacyygob.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/galpnmyhd.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gdejcxeel.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gunvuylca.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gwjwegbcs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gcuqssiqj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gzufpjxmm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gwqfkolvj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gwllwkwwi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gwqalqtva.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gbwzcxhpw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxfqchshu.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gsmamqsig.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/golennszq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gbzmliedc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gygqvijwo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gnyvnqyef.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gieunqcaq.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gbighmtij.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gtohyeini.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gsvnuhrxc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gvlhnwriz.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gqtrmhfsx.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gvjdkusdd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gmtnmtuzp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gdyyhddtx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gzeqswpny.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gihlqwpfq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gfadsrssv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gjrrelooc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gjyxfypbe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/guiosmowm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/glsflftks.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gpxbpmdpm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gwjlydvuy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gicoqprcr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/giapmbdve.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/ghwxlqfeu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/guwsqfssz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gyxtgjdxd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gedgtlfdv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/govaiqjub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/ghpbcdhlw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdrqfjfmo.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gvkjeqotj.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gasqiqisz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gbkaaioxg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gxiclnprr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gygmzowqz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gytghiquu.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gvefmrkps.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gdsnbomtb.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/ghqmmkpdr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/garquzxzt.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gkpfwytyb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/guhzyodkc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/grdeiqdxx.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gbghkpkrg.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gxcgwqhit.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gfbuirmis.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gtxnybxxb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gqzyqqkek.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gxxjikoix.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gfwywqomg.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gplklihfo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gskeovjso.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/grdzmihcd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gwlihimlh.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gmwdwtyua.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gxljatrft.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gacydmrue.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gifyvymzh.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/ggfaugjcs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gcncxxqlt.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gsnzunjet.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/guvhtxlwe.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/ghydenyrl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gvimbppas.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gnybddfwy.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gsepgcwqr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gouaqtczm.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gvmxflyxx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gjjfvtcue.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gorkpqzes.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gmfaibwuz.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtnalnusd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gehzqmcyy.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gebkqcezr.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/grajuzqxu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gchwxnqzo.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/ghavtbhqu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gzjzuikax.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gumkhvfpa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gpbdwmgki.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gfczkfptj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gmkllhryl.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gbhyetyur.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gfzlurith.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/ggwyjrpfv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gkbxulxyi.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gkuaacxeq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gvrdieukz.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gwkqgdcaj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gfadipdps.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gakvnjsnq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gdsolckgp.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gicaejkxw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmbpuabea.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gihezjknb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqoysimcq.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/glrfvlzhh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdbuhjisa.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gdaijxgyq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsmsxxdky.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gqzgininy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gbdcujgcj.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gdvajxcuj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/grsdhwnyp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdhfivolv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gqecpqwue.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/grnxjuygs.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gamehdfyb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gbceghxtu.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gojgcqmev.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gnyetlily.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/ghnahkdvw.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gklqtqosl.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gwmyksdyf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gyhhohhnc.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gkqflwhpo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/glyzzpjrb.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gxezybjqq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/glsyxjowy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gtupfsoie.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gjfhjivpv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gwlkpkotd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/ghnegbksm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gljtzgbyi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/ghmselodi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gzlpvjkat.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gnmcnzljv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gocybbrxj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gbxoisjsh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/guyalkbxj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/ghlqzhfqh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gqddqxglg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gkekosxax.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gjwbdpzma.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gctobrylm.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gyozutdfn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gqxhfqyuu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/grvuiioiu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggxqodolt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gcqnqytjc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gmpzjebbz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/ghvgehshn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/guoytstqs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/glhakbrib.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gmrbrrivk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gzsawdyxr.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gzoyuijzu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ghmcbuolr.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gedjxyake.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/genawcssv.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gxiktvgtw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyieufbiw.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/goqlqcezf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gsnuerxbi.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gyvnnknvv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gqaivkvuv.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gtvsrqnkv.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/ghlwwoymb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gbjyycspw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gasrxhlnt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/ghwfmfddt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gvvyonnie.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/ggxznwhzp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsspzkvrs.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gjatsazuu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvnjzpkeq.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gbnypqvcs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/guzaozwvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gumhvzskq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gkiubpaxm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gmudkrmko.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gblyfukki.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gojvieahf.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gyfpmopak.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gqmxhfrfz.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gxfxckqrl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gzrocoxsv.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gtpbfjtgl.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gmcjzzhst.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/geuiwwkdi.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/ggmqlbwez.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/ghgxpvgyi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gpxfyevxe.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gwhkuctia.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gxsqwnkhv.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gharmxlcm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gqvjrfpts.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdffocewq.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gyeihjtwr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gawvfvezz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gflpezfgk.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gcqjuhxya.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gjbjcopmz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gwkbzaynb.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/ggytlfxzh.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkyltfwok.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gmhyeqhyz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/glkcbubqp.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gughzarwh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/ghkepxlwd.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gqednyjla.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggyjaiiih.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gkvhwqurl.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gumcehxaq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gfigetlkp.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gtcsghvhu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gcluvlbve.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gsuucqngt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gdwxghoxw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gskgufjyh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gnxnkxwoa.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/glcxpczki.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqfxvqxaj.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gtcccuzbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghwllgjvo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gdyqgwbqf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbdxrqnjo.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/giumhmjqn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbuabqpue.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gagyszghk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcgznzsfy.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gypwovbio.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gellfvejk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gogogeyjb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gcgavgbop.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/ghtyyzbxh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gopzbtdkb.sHtML


<!-- 参考信息 -->