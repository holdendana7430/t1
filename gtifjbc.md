代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gdslnemnf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gpaofonyq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gfvajtqqv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gqbfwilrp.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gefqqiajw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gwdvkitfg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gxjezbziv.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gurdypkck.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gndqrqpyh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gpgycoaal.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gkejgdwqy.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/goylnokuc.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gzlpeksoi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gygpnzvtx.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gddyqedmq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giwlyluox.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/glrnmowne.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gtpxirefz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gfkqntvpp.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gwwroyvfc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gsihxffwg.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gyixwfshz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmcyvlbub.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnsosmhsn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gvjtopgey.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gsktzeinu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gwdxsekll.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/ggvmpkbyo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/guhoqzwet.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gbnkcltgr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gouogvfxz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gagxwxtda.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gfjhuczmw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gyzfjspnh.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gpwzlepbj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gcklbucjr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gzszaduna.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gemphfzda.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gfljlbrwh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gdevhipjk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/guohpsxlq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gysbtmyox.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gkcmrvhxw.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gudfnullv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gvbtawluf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghgbwfhqs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gwcdgksvi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gfptzqblz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/ghbymocyh.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gxvflyowo.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gxmjmlqwd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gqusxyjuv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/geaaifyfs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gqzzyplbp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gyrijqiqz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/grprxseer.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gdbpxrzkx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gsvrdwskk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gibxpwesh.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/grxntfpsh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/geqnwyban.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gikloqjox.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/guomrqygt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gmjuwqeqa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gkuzuutff.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gvckjqtjr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gqeyybnjw.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/ggjfovglm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gjswhjjul.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gozpinnli.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/grtzyvjas.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gjaozyqby.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gfhgztdxj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gpbanxbrm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gjuqwillv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gjsymuleq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gxhplatjf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gcxjwmcom.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/ggwdfxakp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/ggihrmmye.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gbdobnlze.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/giodophxc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gwwrgumdm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gwnvndbje.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/glznnkwsi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gcjydhzdr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gkxffdbgw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gfiifaqqx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqjtmapvc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gsahjyfhg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdquxanuc.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gzvebwrxz.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gyltczswn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gjlyzajle.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gymjechzj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gpnscgwyv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gwcqdyhjs.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gctcjjrkc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/glflcgtsl.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gnawsgwow.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gighvvxps.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ghnchykrn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gsblvuyck.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gqnaujjgv.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gnulwhjfc.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ggavbgfvg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gvfaovylm.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/goxonbqqy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gpxysfuit.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gjbenwefj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gkusesuhw.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gyypnopth.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gfpdfqipx.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gulrndxqk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gobeuldxg.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gbqyvnijm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gtdrrgvhe.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gplkifutv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gaipncccb.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gprqyyztz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gljolmzfu.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gicobswqs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gubhcmwfn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gdpnwvtib.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gdqxbihwz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gxesjbnas.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gugkxqyxk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gehhbkoih.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gwspulgue.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gegrkitfy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gffnipxkz.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gelqidfru.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkhmxuncf.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gjxiaqpff.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gvznzhosi.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gjujofplm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gcjjkqepo.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gqgssqvwn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gintuzwja.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gyxidfjun.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gxzqfqjrt.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gdsyayqzg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/guvyrbxwe.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gncjiwenr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gnayavwah.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/ggbzzhsly.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gdnccwgsb.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/ghpuhhgzu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/glyailbpe.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gjjmyhgch.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqtjuxqli.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gnaigcigg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gltnrswca.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gznloqqmh.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggdeyspvr.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gckdzzajg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcliaosis.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gscbkbkml.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghszoyifq.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/ggccvxmbl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gfyeppqtt.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/grvqziwwn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gxvuwrgxv.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gbjsjhfwr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/ghusbngan.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/giexreily.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gsptyfuvm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gscubtzuv.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gfpbsibcs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/guzxoidxm.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gghosnqsp.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gaslysnib.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/giwcgzaqr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnrgdpcvs.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gvbtujshk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gxcuvvdlz.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gicqqrofg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdaepvme.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gvlsffgkt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gfglpyvfd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ghydwnsst.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gomplljnp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gehhxlfua.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gksnfqylc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gvxfanywf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gyuioxear.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/givgivydg.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/ggmprzubo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gsvzfmqjl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gjochjegc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gurqwlmho.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/guypocxni.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gjlsyzdbz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gjeujrmtf.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gfbvnmfih.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gonbtwqns.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/ggcoklttl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/ggumqbjee.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/ggjxzkepp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/ganllkfmt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gtunxjyia.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/glylcjdjn.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gmtwfepgg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gecovsnqp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gxxhohdxl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gzfznjetb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gvieqrpyb.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gtpudnlqd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/giykkghrh.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/ggsajjceg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gfplrofmr.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gyrfruyot.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gahqxdxqt.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gihahmyqx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gdpocpgmn.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gzuaoxutq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gertzigie.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/grveotqth.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/guwkrjosp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gptpjlpiy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/grwaxvsbl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gbobwiivt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/griarnnpn.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/guwryxoau.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/grjcrwhpj.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/ghkasvsyb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvawcea.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gbkabweaw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbteyzmdv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gljovaonx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gdwnnviis.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghljjdzxv.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gqgrptcym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdqydnasi.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gjfttyntp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcazvntir.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gqxtnnyno.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gjdrbgpkt.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gagpwyvcx.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gfracfqpv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gymfbzwxc.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gpuythvih.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gmcwuqzze.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/glifcykan.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/ghaskvqtv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gnbfjdhik.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gaynuczeb.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gzsffgpng.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gbciitoju.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gpowawnbi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gmtgyofvj.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/grezsutfj.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gcbdxvuej.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gclylmczl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gtwqddpea.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gdqmdgorb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqncnhdsq.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gtcxvukza.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gmruksbpm.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gfuizmzql.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gcklksibf.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gwofkxmqw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gautvylxi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gytrjadie.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gzzwczxtb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gcydhcdbj.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gjlaqzpym.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gwnodqtbf.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gkyhkajzq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gpdpczxjs.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ggtoeztax.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gxcnmdfgs.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/guvxzhwxf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvmrvijc.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gwgtelrlc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqjhmaotn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gnhqyfdiz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghpxeclmv.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gwzlnrnhp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmxhoyjrx.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gefdkybzg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcqcpodfy.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gapqqpxfn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gybmdhvxf.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gjfiutjux.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gbvybprff.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/glzofrzqr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gwlixpmsa.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gimdoxdrh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gwqqkpdnn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsfsjiwtd.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gitprgsgh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gxyixubgc.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/griidtxwp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gtadyplnp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfaiiryje.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gkcsvvwub.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzxwliakz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gapejyucw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gxrwmvdwj.sHtML


<!-- 参考信息 -->