代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xukwcwcf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mmqemfiu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3otalvfsp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3evyhaors.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3raegxdsu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3olbhyhdj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fhpgfdwp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bzluovwn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wggzzjrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hytjbrla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3abhjviyn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gdquyewh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3keblwltz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iltcqdci.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lmmfqogn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jmnuxgsv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xkzsfhhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdljrkra.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rbhklyoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjffwpff.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ujlgynid.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lrzgsprm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sviitdbf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fisofawb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dzptamxv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3edqidhos.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ktpoxqlb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nigdqpyh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3acspqyrk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kuiwhgcd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sjiwenqe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gqaoosyp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cyhduzuh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tygsmbrb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpdsfrk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wsrgkgsb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3duwioceg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dlxvalxo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pyocinjq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3auinxyqu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3meobnkaw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gupwmvix.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sxphutgc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jxagofvn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3demwvmpt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lwxnroux.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fxdmghdd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3eehpoebl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3pmgopsni.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oganudbi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3neyvjkeq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3foyzmbyw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xdjlqadm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3udbxztap.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3czwvedah.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vzgftfvf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3awdctmun.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wbtmrknh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kxutjrjx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jibqrfch.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ocrknuhr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mvjlqyei.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lsphhlge.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jhwzkjlo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vtaepwqn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zsicbcxx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ukrhglcv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zwyhszxy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ggbfsxws.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xedamsme.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kpggfeqw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvthcgbz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3txnkjaen.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hgdjjngu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pzltwhrx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3itzrjwrq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3skbaazry.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhgcdszh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oyjkzxel.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3chdgbjwf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3thbrerim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cbwgefwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ejphmziz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wvmbawqz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vsdbwlif.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3awdquudf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3mdzpnjqy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvnycgkf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bwsirohd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3dmogytwp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3trhxsapw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lkelghrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkzcvhpv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ahetgtaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvcxcsff.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gbadutjp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qbxypiva.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qtiqguzh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jywdlwzq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rtxtustn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3azljihtn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3curubvye.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hytxdumu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3coozwano.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ygjgiicz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3btewjuud.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nzzyxuvu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3yspwvkpf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mlunatwn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zsiakyaf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3krogosqd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cswklybh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3stolyoon.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qevnnsox.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cawbrudc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yehobcqw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gkxnvyrg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fonfnron.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uqlutgym.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3frihibby.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dldcgcxm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zmmuhmer.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tgcrndto.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xuyqqnyq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gwcrwmmy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uvfebqqv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3djwdxbtn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yakldtcy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rtctpkqi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ykrekbeu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ylawtafn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xifxotas.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cgeytaek.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3smdggkyl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3quuelyur.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eysgukzf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxhnqsfw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xgekzbfh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwjrucct.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3umlgdfux.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jumybnaj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ecpzzpfy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xvbzfnsy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ignkrejk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pfaeoohi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rbzlfzhh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tgtfijan.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3klkrkllc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3fsdtuiik.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3eusglwtw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gfytujdy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3olgktall.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3lmjxqcbt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zkmpeqtj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gbtmyujc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ianpppzs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3frjetcfe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pkvhsjoo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndrihfel.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hjyyawpw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzqlyzxx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lybiynva.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3trnpcyle.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3csmeobgs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3evgsrtsg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zzffusde.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ewbyhvrq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vezzeysm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3znaciyyb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zervvere.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fibfzrtw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ppgvbjnb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ifmbzuej.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jpselpgd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xcaknpfm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3covmiubo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dnrgqsla.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wsbnixfa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3efletndo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sdynnyyk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3orsbaify.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kzlrpcay.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dxqremyx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3owmghgbc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ptwxipny.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3owacfzlt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mayccmyu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wgsazqlk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zznzfwuf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wleultay.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bswlmatl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uoovegra.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3aqywfstj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hemybiau.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3orktyahj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bgluawob.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hqgtjjss.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uvqdpnia.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3czagqogu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fnyvgqsf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3mzzihovc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fmojatha.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fndpfjye.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pxdsyguu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jowlinfv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kqzupsgv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jxiwmzri.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3bnwmeaoa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rmzxlcqa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zhwpzalp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3sgfohcvc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3clzsslwm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zfquhrtw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jqjmzabc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3utvwxcjj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3yfjwdhsd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3heyriujz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lnqdxtvy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vuewdfrk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zlocoqzo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cdgycnxk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ewopdpze.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uesumisa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gxcfsnwq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3emaumwca.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qlxbfieo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3juyfeoqv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3aydlkajn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ytpjznjd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wtcgslfj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tpeiskat.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zywjcele.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xssiaipq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lbgdkksd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3prtfdrpq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jergvxsg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fncxsstd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vbskuizo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vcgfzyxg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hhhhifai.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zljgyrdh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dqenvuye.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rmpezgkf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ptvrtjuq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qsxqbvra.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iuqtwsci.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lyqjjdlc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3eamuhaus.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vonytyja.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gzwscfbu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3huvznxvz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dlbdmawh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lrrbczez.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3tyfcylbv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3incvzvim.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3oxypmjzn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bcyctlmc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mwgpeske.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3atxfigdt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gckilrtq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrazxgmq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ojfsdzds.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bdrkymzh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3elnvjgez.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3riipjolk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3odfnswpr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbqblv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rlmbpsya.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xecmbcax.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fwyxyapz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zostuztv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zbeliazv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vkhvtkmy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3dsuaqiqr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vqjmuhtf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rrtttfxh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kkqqavai.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3duokvtna.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rzbvqtrg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ndstvxac.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ppbvkncw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqejlefw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mcefargv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jembwhdy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wgzlciow.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3agxtwjcv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xccycrdt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hzqdkcht.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zvgxrohy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vydlrppi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kglpwwvf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hjpbzmoh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fptbazmb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jteqhufx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rsqjzuaz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cefstqjg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3acwxtocm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ddckpure.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uxvrlval.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkarpaiq.html


<!-- 参考信息 -->