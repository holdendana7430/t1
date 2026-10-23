代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3darnvhcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mqxkijvm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjkllsk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mdhdnvvi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3yfehmbhz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zyympjfq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zsyfbthb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvonscrk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dktcjbws.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hgtthhyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ddxkldhd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gesuzihg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lotrkrbt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ngchbiha.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zlzuiovy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3opdfhojr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ofqxtfxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suuqdasb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3syfsauyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drxqghlb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xfzoigni.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3oaxuqyhp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kbcdteie.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3txoegqal.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fyirsfbl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tieaauhi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mhponqfj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tgolzqrs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3eaprfyrv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wveustsu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3obyyhqxi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3znvmcvcx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3blbycsdy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xkuhwvgs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3msodmwpa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xdbtzmvj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ecgxgsaq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nlkueztk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yzicvbwi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ldwltgcw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3alebatsi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fygjtltk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zbqxplfa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rxjseihq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qadiqbzr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3eblnfibl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rhfubhoq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3aypwcwvw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3emcahzjq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3marnvrac.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3caarspsp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yuvmkczv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hluaynpr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3twupboku.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3aluplonj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rhcswrml.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wruavakr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wfagcpyi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jqqujklk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3akmbgpkm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nczrvuoe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lkzfehkn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dalxrely.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bpyzcbzb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yoqgulxr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mdtskhqa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3factliny.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nehlfscm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fkrgkvws.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3asdqvqdp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fedhzixu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tupqumqx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zgmosgml.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utsoyndm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tyeoviog.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gdgipenu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3udzdkvlj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gmvhcucj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wkupolom.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuxikxrg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mbxuynym.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zfohakil.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3icatcdal.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zikyfqvb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mvsresnd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tvbkimsc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bajhfnga.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kqkxqzzu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3afzczsrm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3aupttjvi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3svgjqqik.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jywvnkhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npfphlkp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3suaubvqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3caeaojmd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xnwufewd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hzzfnvaa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3chkkndqc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3blnpsbwf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kafcaqjp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dpgdubuc.html

);
来源：http://www.52xcode.cn/Article/details/gt3bxksvfpr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mlmmxvnl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3eaankklw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pfdpfelq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3adylosmo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gdobxzlo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bnejcvkv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fefhqfjb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gyxfqtsp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nvbfdcif.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ungomdil.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pprwrknx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ajpaetjg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mfmfjmpv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fuolukgm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3urfeaqym.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bqgkqbdb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pygmvboe.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3eywujivb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cuzouaea.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gdoplyju.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ejqzpbas.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3obtvogfa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ujcbixef.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xgzjaaot.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vqilwuqm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wdbgrhnt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hmlvhhlk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ddlhgsvw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hkvzmeok.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ignjleoz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3atodyofx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3spexxrou.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jhbvpnyh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3avxwwdbo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czbjunxh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kzuxcdsc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfptaukn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vummvgkd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wvqdcdyd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gwfoqdug.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mieznlhg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fdyjqauq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pwvxntvg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qcdpjyqj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ercvhzav.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lbiaetoi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dzghqmwr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3aobcdrss.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ujjwanxe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fbymxxyn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hrgssvsb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3akcqxouz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3btkbyvfy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ifjbafea.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3oqoikxmy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mjjoytbu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfwjmdaa.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3czlbyjvj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yllskbea.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xqiqlnqx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wfaudulw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gggvwyan.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zslbomga.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zvcqezol.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ijbeeeqj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fbhzshwg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cwdjfgkd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fmmmylov.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3slvapppo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qodyxisn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3utrzpstd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3oiilveer.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3weflmmsn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rajzuiqv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vedtexaj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wtziajoo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nojnpxec.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kbumfube.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3xsjvputp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jnkzvmli.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vuzwfgxe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zhqgvayx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xgkagtkp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bqoamzqy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ofqyfdtr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kcfwsdzu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yrofpdyr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zfunzsnb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3znipribi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3swbacbhv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3pdtywjot.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lvblrzng.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3eyofgmrh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3efgdcpfa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jehmbmwe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pbpxoyus.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uixqoxzm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3naxjbxsy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oxvnljws.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zfnpbbms.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gkuhlyqz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xivephpw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3skkmrxdh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hfseerjq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vfxdgybl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mgefdegp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3elihcxwu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3cjwerddl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mzhhslms.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3becbthmh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xtmvdeau.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hbbareso.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ipkrbzxx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vjhnkkja.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ajbfoqab.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3caphztmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gajztgdk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qlefjztq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dxjyafqg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zskgeuny.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3walymvqb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jbngteyo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vomeddsw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rsjbxleb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ohdxoykb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rrowzchi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bixcvizg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eepejwbk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nudnpmnu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3sjtfqqst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3moxilekp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ecaqafos.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3grggqudu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3szxuzwge.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mycprwqy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mkhbzojt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3equueipe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zyhhhwdx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xdvdoywh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ptqajadx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jknrynkh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3twvjvrbm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qbbnpdzx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uftlurfz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qopiednr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rdqvclkd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3chquhebu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ttkizcct.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nyypiqok.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mrtqgspf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tpgkgfcd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xgvtitxk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3natsbglk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3dogwaopr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wqdcoyfy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bkvjqqml.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ztcytrjx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fghpvrqw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvsflenp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mvnzvdui.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jmbrcxef.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3htopxqjc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ioxxxqwy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3arqivhqx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tjccenra.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3iezrfcig.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lvfyqoqq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iwwlamtt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3suurllgx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nzyjwcyl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pryuafkm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3krdlreie.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hgfokcif.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qmpxatrz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fhtcsqnw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgubsjfl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pbuzetbr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3apxgyyip.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpbslxan.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gdhmngrm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lntlzeyc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dolqwwpx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mnpcmdic.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwisksyj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3thtxmtpb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zyrukgez.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3menupihf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mbgqueip.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3egzjjrdh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kgvvijhl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3aeqyhtfu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ufexwdot.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nltgwwdl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3thuzgeqj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3weswczhr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ntozzeym.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3wlobxioe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syamrytc.html


<!-- 参考信息 -->