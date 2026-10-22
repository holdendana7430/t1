代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2geiwlnrk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qcteoafd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uldsrfjy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ryvevjgo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2awswcthz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2keqyaeet.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgswjef.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ozzvxfcw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zabbhezz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2nnmmyphl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tmlqgtlc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqyrduit.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2johiaubs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uydphvbo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dnllfxmj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2twvdghtk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2flbttuck.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hovizotx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lmjhwjhz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2hjpwgxxf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xdjodool.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfyrpmfg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2gfrrxxtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kovesccf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gyhnawqa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2thnqeipv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mboaveoi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ljqwipko.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kraoiarl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ucgtwwfm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zzpqgrew.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ebfrbime.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqpqqx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2igaurpce.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vhekmuow.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qtzuvpcf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yyllnlij.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ouwlhyog.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zptxkrzh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dcbukbmf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ecmdrtkh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2oclvghes.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2aucpcqoh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xxitjitx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zinniksc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxrjrpbx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bjmvnjfd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jfwwsapf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ithcwdjo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ggpjfaxm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fnokvvyo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvefbf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kpyntioh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2krxekani.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iwqqyvtc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ccfogjyj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cmohayde.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zasilqia.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ouizcvbl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ursjlzmb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2btjquvpa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ltkwzfcf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yryfqeju.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2blcpqclt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rxskohfg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2edhbvuma.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uqhcvkon.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zmqskvip.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2poekhctq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2illpnxdm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yhiytzjz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vakybjoa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ebiuxnan.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zabdosbv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pshttfpu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ormsexaf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ylpoxzuu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vjijvuuc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vcoxqrxg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2athblpdd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2yoefepcw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2guoomhzi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2corylets.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfbwceew.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kxomiwpj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mwvefgjf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dcbsvohm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2goiwuzal.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gslhgrfw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qczpzqoc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2spirkeuk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fulmqdfn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2htswotbn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xzkoqhpk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ibgjvayx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gwexuivh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sceiwxmv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ryzptvug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsyrikgq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2pqgchoqt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xgtmgcjk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2chsogybz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xbtagytl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ibvdyntq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vaknizzw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xpmjeevr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jaoxrovb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zdwidyjl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xjcdnolf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tqnxxlff.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bqzbmmnr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2kbapylyc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jopnbajl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ygwwlcxr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2racszkjq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dflbcbpt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tunymgdv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ktvjhiqh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ycbocdzu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vfsfskrl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vbgsgott.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kzefjkwf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ibxqpzby.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yzaytjwv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hdursycg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vvlpomnm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2epnadaxi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2eywpsryh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rcpppfzu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2peftecpz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gpdapwsa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2efrovdzm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ckqansbk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ibdtfsur.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2mewkfgxh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vwhkbzju.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jdnezlby.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2iogehgno.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wgrfogeq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2sejbntqn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nrerbgck.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hwsywfrw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xepsrfoc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hghjynai.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gojwxzbc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mercotud.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2danoczck.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2doehrlck.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2rxcexhir.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mbqelisf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cbttvyzk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kcqjkdij.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wvqcfkyq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2siogvckg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fhgrjcov.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gmuuppyi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2dvpylyuz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cjvmmzlp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbrkftat.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ydwdxeou.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lgbdufoo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jkudsqch.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rgodhkmh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2odmedpjx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chxdlmaz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rcoooolg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rdchyjwj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jalmslcg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovjzwqrn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rmxiwowt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lwxqzdtz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wslyrhkk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rvmjzqcn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2topywxow.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kiiaapab.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rdsheyti.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hpwhezec.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2syvoljdb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ritrjnhb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zzdmclpn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aikeyomv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xagjmcqv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yeyqyaae.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uphmtkkc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hzrmvgvx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iqucfsft.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yjjuwerd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vwffeegp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pijoydao.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2envalblr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ehysvxpc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2avjhpiub.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lrdwmztq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bedccpkg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cltcilec.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2uwpfvtiy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vpsnpwmx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2stakzxca.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fixzhzlu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fglwoovw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cwcsobrz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2idfmjhqy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vdxmnbel.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bxaieoqy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ltaauyvl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bblhfhrh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cdogkvum.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tjycfsph.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpmjdxtw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2omeafdvh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hcjkmhkt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mtlgowhd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cmhmuqsw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzjbkff.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xmspbitk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vqnylrvz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jwbeilwy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2flikkitm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mrgynwgc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gaoqtpcn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qkahcrwa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qqreubiw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kiwwqmve.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2djsyoebs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vjifnfvy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ywgqakjp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2tzgspolc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2scehtprc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gjeuezde.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xmvtotsc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mgeerksr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kuzpwqiv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vomrekyh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vzzfnwwy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nkxahhue.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2eetbgrvf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oidrryvt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2aoiurxqg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gqbbpiwl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2klhvxrac.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rhonhsnq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hbfljlrg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nsytyaop.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2intgizlu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tjsalduy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2adjsyvlx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2tyiqqtvu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wswgxfwd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2msouwaab.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2twcfopnb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tenzehnb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ekbdgecw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yrkltika.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fofostmt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zwtwomwx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2txjhyvde.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tduxdnli.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pvypjvps.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2dfoqutcw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2uwssjryi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2szlorygt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vwdzyzhk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xwlxlupd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ejvwaszi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzpzyymh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hlmalnvx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vyautzaq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2eeajxcso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dxiuarci.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eaifhcsw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hsmxgvij.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nrjfgaub.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pqljzxwc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tjhhirig.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uekpvwdo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dveaqsal.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kafwsukz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jfzdrwrb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vcdwwlbk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2izbljwbh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rxypemjb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vkipbbjc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbvxdpsn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgpjxjkw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lvomqvlx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2axkwkqav.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oabtprje.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xowumzqt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2whfhzjee.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tmbahjrx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2onvzhuxh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ipbcbuif.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mxbtxwum.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zlfcxctt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gsvyflff.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2eogwkpxz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xvsltbhy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jocrnvci.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uchzqtap.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tlhxgdkr.html


<!-- 参考信息 -->