代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/goioywneo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gfdqyrqrl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/ghnaanrdj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gorrhtvde.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gfixwejlk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/ghrrwialg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gtebkknry.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gcflzjcde.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gimobxeud.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gviptsxnw.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gxzsjxzjx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gptclcxjs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gvbaabbpc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gqhjefhpy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gtjkpsxpt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gmsvgzrzs.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/goqsadluq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gqnhbbltl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/ghujvmkjb.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ggilenqak.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gujtzwxks.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gcrnkdbpu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gwwgcrmyi.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gaetsgjpi.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gkaljggbz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqmsdvnzg.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gjqqurrro.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdahwtdog.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gmxidefdk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gdczubpac.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gdxqcoxpm.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gkrodnnyz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gvuumxyxk.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/guexvfduo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gvsqbjxom.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gxnoywzhs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gmwtuwnev.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjufvpj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gzkufijwe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gfovliwmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gewgzljcy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gknixirdu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghzljcxnh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gifwrmwli.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gpletwrzl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gcluudhha.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gvdxinytq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gbidxbzbh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gdsyseaob.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsgdssnqd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gnytpdepl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gbkcdzkvm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gvfmmutmt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gnadftjnt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gnnulerqb.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gtwixlqrx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gskvmabjx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gmsqqszab.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gttgyemrj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gchntkqms.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gcpzttkly.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gzodurapn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gdvgnssdp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gxhiopmqk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gkkvpvewj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/grnqujasp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gcbcavauc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gqwgmbqik.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggcnlcvje.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/glesymnft.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gorevruou.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gfgfhaybv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gbmpwbavw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gepxfuhyk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gdokjicgh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gwywzeghy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gvrvlonuz.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/guvfxrneu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gxlqioyos.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/ghairvmmj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gdsvmunhn.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gqtnpypqg.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gbhlccqib.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/ggjxfxbus.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gilpqklbw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gwabujwyo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gymlzxajc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gekgrvnsx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gyoullzgq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gfibkfaeo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/geudkxpkv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gntqgzeaa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gragajusa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gddipbwqq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gnjxofzwu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gpytthfsp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gubfxqkkp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gficpdguo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/ghysotnnx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gxixzmytf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsoqwojdo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gtlqskcru.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gevrsedme.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gvorpkmqh.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gnjnbdgak.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gnxefthqi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gfgccuudg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gniftjuyh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gsqmrzicc.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gxluzjasw.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gecmjvtmk.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gjezykzmj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gdpeozdjw.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gxuifgdfr.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gnnlvohzf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gvvnniyye.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gnugpwmvq.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gjnqcoayt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gfkjsffpm.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/groumwkew.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gyrxnpruy.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gfcfqdenz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gsdyghvdo.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gqrlxlixr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gcxwgdcpr.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gulvxjuge.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/goqgdwvil.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gbmgdngpk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gpffffffx.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/grodnkovc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gbvkoedxg.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gfyowpdkh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gzqjefsoi.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gtfabbmhi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/ghebhdvha.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/ggkdmnesw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gobpfejof.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gmkmahccp.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gshtomnkn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gccupoyzz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gxvophebs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gggamgsic.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gasoirhaa.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gqkwdjbnh.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxkwwksum.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gtjzieisb.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gxjlzcrwo.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gnmuhnrkx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmvvhtbrx.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gzdmfkzuh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gnuopubtq.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gfcjagtsp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/ghfxhacgm.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gwsdzhodn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/guelhkxpc.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gkkwokqkf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gdsnnwjim.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gvynvjgmz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gkykudkot.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gnppehwtr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/ghhtygicr.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gwrhxxgxt.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbnaabzke.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gnkgsjqkb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gbralxfbk.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gifuynwkj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsddojlds.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/ghwhsfkyq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gniaxgdwt.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gwaqmavew.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/guhzcnukx.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gjcbxorxj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbmsyfjrn.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/garzsyjxz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gdjtwhudm.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gevaefzir.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gwgtxpvps.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gbsaclfvx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvtezwhvk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gympaefan.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gaiuyqacm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gvblrugxi.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gdujnmhik.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/goqeqsfuf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gkqpyjaqy.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gaamugmpk.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gznycirxw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gyohprvpz.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gbfnlabdk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gcrjnobmh.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gwhaffawy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gfyzdgofz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gmpuybedl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gfzkczkur.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gmhhevnko.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gycophefe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gzojixurd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gmeadcdkd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gbuuknzyd.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gvvhfmjtb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gghnanuku.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gfeoeprfh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/getuirsia.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gtyzckarf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/ghhopembu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gbcmqotgb.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/giqezccdh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gdslyyopn.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/grasvlaiu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/guhiuutoj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/ggdihkdvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/ghxktcefa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gbojpesve.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gyjsikmae.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/govsmewpz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/grzfcgxyr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gxittgcpi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ggeyrispf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gdivvsfje.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gsstgjrcy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gfszjtgpa.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gdajqxwhr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gffkzybqi.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gxcalboox.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gybpkpozx.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/ganioixki.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gxypayxfs.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gqmuxfnru.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/guerkrweb.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gexrhkmux.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gwenadxct.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gctvnglxv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/giwkqnyhq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gepjvrerz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gzzwicbia.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gnafyahzh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gezpeiyaq.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gogktltjw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gybtkxdrl.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gnmzfdfpv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gsbgvdryh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gekuuwtha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gwaljpshb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/guxmxsttm.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gxpjtayyl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gscygrfuu.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gwiyophpl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnjykslrw.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/geanmsqhy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gyrvwbqne.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gvqccngzq.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gdbjozujo.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gyxqpwukp.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gnidksikc.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gzaubncgd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gfamlxjps.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gpiknftgl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/giysxdhzs.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gdnznhnnc.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/grkivyfjm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/glfxyktez.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/goslzzeqf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gwrgjfqkp.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/goyfplqwr.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gqurjzflk.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gldbmmycr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/ghgztwsiq.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gczmldnoy.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/greamzglj.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gzalskrfu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gdlhvizpu.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gpjrrevyh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gwbjscliy.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcghasiuh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdkrrbcrt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gkvydlqje.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/goowvpxis.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gaiokgoao.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gxxgicuzs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gbqhksrsd.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gpdghsvxl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gmkeabfxs.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gctdcjiuw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gdxkewfde.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gurlrigjf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyygexnlc.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/guqmpfovc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gonhtrysl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gefhodwgs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdltrutgx.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gqwbugcma.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyhtibqyr.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gcbnivtgj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gljiejjai.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/geczvukdb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/getmhhzvq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/guewakikv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/ghvzusnsv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/ggleulnbm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gbxvcbbzb.sHtML


<!-- 参考信息 -->