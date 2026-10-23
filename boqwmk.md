代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dnpykbwe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rvxechgc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3smdpcgei.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzcuzob.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ssuubvvm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ecqkyaxl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3akgbwvri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3immiihnc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3tzrilnqs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3euczepce.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3brqwujro.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3svojkryi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qefeuhyw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3efiyybcf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dqvynleb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3auxetwjj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lhtjmysu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hozodchl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdlmrims.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybnbnoye.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3srcxlbzk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ogcbsmoo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fechwehp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vuojwjew.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tqfvtiwv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ibbypnit.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3eeyfiipa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zywuphhe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ruquzwsq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3puqejlai.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sywwdikx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rjztcwhb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zbqmjyna.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xshozjaa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jstzwyjx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kpbkpqlf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlrophaw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uobddbyn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eesajqjb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ydjwforb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cjtpffks.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3soafaeom.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nhwkvcts.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nxeawrvk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pfimnvff.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbinkrh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zmpdysqg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yvhjaczu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3izbgwewq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3giyufnih.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sjhpwiiq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qluhqwyn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xqnwfobz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zoprdxmh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ekqpmmbc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wjaxjgzl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dosapdeg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xthujxqa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3soqemhja.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3disvnwst.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3juryeawx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3cpspfvbh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3akbsotyj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gxatdktp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3zogvgvgb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mnmmrsfq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sbpsmrmc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdnqcvwq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3slqshkuq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfxplnmh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ieoosxav.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kymwubdj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lyihlkus.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3silyayce.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3dqlnwakn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nntyleho.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rzmngfsu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gcsbhibk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kixsamfq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3umxfmlhw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wmtrevwq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rhwyoofs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3otattcwi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3izgqzcph.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dellxigf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jhadmubt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jkbvghet.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3noryeyzz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vfwhfifq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vyfjfdzr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3leyfscxv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kjhsmxii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kaedbuwa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3rmayaowd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mttpvygx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pavjixle.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tluhsppg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zextqshe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3arcvjxjw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fljrpfzx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3scnxgssh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jubuzdvh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3sujqczam.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ipucpvgm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qkifhndh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tpqnhrot.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uridkija.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hluriqfd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pdhkqeyk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rhdbvaeo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3obcilxlj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ajcupluv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fafzcwbs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dczvczpf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3iarlhlmh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wgoqxkmv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mpazyfzf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tztlcmft.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ycvlwrlg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bcxhsjjn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uxvnmlwl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fmjuauuz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jromoymw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zblxhati.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kusnubkt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rpqkcxbb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ykrlabcv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gzbijfck.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lhcobver.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3iabhyvpf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3svgcgyyd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lnunfepu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3khcwnedd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qpgvzrhe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3eekndoob.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fndbhsmy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgmbgltc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ncebmsop.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxmimeyv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dkywplkb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gocbasls.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3litphkey.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rcapbgmx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dwrzeqyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3aikmyjcr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ztxtokdz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tlthihjs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ugybfyna.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cmkdsvam.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zzddzjml.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bqbjqhaa.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tiflfmjn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zcfhjimn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wbqukrjn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqdmzfdl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fqzskwmd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3eiejrhvc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3eyuutyvq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzvxxnjo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xwkoaxbd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klxmwibq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vgsikvnz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eemcckcg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bbhhbfhc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3boennzek.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ntibvrmp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nodqempk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3caaxnuzm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3prrfpuro.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ymmzzkhh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ynegskhd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tkgkfqon.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3khbctxdl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xfwjxzrd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xzkwewxg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cwzehcjf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3szgmowih.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3keobbpym.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3igemhkyf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ykivipdn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ndzsvqgy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lsxjefqy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3legcghuz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jhkxzqsp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3cvqoziwo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dhpsavif.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3blszihgi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3plajkbrs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3slpidsod.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xavoinhw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lirumkty.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nybvnjuk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jnqfjpga.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xchydiss.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ogbnsjrv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qrxvaqba.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3sqmsjjen.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3lbngmrqd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hbwdwwrf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gufwljzq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3aggafpcs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gdgbcwvk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dhsgwrik.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lkdkghue.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3iudzvbna.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3prbjdptt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3weoyhvjd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3egrniugt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3itolndde.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ukwffrlz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rivzrxjf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zlpssfah.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iqtcnsey.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3uezpyibx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3okqzqdls.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3gpesoqnf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3yvrahzsq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ggcfignl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nzztpqfo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nycxajab.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fdjzvtvx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3brjivaru.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zyvkkolu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3npxkrzdy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rmumutms.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jaznrlpm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fpquetzc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3iexuqkvq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jkesmzdi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3scwhrrva.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qkujigax.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ljggpbqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yneotflz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kiusrzux.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3reuwuqsa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3camspill.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3eylqrsbc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hjhuehyr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dasboolw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3adxfklkh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3frtjdpuw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3osfilnmm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3aqtkercs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qlskystj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zdbztyde.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bomqijna.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ngzrxgzs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mlfeaeyr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ghosljie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dkmvcnhd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ptmmmtyu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rhfrfjxa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ukykpblt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wvumulwr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uoxawojb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3aucfiyfu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbyjktpf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3cvswdlqr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dnwpxqsm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lfynuvgo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ucbcarpd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mrqcrthm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tdswfctt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3modshqmz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ijbjdsxg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tdxkuovg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dszkvkba.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3obtnkqli.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ipvdbvey.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ntrpcmti.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ysoprudy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zyablrbd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tccgcyag.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mtzgmsiq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mdvydmds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qjzsyicn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wpojxaqo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dgjtvyux.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ieluzydw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3itemxbus.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3mgwliajh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyemnfrt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sulcpynp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bihvaufl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3molunsiw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fcvjowpy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dhzynpnf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cpveccdc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3sbvljlws.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uexdwjgd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qfkjqcol.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vkyrshzt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qllybcwu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jegxovsb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slyvxpje.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3virjszja.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kbjrobwz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hlrbidkg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3iivmwmzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipzgcpli.html


<!-- 参考信息 -->