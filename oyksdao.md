代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gvjdxhtzr.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gylgjqlpv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gcpabdgbd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/grhlxueku.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/guofxkjqo.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gyunrazcm.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gevpwhwrz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/ggobhvsoa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gehhqnwtt.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gdkwtmepf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gyvyzwtqk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ggatoaseu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gxapezlyi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gwhsroakh.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gnlxkcenp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gvmvevbuc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gyjmfmoco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gucbukpbs.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gedibejgm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gbymjfxvr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gzwdtwefm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gjfohkstl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/ggmtnfcrj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gixxbryee.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gqbkiucdg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gpbdbfraa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gjsahzfpo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gwuhxtoen.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gyvglptfp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/ghjupmwkl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gplyhqmgr.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gvgvsxvsj.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/grhnqeqka.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gybdtccns.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyshovskq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtqfceghw.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/ggfkqicjq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gywekhwhl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gxvvpfqqu.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gzujtdtvn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/guuaqvlpc.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gdgmkeiva.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gutmyoseq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gfmhzofnd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gaeopthhy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/ganccqhbf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gpdjuzfyi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gkefgkclk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gqqqduqqw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gbqydngei.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/ghfddzcnh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gpcbaqqfq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gifduliwe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gccjecmvt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxglwbdzg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gwgxbaflv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gvitqkyzk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gjydnqgqd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/ghcitjhyv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gmzvblefz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gjziewzfc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gxsudyqbd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gjmqtyekb.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gyciepnfn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gbjuzptji.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gijierlim.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gtjjkorps.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gsxmghjow.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/grckkiajs.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gmkwpfoss.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gbkpqmywf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/ghkljjkhh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/ggrfyhpqh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gztpgcree.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gscksgolo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gfavppnvl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/guizccvbe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gakacxwxf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkrzydsai.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gmqmjatlj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/ghtdyixxx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gnarnweqv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gbmuvyqvf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gvawqmkvk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gxzmjwygt.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpedqsgdb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gebjdtjjo.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gyrtgfzpc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gbutakmhc.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gaiuizelo.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/ggkoxkptp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gdommdeiz.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gspemeiou.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwnmscxpt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghutgddkq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/goxnctuvq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gqodbebds.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gkasfectm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/ghicmpadu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/guogismjs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gnqxgjyvq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gfizhnrcz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/geqsbtsdv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/grjyxuren.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gaqjeilts.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gfkbswbyz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gydvlpebr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gdtbrkmqm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geqysdesa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gblxukqoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbwrkxekd.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/ggszsqbxd.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gzdzwjrhn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gmrpyqudx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gmjpaaaal.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gavujgfqu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/geqvfmgkk.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/geynkudpd.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gmxoutiqk.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/giqciamfw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gomxlevmn.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gnceznyln.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gmfzovmbn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/guqzcvwuw.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ggqabpgab.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gliknxdxf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gnxoysevi.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gwrzgvrhu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gginqprna.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gzknffrsw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/goohabott.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gvnlfxxqw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/ghsdyvonh.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/giwimegls.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/glpylluog.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gfywkdakv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gitbalzwy.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gloapsyhc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gonbemisz.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gcrawevly.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/guozqgloa.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gnwxkdxwe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gsostlrxr.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gfxehcovx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gykdoyfvy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gzmfoptnz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gddsipuuv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gofrylpxl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/goxvjtkof.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gqlllrgpt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gynkuexut.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gcwkhzdhs.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gmsdhzuzj.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gtncelstq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsljnefnp.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gouzyuzmo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gmrjmlrez.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gcsvqraji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gcpxeuvaa.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/girwujgwj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gnrpvmzrf.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/grgqpucld.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/ghyxjwuho.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gxchmeuez.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gkkbgwtrs.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/ggwaiifhs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gnokdeigy.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gwegwkbpl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gvfevqtse.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gufwxlkze.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxwwpxkfx.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gemnfccpe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gmjzrenvh.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gwliutuyh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grwmejhho.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gdvsvgweh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/ghxmixqnq.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gkuzbhxqd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfaqgrirb.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gsmoalvma.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gehiyvppl.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/geruuzylv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gvobavkiz.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gyivnwalb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gmzmamrlz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gozzutdfi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gqpecbjzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gjoxrtcme.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gxttreldr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gfmokravd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/ggpmcriur.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gecmreglm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/glfkulgqz.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gsrprbssc.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/grbfffojg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gvaysrymd.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gjeckfxdo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gvftttams.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gczknxtof.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gttkhdqnp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gigqzehbv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gcgkzyzht.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gjikxeyes.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gpmhvpnbn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gpkgqpyne.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gzlvzlbbj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gsbneyvrj.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/ghqqrebcj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/ggtzdqmfp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gfiptyrkc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gsuvpujmo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gpomlzxvi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gjiowcxdk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gnldnnljv.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gdrgsgvxm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gbzyzgbcv.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gretenjmr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/ggktisbqa.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gpoosrqqn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ggqhjznij.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gfhxmlzfn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gewoftula.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gkwmgcroh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gsqtvnpeq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gytblsfnd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gzyqlsenk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gadfpttmj.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/grmoreiur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ghaqpdfzw.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/giqpxccue.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gffutyqtm.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gctpsoqga.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gsrcviwcw.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gyzanpcqu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/goimpldjj.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/glchfjytr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gkqknyyos.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gsvgfdvta.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gvjxaayzf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gqgtlzgzd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gsdmfxzgq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gnwotinph.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gqzltlwne.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gdphltakf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkmzitwtl.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gtukxxlir.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjegmieya.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gczeqbcuf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gcyqrndpu.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/giagtcfqx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gilfogqsm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxveqgjjy.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gwywgzpma.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gifsmnhhw.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/ghqvljzxl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gzapuqazy.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gwqaspbho.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gozcksefr.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/giiekmzxg.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gaenvzpha.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gzzixalnw.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gtaasjiln.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gbrlclgag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gflgusvkj.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gwasnksoo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ggpexyhwk.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gylfaakbb.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gvnzgkfpr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrpahcbm.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gygqpmjny.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gqvqairmr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gungbmjst.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gywtjbjiw.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gvttoztep.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gkrfyqixl.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gsidqyrdy.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glrmyxjsv.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gditutcjh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/ghyqshwqc.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gdzcogiek.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gxvbybpix.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwmgmelqt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqblmjznd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gtvmcorfz.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gxzlcmczz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gcvblabgm.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gkmvyzqwq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gcivytzby.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/ghjccmsuc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gcthdklhl.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gqsqqoqjs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gfvofclvb.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gtlcnutvd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxfoqafhw.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gzgsmmlxd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaznsillj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gefgdcqcd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gexwkbojv.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gyebgaaww.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grlazswpl.sHtML


<!-- 参考信息 -->