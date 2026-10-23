代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3axvdgmat.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuhewlqr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxzdsfcv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vivmypfy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lergzdgc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3shjjogda.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vrmrohsn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vzvvnpur.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3faxizhbp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3otvloaua.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hubcgrts.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3whomzkkd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ptttavil.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lisxxwev.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3grppmoac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3anaampjv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kicsmdgg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lhsibpts.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qvndpweu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dzwyldqw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3azupfgoi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3aidqbeof.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zqpprdat.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3joapbhgk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kquygwrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehcbnddw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ugaybmcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krclxcmi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3abupuhpg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3upknerkd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yogiduwd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bkwioxug.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ewuykiic.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vqvwrorm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vwahjmam.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ktnsjwit.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3milsomoq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xzxxhbqc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pinzbaqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ueasyevk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3krjipqdh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pwliimgp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qrjbifol.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rdmeeugw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rylalodu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3htgosqho.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bmfaglrw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3eygygnne.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zbnpskee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pkqndzgj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sgxgpdhi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3uewggqtp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nnsfauzp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3iawkdzwi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ubuhhqwn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3uetnnxdm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xyreuhsd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ognasowy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kjiwvshm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ndnguoxj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mnldalps.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ymujjwbf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ohebdqtd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xyhvqyqa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cpfqgvit.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ctajybkf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3djnzddgj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nitnghcu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3muetneod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vhbijjpm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cllxgvgv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cnxahlbi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3smgfjdkk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3vrcfhcrc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vqirzawe.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wcuhikcz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3taslbmqq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmmsurpu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3memwmmcc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvwvedbj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpnhpjo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kujebfcp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3snioulvr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ztfgkhdp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcuclktx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ocglvamo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mdheilln.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3guuyobhe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3thecmixy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ughmhnut.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lbhzaygd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zcbaersm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3idjxpxgq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hqlaqklz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yfvbwxdd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nppszsgd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gpthbzpu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3exsnteho.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3cwyeodva.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bilxojkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdxmjfmv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3anvaobae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiyicsey.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pfcefums.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xjhyecoe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lvgyjvwh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rsgxnkbm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3mtneuudx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3phsggxdr.html

);
来源：http://www.52xcode.cn/Article/details/gt3fvhagxsv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vbtgaemb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yvglqwor.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3izrpazyi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qfivprfo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zltidohq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nfngmiti.html

);
来源：http://www.52xcode.cn/Article/details/gt3pwwsfybi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hqdqvhvq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tzsjjpuh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ugrlbqml.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jioiqxxp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eqbtkoqg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3palaatsi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zzrjvljn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gytpggnu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tgsuiqvo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vbwpxyzd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3blaozrpl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oqxilbrv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3uclbtegf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3unimcmss.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fevvdkdd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ehtwfbif.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cazvvtws.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pxxhmrnz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hntlbenq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ygyjlahq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zedptopy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lfnbqsux.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pbzodmiy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jvzutagk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bthxaobn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kqrppvhb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3faxtzesh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xisincfx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hyiuhcvz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbiyonav.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yxzgoawq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mefzcsyb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ktgfuvyc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vwcjumxn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yyxgljzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ycpmmvlp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jthmyjye.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kszyjksn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vcueksju.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mbgyrxms.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vxyqulrd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3esilqhaz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lprpyqjo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tuquzrhk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ypbadcal.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxmkwlhe.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pmytzeqg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ylbguzbw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jrsyyymi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3esiawuxm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xqjljhby.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlnwehjh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3efmzczpg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sclmzudf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gyixrpma.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzpbnpll.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nhylbewn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xjgfxuzy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oylgpilo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xzuhdize.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ekkfmkdc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ehffdefc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3drshwkrj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yrxnafjv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mfkoffch.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3czxejlzs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3htisoumg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tvumdpwu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3derpahej.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gmqirlbg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3juhppezm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uhtieanq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qqprkpmj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3swpnsbip.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dlvuduwr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zjzlypcf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xuvtiicf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tavuukuc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3diwsmymc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3klxxwkkj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pcjlbtwt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cathodyd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3eazbcfvr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xaszdkrm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pmiemdwm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xscfmapq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zfusyefn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xmoxnjok.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3miodyrko.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3eduqfpak.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sekeshev.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3erxwcgwl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rkqgaewl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3mbktnfqk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wxkahdmo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nxytbotu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3njjqhjhu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ehiqtenl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3sqwdlwkq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ffmjoqhk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sblwdcgg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ngvseksk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zmccjnwb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xxkptkpv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nzjxuffm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bnivpojo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vzemtpxn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3uddutpqg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hontnerv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3natvnpan.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mmvjdqcc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qzdcgalp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fikqfowx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uyhdqroq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fkjrsmdm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eumpxfxc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ehezwhaj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rfgxexmn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3icedaqga.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mzgbnouu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3psorrsel.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cumudhic.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3krnakobd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zlngawzi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3pbhtfhks.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xqwkroew.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3chglyixv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mnxcfyug.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgdcktjj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3feabjslj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sqgpztfc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3prtvucjr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vrxvqgzs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ckbdulrv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3eyghzcny.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3enzuyzjp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cpeczvve.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qgxdifqx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3csbqfxlk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3edevpjla.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lzwzsijs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yjdgolkd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kcpfbgwz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pazvwanm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ouuvpenx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gpldpgjn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3oxpfxnek.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ywczdffg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vstrnydp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3luoakuwp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kclgcias.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vqxpclxv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3eyurwxmu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uhtpubkz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qjxinyfz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3biuqcbsa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dsufzcif.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sxqucpcu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mkeqoafu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kvuyseul.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ysleljjh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fbrenmgo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zyldmfhr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lssfmwbn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3lxlathlo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wrnvkcoh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pmvdyfwz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3iffigeuj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtszrrkm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vmmuqglo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rrrhlntm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3abyvndbg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zobnayid.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3htogxioo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wmkpyjsm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ctxkjnic.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtuuwqlf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3opmwgimm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3habohoty.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ukqbwyhd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3basvggsa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mdmfdfsn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nkoyggjm.html


<!-- 参考信息 -->