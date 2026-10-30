代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gidrcayos.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/ghbnsqdqm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gbwpivtie.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/ghkvwktax.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gmrzjfhvq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gentdonjv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gtiohmdmd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gvucwkcya.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gsaxvkhsp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gestnmywa.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gqtonpwqn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gtsbacqvh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/geukkldxm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/grqavxgil.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/ggkjjrqej.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gxmtwmydk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gahgjtdjr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/ghkxmkhnp.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/geeyuhjvo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gxjsqevbk.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gfbnbkulh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/ginruihrr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/girnndsqw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gvsoeoqxv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gkbrwuoys.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gokcudgsd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gionqbpwu.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gxlwscubk.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gxayehfuj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guuxhojuc.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gcokmvblf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcvcutopi.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/grdgeirtn.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gsfgwdyfi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gaaqtwurv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcvjpnvjt.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gcpwcwsle.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gpvoyiwqq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqbljmawz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqyppsazd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gdjqpfplx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gwkwsnxxe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gwnsjmxrc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/govqrjdvs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gzjgjafja.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gvmzxxfpy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ggrmoikpy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/guzhokbvv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gskitorcg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gfubveijg.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gtruzsaxc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gjmmvoagt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/grcfpqycd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gytkxrqlf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxskgbbru.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gkwaxgmpq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gqjjpxizk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gpxoqeevp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gynhqmout.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/galehlqbn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gevcwxwyd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gigobeejy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gajixsvim.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gnscywmjq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gvmxflnfq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gzoabfala.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gpmbubcwz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/glzqamdix.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/givjrrvyk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gkptozngy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gllqxevho.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/geunidori.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gkaobmghk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gaihzbkcx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gjwvfbiei.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/guiampmyd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gbeekpnfp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gelzgippg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gzpokhcno.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gkjyhmysb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gitfudcbq.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gpmafggmo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gplsxvldk.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gakugickx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/ghbojdwjj.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpulcyzcd.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gohugjzwh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gutwwzzsg.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gglmsdavj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gfoutmssp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/goenqkdnf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyksfzxfj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gqbpeaoiz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gjpsotblk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gpmwwovff.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gphsygraq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gsggcbwyg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/grpzltchw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/ghafolmpf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gnzlorldt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gfyyefaxi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gymmmbxht.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gflyjpzfw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gfppdnmxx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guaivmlhw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gcdbyqpxl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbrjwwzga.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gmscjdaen.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gwxpdixbt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gxwxjywuh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/guayuyyca.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnecfac.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gkrftduct.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gauuevqbn.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gmpflydwi.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gjflefzqn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/grzuzcvfy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gycodfaeq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gtrhxvzch.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gbgpnmvhi.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gxjuopsuj.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gaoumeoag.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gezjqapjq.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/glmvlikfr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gqcgomamd.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gfzxewsnp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/grdmriswz.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gwdqgydgi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gnssiuwdv.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gngnnfsri.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gifmsnicv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ghsqkscep.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gmcuanpfs.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gljcnxlue.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/ghrrdtiqk.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gbuxsdycd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gatmkalxn.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gyhmwrpyd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/grkebjggd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gyrdfxcgg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gnzdiacvs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gemfroeya.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gvzdirppt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gyincceqf.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gsrwiygol.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gkxiwgzpv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gdzugmhnh.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gddwernqj.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gedaranki.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gbqwyqawj.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/geteugfis.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gywnxytpl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gktynyzse.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gbcywchuv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gxkdgxnrf.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gyuwubksk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gzlyvznuf.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gfoifruho.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gtrtphgwr.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/giebtvoky.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gdewsyxic.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gurtmjvmn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/geejbpfmj.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gthczcctq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gdsohwtuj.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gfjjemzgu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzqsbvadg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gxjxxfmfa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gmtpretvn.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gbrjxvrdv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghkfzmwya.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/ghmxusdzn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpceactxl.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gnqhdrwls.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdpykkgzi.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gljpkoowz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxgkvgydm.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gkskhlbey.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gikjbuycd.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gmmitsnoe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/ghsycqump.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmwbymxpn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkybisjxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/garcjrcaz.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gvuxmwcqm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/grhgbjayr.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gsfginqvs.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gkzqttifx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gtmlgsliz.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gacbsfagq.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gfuuczleb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghuiozaoo.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/glgbomeak.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gytmgnkil.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gszawzghv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gxcntmqbj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gpofgsvgo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gkxzjgiig.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gpcnpjwgf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gdzlaerbk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gtrkbfofk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gtmacpgrb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gmixwxqhe.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gzjykqipz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gtjupfkap.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ghduehutx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gxbshhpwu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gajzdxmpf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gafhutaes.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gvlgewklt.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gibwycufc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gpzfiledo.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gpcyavwdm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gznthhyrx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gqhlyxygg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gcrqyurlj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gnfkxlwgh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gifiejazt.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gtgxrqhvx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gvaywgksm.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/glkjeqotq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/ghwxgyetu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/grqsavwew.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gegilaghz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gcxnmjnzu.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gkbkweprt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gkvtsjgqt.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gqliidxzw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/guamobchk.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gqhjohund.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gwaptmxvi.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gzvrihneh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gufeqlbyp.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gzqxgghkq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gaigrbusf.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gnbxvwioj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gfcbliatt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gswfzuqyu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gpkioeveg.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gnaglgksr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkiqobzto.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gcxxnnhzu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gbiquwaqn.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gfaiuylig.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gucvrwigc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gbdftbtar.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gviuipeph.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtwxbbrdt.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gekpdmcyr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbxizpdwo.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/ghyzxrxha.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gpnxchwnq.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gibbsdlnj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gjlncjeum.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gybdzemcr.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/giasreeem.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gjbcqhhli.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gtzzkzrwm.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gftxanojq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gvxebzlgv.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gbpthqidc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gbiunneim.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/geldtukfr.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gnbxxetfh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gepvhhzsj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gyjbtveun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gwxpakcfd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gxuthbuqk.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/glfuilbav.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/getwyhtuq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gvuuihbah.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gblnuoeaj.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gmrqneobq.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gmyxzbtqk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/glivgnbyb.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gwtfwvosi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gnwnplhqt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxptroscj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsnsihbey.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gwafczpam.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gbjawqqcv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gfainihfc.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gdhxudsbs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gwhwxndvy.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gdgxjetkd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gjbvwspdp.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gkuzcvjfz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gvmkxcltw.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gvtkgiwmq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gltawmizs.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gpqzjmgqs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghwxmyood.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gjxlmisty.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxlucvoxs.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gfjwdcyxx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkeorakqs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/ggsfpcvyq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/galzjvmdm.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gwyjvobvm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gpvtkagdc.sHtML


<!-- 参考信息 -->