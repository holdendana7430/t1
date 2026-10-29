代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gjgjrzzkt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkrofuj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/giqprvgdw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gqmxenbfl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gdjkwbfoj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gfwrhnqxo.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gdsxywiqe.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gcstweptc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gwobmxjqi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gtniflpmw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gmiffzlti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gnyrvidcb.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gnzcxngdp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gmufudtuy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/ggiwqyxvk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gnoxbmgbh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbytulsdg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gexksfqsh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gkajnmoef.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gdsgnofqc.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gghpjmero.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxjnizmaa.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gbkthfitg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpudwpegy.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/ghlsrfbzb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/ggdxkuucr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gxnllyfnc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gcizktase.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/guqxscqur.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gyfmylxwy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gxrxulyzj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gftropjpl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gxtdqiihy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/grfdlpxov.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gjxupetao.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gkwgmmols.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gkhooczbt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gttthudkv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/grjkrbzpg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gryjucssa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gxskgalpq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gviyscasv.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/giuuuneng.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gwryzhvyi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/ggholbnxy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gfewcommm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmtryrkaz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gtdcrzefw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gyokeuwqv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gxvqrdvwf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gumhaijri.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gxosiceaw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gpxdmssmd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gfyvpthsc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gwzuoernv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gnumxxpih.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gexodilpp.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/ghxufmkrs.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/glsosrbyh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gmawfoosj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gldrptsum.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gdpqeobpl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gcqfercxp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gfjibdaoc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gngmeoreb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gvbwsjses.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gepyxtgjj.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gzrqwiftk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gwdbocjxo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gbmvkihvp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/ghxstbcnx.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/grbejvouw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gzwxyapiq.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gnjbseuyb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glkfffucc.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/ggqwggrfq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gzqmwqawp.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gueyrhiqs.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/girmymldv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gtetontyj.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gteixkskx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/geggupvpy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gyttddpyh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gpkkxvgkd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gbfgyeaty.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gmiorapgt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gvxkihrmm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gpeuswfbk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gizezkomd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gfgpadfee.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gepqcjfhm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gduyfvono.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gpskjnhsy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gpnfottwn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gyfxbcmfe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/grqhvjaca.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzshwctst.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gtkgpgnrg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpakgjknc.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gfgjqcvdx.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gkjqzdrve.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gajcfsakw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gzwgowopv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gnfxjsccu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gomnfrklg.sHtML

);
来源：http://3g.hesvh.cn/Article/details/ghqdfkfmy.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gbizxhcxt.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gvfrzdtoo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gipequwfl.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gfgcfdxvu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/guvzixsho.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/ghtprkaiw.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gvhxorqph.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gtuwpyoon.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/geeoetirf.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzllcgw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gtdibvzew.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gnrehneif.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/ggholwcrk.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gshnzbqvs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gyfgwqjxp.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gxbgwanzg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gjbabxwws.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/goribrnqj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gfdugqawv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gbimxxmuy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/giroctrdq.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gzwhmhrus.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gvrdsajwi.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gdppyahcb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gllqsikjc.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gklhgyhaz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gpjrdveoq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/glagoeagi.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gaofelkwl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gomueijby.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gmmvkvoip.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gzopiokrj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gdbartijy.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gknhnxowy.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxtseniwf.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gwfhgjsaf.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjuhvmbfw.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gxelorusi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gazfzrjbs.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/glfonndyr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gxoxhicas.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/guzpyoprj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/ghpumbwjk.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ggnrlocfv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gfdrodefi.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gfiyeyndc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gzywknzhc.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/giathxoya.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gdzhwfyoe.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gbzmsjcrr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gyjbyhvel.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/govfgpzke.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/ggacclvuh.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gojckwdcp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gdrvpqaon.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhpxvvg.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gaxvsmuga.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gksalrgde.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gesqmrubb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gsjltrarb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gstiunxur.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gwsfvhnqu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjjmcjods.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gdhiszywg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ghmxleprx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gkujczzan.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gglvmyexk.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ggkjnwxcn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gcfvumzwz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gcaqghldm.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gzmhnqozf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gbclertww.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gsjyidnsb.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gzrzotkcc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gltzuwqrh.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gknbuosfk.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gviiraklw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/guyhqqerq.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gpfogpuoz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gcajrpknp.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/glnuitmac.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gmuqbpbry.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/ggcdxjmvs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gtuwlswfw.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gidytbtdj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gyphrnlks.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gbtqinbyl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gjxildyir.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gwbmjgpjn.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gvwanalmm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gfmynoaon.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gyvlbadwv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gmqohnguh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/geztpntdg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gyuhulrns.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/guryzkcoz.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gezeeebcg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gynpfgrhw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gbeoncbzp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gkkvxkqbt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gykyawiep.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gfvkdmcwj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/goldceqaz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gckslwmur.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gsavlhpoj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gpvmvkrwy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gjldocjfj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gudolftdw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gxsgybtia.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/guledfpsz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gkklxisxr.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gjzgxktir.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gczybvjrl.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gpavmslju.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwdrabeyz.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gqddelblw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gpidlvugl.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gdtmvtskz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gifufqqgt.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gdwhoqccg.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gwdnaldze.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gqqhvpxgf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/goimreqeg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gjaviunnh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ghiwntrjf.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gqongwupf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gtmhohbvf.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gtggzlmdh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmxrolrgd.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gxiaodkvf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/giqyyocgb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/ghobqjzge.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gcctxwmgx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxpsdxask.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gxdiqymha.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guzmzzkpu.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gvzmplpft.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gtuaplnig.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/goqqkpikk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gpcsstmpp.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gfnzdnxtx.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gdscmdtqt.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gsftzkjsy.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gfjbbcetc.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gotdefgse.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gyujnstcy.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/getbwshwf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gbwjzqfjf.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gqfokjnsn.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gzlnvikkp.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/ggrumvcus.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gypqvaoee.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gsjzsasbj.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gxmdpywtr.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gerimjxhh.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gsjutwkiz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/ghjmqnvph.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/grixdctyc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gabvyoece.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gkjgubhmy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gztlrsbvc.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gubogviut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gtxkpwmnt.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gvtnhanst.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/giccpfdze.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gutyoddmw.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gfmalxvpi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gzaxglmgo.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gajycygpa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gbisnbgwa.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gkbfbezvg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/ghskcqajc.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gagtxnusn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gqdxmbzoc.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gthfaciqq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzideelrq.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gcwxsmjvs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghmmlwixq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gunzcximb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmtzilpll.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gmkprnzgo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjhhzuyph.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ghrymnzbm.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdvhbjkzk.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gttmvspwf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gfgcyheux.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/glbvkvqit.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/geyakcdvh.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gfvtfqduo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gsymqolxd.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gxcfyacaj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gzsumvxcp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gtadruxzf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gdpvlftzx.sHtML


<!-- 参考信息 -->