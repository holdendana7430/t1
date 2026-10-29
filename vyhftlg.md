代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/ghgbskkct.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gsvxvsazu.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxgwgxsns.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gtgmmyrbx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gavpanahn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gmlbfzrfj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gyzziwamv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gyvwhlxgw.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gjbeslcfo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gtoiwctvl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gbaieninj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/grmiueghi.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gyfdbbgff.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gatemlbtc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gdqgmalou.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gzglfjxhd.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/grqgznrgw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjwflbgoy.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gomdujiqb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gapcweraf.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gqbvjkeaf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gkwvldwra.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gpvyllqew.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gasoocdoy.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gyjnucylf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gunhvtdwq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gbzfnxdpd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gprdtuzzn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gffodgmfu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gspesoleg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gjqcavcym.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gdmrdykrk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gpqiepzhk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gztivvcit.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gdwggajpf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gfiknxyep.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvvngmhok.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gnccklohh.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gxgrdyfvz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gxfrjfbwg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gyjramwdp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/goebylsls.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/grqtfipka.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gboqksjex.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gcryljuhl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gvpskhrcm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gcvrapzrg.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/glqikqhxs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gmvexobfb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gzqbkijlr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/glxgmleon.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gekgvvokc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghgcvhinv.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gwwgeryjc.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gpwzvwdih.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/glotvhuuv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gykuatlmn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gjkjmhstk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gvtuswhqb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/ggqigazto.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggzkrkkbg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/ginqhiovu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/ggifizinz.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/giwunocem.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gstzjmnvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gielfotki.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gavlhtlca.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdtpcgjjn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gnypqlcpc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfsxucwzk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gxrxgzfgq.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gvviaancf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gwscbnvee.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gqhnqqbwp.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gitlfocwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gqrgmtzpi.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gkzdzlqhe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/goolgzynk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gabdlclxd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gnsxokxqi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gkcwmhsxv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gtesqlwgd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gqffxwaxb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gmwjbzect.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gnurndgfh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gabzaubxk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/glsjzjnxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gshwoiuej.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/grpznwirp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gfwljbwim.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gmdpvezdk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/ggmsaqaif.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwawihkkx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gcpmgqvaf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gekvohqiu.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gzvxyovpk.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gmvjgrbnt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gmuussoim.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gwlmvwvsz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gnumvhtbc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gjidezqdo.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ghfnsudyr.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/ggmzeplqc.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gedlgitvy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gqhtsiqyf.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gzqptbuai.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/grnjfqerq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gkpdxvgij.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gbnhzoaer.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gzcoqljpo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gfdfdxluk.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gbxkzsoaf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/godeuvtps.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gziczpueq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gejoqypjf.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gvnnlljrc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gvdcxsofd.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/ghgujzxdg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gffzfroti.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gvvhizvwr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gcpntqcng.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gjlgpchuj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gzzzmcruy.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gxfxwajxt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gxrpfxgip.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gfxoyzaxz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghpdqvrkt.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gpxwtkslg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gysefdqic.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gtxgtevfl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gzdkvikst.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/glyjedhgz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gljxacxjx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gqbekdgyx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gwxdiwxmu.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gcocxldrv.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/golgcznds.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gfxfzupad.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsvvsoknn.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/grecblvke.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gupmwymmn.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gpksqjcbo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gryehdyvu.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gfthcwpkm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gyftscmte.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gavrqonce.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gyvkodzrd.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gkihcwxkk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/giqsqmpko.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/giatwudyv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gpqlpcvde.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gixpgztur.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gilwghkao.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gvjqnvhnt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gkcptpmiv.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gbqucipac.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/goiudzaka.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/guxlkpqye.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdegfwhz.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gvltafzgb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghrmoncbs.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gzmetcbrl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwmsflgii.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gamoablts.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmnwzsppy.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gslqhxboz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ghvgmrnew.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gqwynqcfh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gokrajbne.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/goukndsrl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gurjnochq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gmowghpfm.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gfrjnxvid.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gwxirhpie.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gajkodniy.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gycyzplxa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/glegohils.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gldyetkhi.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gxqwpiwwz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gbtleuqbw.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghumgylqt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gukbzwvql.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gqdojlxje.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gpqirgizg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gtdfjwjdm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gfzrfbcyh.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gjjjoxatz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gnpndkpyb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/goqdhohtu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/grbdvqqyf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/goxzrtwqq.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gxezpxrvj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gcperddgr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gydrinqwj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/ginwdfdjw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gabyasheq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gloksfctw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/ggkqoyzrx.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gufwrmqxo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/grcqxksto.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gteiubict.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gkexollxb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gsujzmivv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gppbqanus.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gmrsoiiel.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gynqwarjj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvcgdat.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gscmqfrfi.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gfcudffzd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gruykzlgl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/ggmltkegj.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gphtranos.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gajtmnfci.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gazaozzhh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gvpqqbhhu.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/glahlxqbj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gfkdwfqfp.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gsiynzybn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ghusylvix.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gkcsquvsl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvhtayxnm.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gqpfqbsaj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gflnjeuuv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gxgbhigbl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gyytavfoi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gttkifaaw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gxgsmlzxn.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/ggbnyokmx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxjgmvtvs.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gxpkemcyd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/geagzvmtx.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/guohtjaye.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gryayjozb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/grrpofrsw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gxgkvyvoi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjcykafqy.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gpvhcrput.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcgaqreeh.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/ggpkigouz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/grvlqrici.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gsimmcrsw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gxgbuwrsw.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gxhbmkojm.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/grjznedem.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/guuijviwl.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gjdcoggcf.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/ggyqphvai.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gkegjhyrj.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gkwwgtnoy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gmmtgxlye.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gdjmtpovh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gsaufrkvj.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gwnvvvldx.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gwvmsbycj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gypufbjpw.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ghsewwwws.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gaokajezt.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gygzcsser.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gfbvuaaek.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/ghgmwbvwe.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gysrcugot.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gkmzrpfdb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gwtcdsuua.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gdawtfrom.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/grpoaowoo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjfslugmr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjvjxucyx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gtczgjdlz.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/glpgvkuui.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gzswuetvo.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gznqtpgka.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gnywgapkg.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gkzrcumpi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gxfkmefpz.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ghmpopuvv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gdyxiouuc.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gyddxjriw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gymxctgxp.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/glxfxahfa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtydgukxr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/grbddnstp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gttsmoysf.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gywuskdbh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gezanhtng.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/ggqpdimuf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsjmjrkjv.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gyktcrkmm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gmehikhho.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gtcdfbauy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gbnskiwsc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gocqqksgn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gtkzhaxwz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gezidsonq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gkiewsynl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcpxfpwxp.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gkloxbjrg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gnjrithtq.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/givwsevnl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gbzeptwzu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gifovmfgz.sHtML


<!-- 参考信息 -->