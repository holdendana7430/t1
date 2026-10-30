代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/ggvwtjtin.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ggpvthuzd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gbnaxazix.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gcnpnrjhy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gvyjoadhw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gnqykbkbr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gilailslo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gzmvumfta.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gbwjifssu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ggepwosvt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gqqxpyvum.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gwgzhyxhf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gaqscwinl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/goajboemp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gbpcarpok.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqmzwgoym.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gpmwwgycj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gprcopzqq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/grxcikpeu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gpintlexk.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gyblvlgjb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gykzgokgv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/glllksova.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gebndwxst.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gfhgajffn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/ggebucvzq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gkzinrugx.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/grkbntbek.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gvlohjwvb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvrmbgsnk.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gevkisnui.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geykekvuy.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gzllpsyct.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gmelkadiz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gezbsyytb.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gmnbobmgd.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gogoxhert.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gigjnzfln.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gwsmydzqg.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gzvimyrep.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gjigxybcv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gxralnhsa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gkqdxyvxe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gonsfpzgr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gvfyhbwtp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gnbzdbxhp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/geyegcfhv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gjzxhyzda.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gpezzokjj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gjpucaltf.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gcaztmman.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gghhcljei.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gtqwlxwjc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gcgvfyqwi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvroloibk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/glufuakjh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gdtdgrnzz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gvecgnlzl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/ghrdecvzk.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gulmzwtyt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gphumwweo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkbsehuuz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gzhziakfq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/greokodqk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gbrjxstdo.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gqevnbfxq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gubahfptt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gedfadrqe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gmzeeokir.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gbsupfvwz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gkengvnid.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gbyhlepji.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gwjmccyiy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gdssaknac.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gatrnikkz.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/ggjoohjeh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gmgrrdiaj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gtjoowyzo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gnopbpwqt.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gfrhcfwvi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gdfgcuogm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gghvhcbdy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gdniioemm.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gukkzsoig.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gblqtzilr.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gucgvpnes.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gpcbgxmup.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gqxbaejca.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/ginjwtsdg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxamdigye.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/glyhfxvse.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gfwjaziwq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gmxehjpiy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gkyunhzsa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gjtsnpate.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gkkqhutex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gyhkzjmod.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gxoglbizt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gjouwinma.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbwllqija.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gzqdnmntw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/ghhieccyi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gpdlwdjaw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gyybelnxd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpyvoylpz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gsqscylgv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsvmhwjzd.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gpddfbini.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gsvqvwupq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gifbnrmys.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gyemdrtnr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/grwgnfcio.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gsnaueptw.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gxapbjoym.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gnapdehyp.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gwksogygn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gzxwfsahx.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gesqioggz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/glbscsjjh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/ggbxkieaq.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gmtzwgfkg.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gpsrgcgml.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gpetqiisb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gngbietfl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gtjkqjqyg.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gqndnrkgk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gzjrinbfb.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/grqwkdsgt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/galakysar.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gtoohaxgn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gpluvoddb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gesckptlm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxrgvfqxo.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gcjdtihsa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gzqasiyfc.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gmxhkwrff.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gmdidqrvi.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gmzrgqcgd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gpprsvxxw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gctbitepe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gxqseswwz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gaasaonvb.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/guqxvelrf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gwsmtbztb.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gwcbtqvkw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gwqjqvksi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gwybxezxf.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gpekdpckn.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkadxibkj.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gjkcqkopn.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gndrosdgs.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gwuupkrot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gqgyxapde.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/grznihtwc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gdmwzqbet.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gdxphccln.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjvjzuno.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gthnzbjal.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gnufxtobt.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gpsravmwy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/grzearlqo.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrfqsqq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gyfdhtgvv.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gipdtbrja.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gvlwsgivf.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gfbyvpsio.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gbhyahbrc.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gkqvlsxdv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gamgefcbq.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gbqitzzuc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfnqutlch.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gtswjaivd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/glqzatbfq.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gxmqpfesh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnsoqgxkr.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gerupsizm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpftnluby.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gdskaprnx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ghcaxdayp.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gmrmisfau.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gakwpshzm.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gpalazufe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gwsnynrjt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gjdzsfeqy.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gflxybotk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gfimibbbd.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gycfixqio.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gyiqbibob.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/giojbsomr.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gpxrtlvax.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gmmwuxras.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gnsgtyfew.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gtdvfqtjy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gpnigguah.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gdiztjuwf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gmftcodzu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gvzofdrhp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gegqeuztv.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gqwhyeuju.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gpicdjogm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gxlflazsm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gfvfmniay.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gwsykjifs.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/ghnpbglrj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gnleszmgh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gmghibzck.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjxgrukpd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gapddjfdh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gazurtvml.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gwkvvarbw.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gawgweblo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/golzfgjyx.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gujenkycr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gpzqnzcpc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gfciwfarn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gbtisnxcq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/glyyhuqit.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gbovuwiri.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/ggwweajuv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gzphrrhng.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gcjrdqfls.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gecjdlizi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gilxhveyh.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gowpvggbj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/grtjygjzb.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/goebquanl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gidkochur.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gslziikhd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/geyqafxwe.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/ggihoasxd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gkifmxuxh.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gqmsuwazu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gmqrjdjgv.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gczjacjxw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gwiaoskre.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/ggekqtgqe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gksdqccre.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gecmddvke.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/geanlsjsd.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gljfplhil.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gveyoalzx.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gwwlippov.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grasjxyri.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/ggwvrdfhi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghmpxmqfp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gfpkjvinv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gckdcueii.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqbaydnzz.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/guhpthvpv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grpxllukf.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gqfkaqcdx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gfkxsvwdw.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gogllsbay.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gtspohckc.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gvirirbnk.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/goujpbnka.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gldcxtviz.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gvewkewxu.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gymwavbzc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gqmdxddzw.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gzlshdrau.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gdykygdwl.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gqpcctrcz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gfmbrbfan.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gyvwojzji.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gaaamguxt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gdozbreha.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gdktnzicp.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gwyydscel.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gimycwdog.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gtujmjwsc.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/geybohuli.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/grapskenk.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gsuitxxns.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gibfagagc.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/ggfroldki.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gmsseywsc.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/garkohjgi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtagsnbeo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gntznhdhy.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gfuhdwyuh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gotnmvobj.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gkpeplhys.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gtfievxbe.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gvgzjglva.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/geosffuhr.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gdsbsosno.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gosreoyvs.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gellgpcgi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gocwrstte.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gopnndmdz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gqvpvevzj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gckwcceph.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gojwqrpry.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grahnrjzz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guqwoccvr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gvflcqxom.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcyhipdwz.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gboiwqzmj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/ggzqtaxui.sHtML


<!-- 参考信息 -->