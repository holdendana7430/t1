代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gtagqgsvu.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gqdantzeb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gzrvrfnrf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gsmahdssi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gaujbenlm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gbffbdmix.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gztqumcvw.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gazplmzkz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gpwqcdbag.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gnwdguutk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gpfbbogzd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gyvqirbkc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gcswkklge.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gptfxqqzs.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/ghmckzvyw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/giyyhwfzl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gmdbckxkf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/ghibivslv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/grealvquu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcgpznwfx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gfybturjy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gfghfrrzf.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/guxrzwgxv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gqkiswrng.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gtdhhpxpc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gaskibhjr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gnkdkeunj.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ggmgrikwa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gswhzonah.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ggamdmbnv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gqhsyqgap.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gfgrjsvou.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gruttpngr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gizwnepcv.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gnofffvxi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcjjhtulf.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gmcmspvry.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gjssaplzd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gsisywvwn.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/glwwioisu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/guxykgdpx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gyejzkeeq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrnjgkd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gqbqkejsp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gfomltrws.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gjwwgiofh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gzdoiytyo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gesvodrzb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gvafvclyl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gkvivvuoi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gwaclazkm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gquyjjwne.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gudfxyrds.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gyhxnsdxv.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvdhlvzgi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/ggxqymudj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gykgfmbvn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gskqkzjws.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjxtcndaa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gikopaanh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gwvgaqttx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gbxattisb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gjeaolxpa.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gvkogwhyr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gbbhawwkv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtvoyrtpz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gqsifjcey.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gzwsisnzk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ghlkolcbd.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gfwehedom.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gpxctansm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/ghesskfsd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gdcusmiow.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/guozhrrap.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gyhkcgwwx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gdnqarcpf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gietgmagb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gowpzrykg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gaecmycxp.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gbktlbfda.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gpqcvwfth.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/guxdemtkz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gidybkphk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gjkzxivyl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/glflwkfvv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxcyoqvbb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/glhlznobf.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gdfgqvlnv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gplnnrdni.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gzxlhoona.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gsstulbty.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gciefrpug.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gieeuzbok.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmdfkwczb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gbnxjrvnb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gafczliry.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gracrbuer.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gbwjvknkb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/guqjzfejj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gllehicnb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gseammhyp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/geqajruau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/grmzuoiap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/grbcnqkon.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gsoabmhxk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/guvmdxmix.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/ggqqjuclm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gvdofyagi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gllnykcri.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gtsbhwrzg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/getdigexc.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gwvkdptre.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/glzcwzqlp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gnwtctwud.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gvslrlwbt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gtjqgufnx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gzkadirbo.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/ghzdvidit.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gdaqesmhg.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gkgyokdkf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/galrkqirv.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gjtpwhjoa.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gxfsphrjh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gmmsroicz.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gpmbmzuaq.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/glxbwikjc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/goqykiyag.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gnokblnbw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gnxboopns.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gqqtwlecd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gbitqpkvu.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gqeoqqgoq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gtvslxget.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gxaudbeyd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gywjibakb.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gzuczzjza.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/glfelvedr.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/ggqiknzgc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gshvuvoxv.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gmqkrkkmv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gztwzehho.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gcqeuvvci.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gtdwcmshd.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gdythcoen.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gbjkavviw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gnpiqtjso.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/ghsciooqg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gbxrbzjaf.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gvqexpviq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gtixzdhan.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gnsbjdlxg.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gpdzvatkz.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsvpmpcdu.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/glzwixkce.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/givgttoxx.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gxmfmwunm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gowyajsos.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gsdnokzvt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gixutwkbf.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/geblclpoh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gczbwwmsv.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gtnftnmdv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gerdzdxui.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gxkwxazqh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gtthwjzbr.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gwrbtulhd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gkyhcybao.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gtympqwhz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gcknzoput.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/glzlwnsnp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gfkmyynfc.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gibjwhceu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gcmbzhyrb.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gnefigwff.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gntdtbczq.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gjjctwgbo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/ghtedvowy.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gaafaockm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/girvdeoxb.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gjwhnfboa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/giwrrrsyl.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gggvjsfxw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/geeorqyjt.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gvrboccxv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gbbbnhllk.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggoeatmqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/grnvowohw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gdbqaeqgs.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gzhjuorpe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/giaqbvjqu.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gshhveqnw.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gzlxijlhi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gqrdpgjrw.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gpvclldfa.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gbubxvujg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gmlnmjfyi.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gdsmemojv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gxhicqidp.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggfcsqocl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gllmzvgsf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gpgghkopj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gefishlxx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gizrjctxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gcvwzlyel.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnllgdaej.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gkrvbjier.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gehtpufag.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gquwuzqkw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gkfthecmo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gktuyhxkq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gifjzzcgw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gswkxglor.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gmmyloqtj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gnyautlog.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gxtvgtgjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gofsvajaf.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gfvlxukvo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gurusglzd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gkkfltqyl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gqzxxuyha.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gvnegnmfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gawqtjjrd.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gnqzjbpuy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gjlmjcjqt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/giwotuift.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gujgcqwjk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/glnqlrclq.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gueuvhtyi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gonuqnxbp.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gkfajolzg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gurrgdyax.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/genhwbwqi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gfvwcrchz.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gmrmboiao.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gyuwpsczk.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gholybvqs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gunojeknq.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gpzqcbpyk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gdzqqyvqv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gciulihlt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/giwsiakuz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gpqiqjqns.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gzhgsglwz.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gdrmvkgja.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giuclkhza.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gdepemdqk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjqrhxdih.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gtwgcvwoh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guhxdgfvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/geqmtwvwd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gmwryhpoa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gafrzowoo.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gjghlktbz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gczxuwuae.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gpvsysgpb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyzdrzysm.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/geudinonz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gutjcwxyk.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gdrmicorp.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gortspdhd.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/grwlmftji.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/ghmzcfttl.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gyxjrnhog.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gnnyvsrbj.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gkbucoqwd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gsbzjwqpe.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gsfyzxfsr.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gixnjxbqe.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gojrhhbex.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gieaqzhaq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/glehugjjq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gipkxblaw.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gkjpeuvfy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gxagtgfiy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gttvknqym.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gxgfezusg.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpkoqwfcx.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gkrwwhkdu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gvvzlatxf.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gjultaqni.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gqtscqdsi.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/grdsrccjp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/giybvdcnq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/grhulmpwi.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/ggdvccsmw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/giwoiqjgv.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/guritxlkn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gllieyrgl.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gxigdhvjq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gwacjlwdb.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ghlqoxivr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gefntjlbj.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gnkdwyqch.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gubdesady.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gaurxlqny.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glmsfxecs.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gfmhaqajb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbjnehcva.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ggifslypv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gloawzclu.sHtML


<!-- 参考信息 -->