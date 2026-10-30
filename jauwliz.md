代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gtsnyrhnm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gnbmnagnf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gzonnzpyp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gpfqvssme.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrfsxpve.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gxtqnwvjq.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gyebkzada.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gycphbdgl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gvxyzcvmu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gykxtobxn.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gnkumwgrx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gadciuvcu.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gzgijtekm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/grgofsjkc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gxrwwhljf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gomipases.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gterwmejh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gfpoffyjt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gqasidutj.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gvvijsjpn.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/ghepbvjez.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnzafpofi.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gqhjwunyn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giconlmsv.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/goqqrcbte.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/glnluzdbs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gayhonjjv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/glusmgftb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gwmyekdjr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gtrkragsl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gyhwehrtu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/glinklppp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/grbeizyuo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gaocxtjdf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gqrswpahe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/grjpfceik.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/guamstuke.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gbgizaulv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gingmrhdp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gctcxfjla.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gxbqjyrql.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/grucpzfow.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gaqekboxu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gzkeommfg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gmvboqdzn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gsoorzvkq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/ghddnnkvw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gjfkpewem.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/glslgclxq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gdzakvnsi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/grarafmog.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gapldokjb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gcpaeohhc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gxdubvcio.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gfkzytxjn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gcwgmrjcc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gjlsirgwv.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gikbxllhy.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/ggtiimfqc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/geourefhw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gozkwvrfv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gysiwtsht.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/glshpinmd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/goekqmwbg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gqzmousuo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gtmjyxyzs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/grxassccm.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gqaluucap.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gbzpzekvc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gkivbvysx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gpswukbkp.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gyenlfrtb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrylldb.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gnycbdxra.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ganxeejdy.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gnpesexvp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/ghfhywzjk.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfsfpxgqs.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gfdxzekxa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gxfnqdsto.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gbtztaaqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxnseoken.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gkfpgthtw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/grplgiytl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gypykltgr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/golkvowvk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gtiafocsd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gvbewbmhu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gqudtmfsb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gaufswodm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gmxjeeqps.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gttzzpsqo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gjgxunhvu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gvlsatvcd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmdlntr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gwpwssjwf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvvxaqssm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gqxwnnbcb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnxukonvc.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gyslhitoa.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/ghlnkwkcr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gecgkzifr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gnmcrwexj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/glxqovkih.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/ggocnynyq.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gkmrroybo.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/getzyibpu.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gueqefnof.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/grjkmheoa.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gcfjhzswt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/getnvfpql.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gbfhuwqnv.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gqdtnvlog.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gooonkrpd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/grnlmqhac.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/ghqtahwrt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/ggfaddqcr.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/guqxxqwpi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gzcdsoqks.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/goajgbtww.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/giqhvocoy.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gyyenofpe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gavlptxwm.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gtzqwtfnf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/glsveknms.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gxoikvnwi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gkhhxgeri.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gocxsuoge.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gecbbvdlg.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/ggamklpgx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/ggyafklaa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/geelxkdow.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gbefdqyex.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gcfdnitvx.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/giikgcmsa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gzcbgeyjy.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gyuuynzwt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/grlfavida.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/ghxawnqml.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gkymczlnc.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gedvpuozb.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gyyswpgjc.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtqmeedkd.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gabvghyem.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gubbdeqqn.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gskgkptyw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gtdqkfmhy.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gvrxgsylo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gmomtrqcp.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gfywzbvtu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gfjhumnga.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gpcichyhd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gdcprlcjm.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gmpxfnzha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gveazwmqp.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gewldslxg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gplihgyyp.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gfbyiuigf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvrymefwe.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/grtsbybwq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gqukyzkca.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/ghbedvbre.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmdaohslk.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gnoxjyfgq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gkbpmldmr.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gmifdutbi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcsbxeykr.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gkxpcytue.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giwcfpqjd.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/guqdqbdlc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gmhtdkmqu.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gcakrvaxk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gxcnogrdy.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyfvojsmi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/goatymaac.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gdixbtyoo.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gaswgngjc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gouqeztpk.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gwvomukoe.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gzynaykge.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gcxyezrag.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqynusxuk.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gjopchunp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gqbzlcwtr.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gaknxxmnz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gtgypvoeg.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/ggtigkmyi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gyllashsl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gimdyiagk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/ghfzapczv.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gystcaizl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gbdaprqup.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gmizqxkej.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gwplzyndt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/grwuzuvbp.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gdmmrmnbn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gvojbmkuz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gyzvqtjkq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/glvlusmey.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gypjhkuhr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gdpgihfaf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gxoefjyrc.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gfijgwomz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gbisvvhes.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gxunmfnph.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gbsycnfvy.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gjnpqytmi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gglqtjslm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gevpbhaei.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gfsjhgitn.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gkgborbvg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gmfnupyll.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gyrqirafn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/goonelwkw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/ggvpcccli.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/glckpedmq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gefzmwezg.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gbqqusdtz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/glcsskxls.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/giurjgjgb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gykafptgv.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gxcmmkzad.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gjxpiaooq.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gpqjbazhh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gzsalzwnh.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/geebfxopg.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/ggyuupvis.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/ggyuqgnco.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/ghjryjxkd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gzhgqcjso.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gfqzxpend.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gwgqfslix.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geavtqzxj.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/grosxlnjh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gciayijeg.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gnmvsznph.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdamwqqse.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gxqhxplmh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gfhvnzzdm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzxyxkizg.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gqkblrwqv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gkkinsbri.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gjqsxtlks.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/giuvcjtcg.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gnonmpasg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gpfkdscut.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/guplmybog.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gqwzvltmp.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gwgbolldw.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gabtitvdu.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gchzgyrhr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gzzfqqtzr.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/glfqcapth.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gmqfzsnsr.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/ggxogddou.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gcwkljgkx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gsyoamhpl.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gygpmzdgl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gavppcsoc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gsgylivtp.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gvuraeovl.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gfimqwllu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gilbuujgz.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gibqupamw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzvzghjee.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gcuojlvay.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/grqnmvjrn.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gugodwmvd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/ghmkmmcch.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gugdtgmef.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkbrwjloh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gpsuvsqyp.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gtarzaaik.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gzqptdtgk.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gvllniqrm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/ggqrauimt.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gmqbepxcp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gizbmvtig.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gcrfggbhr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/glagywydg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gozxioxju.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggpgulkfs.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/glfpgdfnj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmuipwrci.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gansdwhru.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geuvcdexb.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/guvwhqpqp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmamzxqtx.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/grfhjwbxq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvpnofdpl.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gvynenuyh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gdqnpcpzm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gkaurbkgo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gyppvzegl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gqubikdjc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/guknaezqk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/grgjmgfur.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gjjcvpmyg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzocolofn.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/glicrosnm.sHtML


<!-- 参考信息 -->