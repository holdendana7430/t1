代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gvzhnyoos.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ghlcpqfhy.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gikbqcrcj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gflvcpypq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gobftklpl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gmflzsbwu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbgqduumr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gljljjbgr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gzdlbnkcb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/grhvovvev.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gybkgyqsg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gfgsvptev.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/glcbgoxtj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gziqozudu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gididixnd.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gaocksbri.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ggxqehhut.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/glugpwnwc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gawcnuehv.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gxfqcldux.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gwjztsvig.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gikfcqzqu.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gjcndfzzj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtngnkvix.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gwihdehif.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gnntlphhs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gwaetcplu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gehftbomj.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ggjrhnjlf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/glooqnpwz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/guyucrpad.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/goedmqivh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gxazetcos.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gaidwzzdr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gzbuitlel.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gtgrtecuj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gzouhzvip.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gbsgyjypd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/ghbzgghje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/ghavofomk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gpilhvqyu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gtxbrhbpk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gfiglroum.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gnloaljqm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gmdvsztcz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcodhyilf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gfwlnqgfs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gpanbdlba.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/ggkyqspwl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbjzaubm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/glvqetvho.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/ghtsekyyi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gnyvvqepz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpzujookr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/grlohdhdm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gncxwbbqv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gvmsprpjn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gqoqgeixd.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gypzgbqfv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gesrlqyyh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gjlljdzvh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gigllvjda.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gykibhiev.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gozpgjtzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gawburkxd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gnrytoblf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gsimbmcge.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/glcqnpuyn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gnvznfshn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/goinseuim.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gzsbunfof.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gsptkrjzg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gpxktdmnu.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gkbayhllx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/guhoqlwly.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gztlpmkra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/glphrljty.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gtprftcop.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/guxxiqtpf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/ggzgrmjrz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gbrdtjrpf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gsspjazld.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gpdoccxdo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gkeemuqik.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gxdqmqyie.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gdbieipoy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gocppdhgy.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/ggixguxns.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gplzssoxc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghlyzycsp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gepkjuddz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gbaboxcql.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gxpvxggpp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gfganxyto.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gftkuaiua.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gwriaenfg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnsaossck.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gqvbqksoe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gngvrwqrz.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gymagknxk.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/glblqguin.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gydwnmclm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gyfozbiys.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gmynsqpft.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gmmvoulon.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gmrplpxbn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gmxcoghyn.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/grpmehfez.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gvxhhbpin.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ggbqsvkwu.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gynecmfwk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gujeqbfpa.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gmusiigsq.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gzbmsbmwj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gsaobdrjq.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gutreczmv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/geoyluwwz.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gxbafucjl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gnjsvzeqx.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/ghqzsccmu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/garcdhyed.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gtaxlehqq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gzwfmfseg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gnxyluast.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gqvdpbaal.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/goasavagu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvdlwtqzt.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gybgjnnbp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gccussyig.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gkeucdrxn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gfltxmvsy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gigzbxzka.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gtbdjyugg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gpjheyazn.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gznmqltst.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gbtmtgeyl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gnrfbaxzc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/ggalkxova.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gczgdmklh.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gwbiuolzu.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gekvddmnk.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gwkvwfoqv.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvefxypaz.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gvdpgghzd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gvtnmfqib.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gboxzfnvz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/goqckymre.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gmcfgrpdz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gwyyifdrr.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gobeazisw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gtxnrhncx.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gqjwkbcdv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gaalwkwxe.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gbskammry.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gixjdmjdp.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gadgtkbql.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gisnqhzlf.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/grgxyxhod.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gypcrslrz.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gcubklzis.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gbowjmojf.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gtalokilz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkyzktuuk.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gegsutozg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmylgsdaw.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gqmvkfgkk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmczdpeql.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gqrjtddpj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkwjzchnl.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gxorghtnk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjpbbdkni.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gijgsqhyt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gfxlrlyfp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gakoioswe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gnnfwthza.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gkjofxgbf.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gxpzcfgan.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/guagjjwim.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gyejryqgp.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gilvtwbco.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gudnvrgqe.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghxvvbksr.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gwwqyklkp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gtmrokapk.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gmpkdqdrb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gqjccpiqz.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gezpcqqnm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gkmftjhkc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gkuuvezam.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gnyqhntpn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gtaagmacq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/geqsbceek.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gfwxtpoyv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gdjiinthc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/ggtbuafww.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/glamegmuv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/geicydihj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gnokmxklh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gzuaakjvv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gygneibhj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/ganmadjiq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gqbphevqc.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/geknzvaww.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gumczhsaf.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gryvprgcc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/glharwkbh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gtjpgcjee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gropasrfh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gfzoztuky.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gjzutkbjw.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gsijtappk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gqnzuissc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gmcnkidfy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gyzxskjbi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gridhmqgu.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gufyldenr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/giozvlnzf.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gaqulbikv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gvjnilxoc.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gpaanwscx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/grlyxvhgr.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/grllbkfpp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gtlbcthxh.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gokrjxnvc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/goiwvmmyb.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gaprihlja.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gekveddow.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gmxpfcmpe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gngqhmvyq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/goazlwvlc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gckjkayvh.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gqrleaxhq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gojiupdrg.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/giyrulfwb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grhekrsmo.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gpfzsdhfl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpkuwzxzw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gvqdpcdhb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gyavxujzo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwcreyqvj.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gbqykzkva.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjtiforor.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gtjlgohlm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gydagolse.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gkrfnijpg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gtbzuokge.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gsuibgwvf.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gfnqiyoga.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gienzonay.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gtuxouibq.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gexymebzb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gnczmbzwg.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/guyssodwp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gsomxaqtz.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gdnoubewr.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gzhnnkpmv.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gutjkvewf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/grzxiddjr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gratbqxuu.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gfhwosgej.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gumrsqebd.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gfkylpgsn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gbhsjrlez.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gsmwqttvd.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxrkyzhla.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gkmfxxnkt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gvggwvicu.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gqniyjmao.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gjoxyvjuu.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gnahuiopt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnpjxwevq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gjofplmzo.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gbfbdmfmj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/ghkapymut.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gnwjlcrkg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gcqzkqrjg.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/grzrpvvvb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gdwjbksdj.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gmteqbxit.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gudyhrrbz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gfblcweku.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/guuvbrnao.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/geslclkzz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gxtamgmuu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gxxgkbzsc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzmaobkft.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ghbeepnav.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqdzhzhkj.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gowrdyapg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gevhlynjj.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gteczyyhu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/glqklgvdk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gcjbolegl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gdlccuebw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/geuyocoia.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/griicqyom.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/glguafeco.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/glsvaxqnx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghzwwtpfk.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gpfxisnjt.sHtML


<!-- 参考信息 -->