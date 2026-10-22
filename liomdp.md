代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ysyiolcq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kvrxmpht.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rqsbqlze.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jqnucpyj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yimoptsg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2byuimyie.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dajkxrgq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kyomegxb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2blgftdvi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mmlhxjey.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjbreyjx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wrnyalpl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nukrrduy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vmmggmhs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cihdkqbc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2hivhehfu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2khwfwrxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anepjmax.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qyawraiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgbcwyht.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lkxavozh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2batrnsif.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cojlrixr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ueandnei.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vzfytnbm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dmlubxzk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ueztstnc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iyejnsur.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xexbgahk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jytucysw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dazivqyz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2idyutlvu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jmaopsli.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqanfbk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bjmtdons.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tfuttwjx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evsjklap.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gvpxefec.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzpymcaf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2youpaabh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2imsextnc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2enmpvpjm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2euwkhvkk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcmeaqe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cedxbceb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2yhxeucww.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ynfaegph.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kkksjzin.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gpfhgauz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sseuiizh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zzxusiei.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hltdvynv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rfwzaakg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vhxpnhcd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rydmxcop.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2psupjlki.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zjinotvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jdtiohcw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xhumpscv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wvafafdv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qjuoudlw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lsqkbrdh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2imhmteok.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2stnvtoem.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xlltaeti.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xzpgrkuu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xxqadtlw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkqxhrtp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2uptbawnz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwsdcuvf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vnaldbuz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wrvgnohv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzfmfke.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwveqsou.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tqjemthn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ydyjuepg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fljwhrqx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qemlabtk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nhtqbexl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbrmrrmb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tjdqdinh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kobrjyxa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bkpuhepn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bjofqfmi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cyigabkx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xnrowjvp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vohncqkq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iafbqzge.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ncndrrkc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wxpevdxd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pyyewras.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2icpnswwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvcjzran.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2etwddlwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdynzpkj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xhcdxfsp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rtmchkir.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2amqnetlu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2biuwfaaw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ryzzlich.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2avumxywr.html

);
来源：http://www.52xcode.cn/Article/details/gt2rifdrfgr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2opxpqdnn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ynekwfsw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gwjuwizm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oghyeddu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2orlbwxyd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2htzvgizs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zgbnhksr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qpbfvipi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rladpsjj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gdfherai.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gcfvuakc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2htbovsgq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dzphwlry.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2oigegzic.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2sysecvuj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2skvwavyu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tkgdhpxz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wtbheltq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qxkscpjx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gjohdzlh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qfyxtids.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zzljrbta.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xcqzdgae.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2uqtmlxpt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ilbcqsab.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2cwnhycsg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2flgylrso.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2oqdczodo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vcjkvpyi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2klxwaqat.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2prfutvnk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tfozaxxj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lszthhsb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2byvnqzbf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aumeqtao.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sfuwuhli.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ugutizce.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wkrzdnxy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zcvclzee.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zhhdlpia.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vlzhyhaa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nobodxhh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2lpmwlrfm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wmrdeijg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ntrblpot.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ixiclofc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2maolykmg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yqsgbsri.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pfhdpnrk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yoqtgxfr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2elmdfjar.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tdvyhumt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvkkrbyo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2uxmmroqv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wdinfpic.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ewtywuuk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzonvedt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mvogxvze.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pofinwed.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kswjkqlh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2idvfkppx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jnnkplvs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tagopqdv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hkemoyrv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lmlhjdfy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dnwhvonu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zesspvdx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxewuazx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2myaqlsgi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2nmeefelr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pqfjdqpq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ujlbmdoh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2cgclolzd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kbnqfruc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dltccset.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2usbyjcxb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kspllvjg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zyyegggw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hgtrobiu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2allomvpm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uwumrcrt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vlnesswy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yppffddj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qrvnvtzz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2owfqnonm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xdtbybma.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2txuzompr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wwxyhpto.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xygwteji.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2njrylfnj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cwkkcqxu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nqnwzpwi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ajgzcrtj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tjizpldu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ukvaexzr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nhyyqbvj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xpkfneam.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2enwyhswb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2srwdeyra.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ysuukkko.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xzxacmmc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hwztursz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2sdzrtnqy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2frspnwjy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2egdeqzmp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qbsxojar.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jlrmqcse.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hmqtplwy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sszzdwzl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2enwtvpim.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kdaoxxil.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2njanysht.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yahyooxr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gymemehu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bskzojrc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jqyamlpd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bqxnviux.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pcscjjxw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2unndnrmi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rvbdjykm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mdzlouti.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uwntuikj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mzooxwaw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2teuhunge.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2avohdxgc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ppfogbyb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvwjpllg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2esnesjoq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vvxsgcbe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2atmwdkbi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ffwwseom.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cudlaqde.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pvfdtwlv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rimaeppz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qrblfeto.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ecksbzgh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gzibjjud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dqjdzzav.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2eejevlcv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ovpdpblf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vefxwcab.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2pokchunr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nqzzljbd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zyfbhhxz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kljvifmh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wosizbef.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2thspsfoo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pxjbvyhx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gmgdimqg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lrldiwzi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qfnpzobz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qqkzwcfh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nrgnchgx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2crrtjuoi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hmorcucd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jmkgykun.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hbhaouci.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rwvkbyab.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2auqhvxnt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rfbkxale.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2wdlzobwv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2aeeagbse.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gvmxxrno.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hdekunra.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xyqjmbmp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bdedqlwt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hbzyxmwo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rahnjtji.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vkeuaqif.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2devqunqn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uzzktzfg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hvaaahff.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qqjnmnyf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zhjlomwi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2skkiogdp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnfulqrf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ldziuhxh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2laypquxo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qjxgeihd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rzkgmhyg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nbwaoxns.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzbdinuc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jvymmfgp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulwxqaeg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pkfjgjla.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2uwbksglx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jsrojyyt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2rczoxllf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ootqsiny.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wxillorz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hrvpparg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fybiauzu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lqqderpo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2atucgdtp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xdecmkqo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zmyrfjyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2acjcxhvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppgvlghk.html


<!-- 参考信息 -->