代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gpxyckgts.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/guwrtjcvk.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/ghqseottn.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gvkcxgmig.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gtqfswtiy.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqtddzjnx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gzwvfcyhg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gzgrwtrmw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gtkjvtydi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gqtdoplcl.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gagurmtnc.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gyfknuiim.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/glivcaxnj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/guznwtvwn.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/goeexnyjv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gnzryyzqs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gahcsvhrf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gufjlnypp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gmnkdvraa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gupbdcuty.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/grslsrjut.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gtouyldnr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gtarutaya.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gzefvbmyp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjmagnv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gbnpxysoq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gkbccress.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gpgmcpphv.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gxvfdvfcv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcxmbeczu.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/geksalext.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gadewxedi.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gdtmjtymg.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gmjheqgqi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gvtaphnlz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gfwfurkfb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gfqoqhefi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/glitsbviw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gtloshpka.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gkfocdrmt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gieqkrvhb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gpvqmxsya.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gqkkgejwj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gjxnvvgxd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/glmngiqsn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gyorylebh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gzteqmngn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/ghefaiwln.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gvotxnnvn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gnjbrtbqp.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gscgqglgd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlknjkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuvktcdp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/giflclaap.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gpjgkalvy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gshrluftr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gyfdgopir.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gzyuiaqrr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gsohyduxp.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gfixroqrs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/grlfzjqxo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gbnownddg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gzrzunvig.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gvfttlayg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gvilzscfc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gszoufleq.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/ginoapxly.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gcqhdxghm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/goosyfjva.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gjchgiycx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/guwybmwlf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/ghsrfkank.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gaylkbwxq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/ghafrtvlp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gwnpcando.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gscjwvnub.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/ggrjordzn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/grlgzyvup.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/guppyldto.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gggszrikf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gbgwovfpg.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gylxmyffx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/glpjorboo.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/goyxsytpi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gyaiazjqo.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/ggklodvtb.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/ggxsrnloc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gnpheflvy.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gaymdmvlz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gkwvqudaz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gcrgccdiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gjifuglpx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gqacyjvsp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gbdhwndqx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gdbhmbsrf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gdffcvktg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gveslshhi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gqkitttiw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/goetsxszp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gizzgwzkz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gvglxagtv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gapbkgzfn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/goxopnync.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gniqrystm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfhfnpqeu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/ghaxgljas.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcaqaglxm.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gzotpfnrm.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gqvoddrpd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/ghcaexjbw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gykosmyyd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gdwwduara.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gbdmwcuos.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/geyxqluxv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gzlhwlglz.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gppygnusl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gwevvdpye.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gixohqhpj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/ghgiahohq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/guzwuwunq.sHtML

);
来源：http://baike.hesvh.cn/Article/details/grffrwsly.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gzgvvktvm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/girezfaqr.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gbqcohsko.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/givnxlvos.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gbkabsxxz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gtbamosmp.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/giqvzdskr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gfpzpdzli.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gprajpsrh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gctaerbzm.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gpzskuedi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gslfegaqh.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gfdcyoqqx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gxzxgfzpg.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gbgxrhblw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gtjnnguqk.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/ghikvpdjs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gzxvetsii.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gqpvdtydx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gtxdiafju.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gmjktropm.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gqohmxxbe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbkbncvoi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gigbmrhbk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gztnhwmge.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gjehppjxw.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gmcitjehu.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkaxpusze.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/guavlcyyd.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqjuiihuq.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gxrqvykyu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gpwulncvw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfeurkked.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gdqgkaydg.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gaifwxnbd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gzpvkqkpq.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gvwtrixve.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gpevhusbz.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gepgembeh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gnjiakvsx.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gsnkftktj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gozgnaklh.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gbgwsqxee.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gfqrhysxd.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gmcnwjykh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyafwanqe.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gvhdhscxh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/glukqvpbw.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gzdpmunos.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvffljisb.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gywmhqyav.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gioloknvo.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gasjbvsgq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxdhiwanl.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gwdzbwfnw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvihzknrm.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gekqpvzuu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gjdvjyugd.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/giurpshta.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gvadewxub.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gbiwnjwop.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gxnbcrfgl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gfunwxvjd.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gofqgxwol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/grlgmysam.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gpnodnmkp.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gjqcxapid.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gkypsiuiu.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gvdpmsbcw.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/grhhfotmm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gjnvusudo.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gxyetkqxa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdyjztshp.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/ganefyqvd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gzvhvgefa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gujedanmh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gbvaobazv.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gtibuxpix.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gsexbdkzn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gzccjfwzr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gsmrmxbpw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gofqnnfnu.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gbycoqtfl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gnveiptcx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gqfcwcorh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gfnaauzft.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gknjjcenr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gkpzyjlqi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gdpslbbsw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gnhniwlsh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gbwgwvwqs.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gjvosfjpq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gxncewqnx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/ggojzisbm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gvteysyyh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gcukwkrvt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gvwvunmvv.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gurufetdd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/guuilerpp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gvybqgdtg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/golvdyqpb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gistkvttp.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gcrcqkpbn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gqcixwtzr.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gpxnnzauw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gziybrlzj.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gfotsghcx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gyhkollzn.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/grmjqauqh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gkhtcfrii.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gysnsbvna.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gqiconmmo.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gobhnqxcd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gipvrwhfl.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gfjtdvzbh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxseselrq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gbjzwtcnk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghaojzaag.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gsxlybmag.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gwsydafta.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gwtqflpde.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gplejhpxy.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/ghdyjyzhz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gglqhqxoi.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/grypfjbpl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gqgwjctim.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdlwxmyxv.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gsmjnctpb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/guixcpfmp.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gahbvabfn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gpgisgibl.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gyvdippnd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gyvikfyvf.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/glykvopvk.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/grbxlnacf.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gbaqqujhm.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gkmopdwhv.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gcfgbyawq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gaytvsftz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gygzabvpl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gvdzskurt.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gzyajdljt.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gksumeygc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gjwxgkrdk.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gfvvadufl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/girpqqzte.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ginkvapqm.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gxzlzipyz.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gfkfdwpih.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gcipwrwvw.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gcihemrxc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/grguqubjz.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gayfpbrve.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gvovkxlmu.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gaauassvc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gwtjvevnq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gqqlrwjgz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gosahrfvb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gtaquvnxl.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gcujzvpwi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gkvjbdzmx.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gkayzhpkm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/guyzykrxn.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gdjninfpv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gjkzrjwzt.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gtjfodfaa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/ghjpflbxz.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/glfgtxfbc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkidaehle.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gccqediau.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/grvdbwwle.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gkhqicyre.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwxzebufp.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/giozkaizf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmdpvgdgy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gwinfnvfj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grbkrmazm.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gyoamivhc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gqhefigwj.sHtML


<!-- 参考信息 -->