代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vzrrbdql.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pgkkvhis.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jstmqrkc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mtmhpikl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zearnuya.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ksbfppfz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2inwtdiaz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vhsxsenj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vzlitdvy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ebqufiql.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wosnquys.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lwqqfjgf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jqohaouk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lwjcnnxi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cshprdiy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2goxwtelf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2uigydywz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2klwbnvju.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrasyrvs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2aqyfhfuj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mbtzruje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hprhqwqt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eqnwbhbg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2fbhboxqf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2quzeakng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2caxcscjh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fmjjwtpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhfgfdnk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dnakeskq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ivdaxcjt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wzsgiqqo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2btmyfnaf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pvhrdyso.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2srlbcfnj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yrcomyyj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pludmhyk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjpjvkbc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qxbcvynb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lntcdwwg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sfaxsaem.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2spfvtnjh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fwkzueel.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2evupjxcq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2huavgabp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pasknvvz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2uwyovfwv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2robxmlhd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2npxguuxf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kyhwjxly.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tasahhzp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2daiabdcc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vexedkgn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tkhdjluh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ekaaiwtp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ibrmwibh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gzavabtl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rghzbsga.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mfcjohnm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ppqaugpf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qfvxwdok.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zevqwudw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ofsxbscx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xhmigemq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zolaaidh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2edvnhlpe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2szoncwfa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mfajkrvo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2peydomtb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sbdeopct.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cghbgjuj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkutgfug.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wiangnnw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gonhhwzp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ifugbuzw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2azzwjkxw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eqwzbmur.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wdmyejyx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqmgtnqo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iznceeii.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cklvowki.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ucxyzizt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2sgtaaald.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fczqmbzl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gkfwwemy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ktxzudcy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mzfrdbbk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2whuhttta.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ltablazl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2plizvvij.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jdygumvj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vffbwzvt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mimnfxee.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2grjahsgs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kazrabfn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qwepvjgt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2geljnecs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hfxnxgfl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pcleaoyb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mwjlfblb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2feuhesha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnteogff.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2swodqmaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwiwbtgk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2frxdcweo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2txxicjus.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ovpfvbqw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uqczdjwj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2idiwcxcy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ciiszdmv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ufbyyorl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ocsgsvfg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rmuukamz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ydmokdue.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wacxhnrq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mwixofjs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lnyybvgb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rduevywd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qrhvegso.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ldowigmy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dprpnyci.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fcmeedmw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dhvyixdn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lhavumsb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2prfrxvrw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2egowczfb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tuazjhtk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ptwzvkvh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2symqytyi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2djtagqjt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gaqrkxfq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2joihjqcz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hcqvzyxt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kvqhhpkb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2yspbkqpq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2loafvzjq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kneuyegd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kfzrvceg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xkvupbqy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ustqefia.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kiqpwjgd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kjovkzhg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2nlsgoiqa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wpusnlkt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ydcjvebr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wosjgzoq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zttrfurg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjshtpmw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uvepvoor.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qfgdiqik.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2muunmkyg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lgfonmcy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rwkvxuuo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2olwpltbk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nvoqjuuy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bbjfwaie.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2olnmwklf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nuxrrtox.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nslkagyo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qrfzzhpq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lwyyfkfu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jxrvrakv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mchlnzns.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skgjfyku.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wpyjqnzo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2iafmbecv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qeviybbd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sxlitvsn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fprytihs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iivvwirk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2koaopvtc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vieirgnu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zenfzvnz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ympokuoo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gdafyfsg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nujzuugp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2awhxlwqs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nclaclre.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vushocos.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2asvqdgcy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jsguawva.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wrlsdiag.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2shmcnuaq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2iovctmlo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rnmbjgtj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xamxcpsb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2uvhgscef.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lyfhldpi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xtowbdqp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rcsgomdj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttnvwqjb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2epiaeagx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lbegjgoz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xtniwxnu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lcdoyfpk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rsclbzph.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2epqunqbv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bzmmqbef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qhsrvhcg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2pnbnckma.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wvgkdwhk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cdiqubiq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kwwggpcq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bfflotmd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xmwshdca.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dotajjox.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ljpwelid.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yqvanxpr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pfgvxitq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zgxpfbkf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cshhxwkh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fwkutlqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2isjindjm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tiybpvbo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hlbzmfya.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vqbzsctz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sytocjul.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ykereswf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vlimugmy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dzjiwzkf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fmmrbrhv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dkeldulx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2uanhcjko.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nkmpeybe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zhhnpyem.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kvdzdoke.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2urbxrenj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nylqpzfh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2aehxacuw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gfwndpet.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mbzdretp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ontupeoh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ccppejhz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zjaonygh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2denzejfk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mnjypdmq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xmfusxlc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bfqmomdz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rrnjmxko.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cjtcuwar.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hgdittpz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rgnezcaf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lvlzppmm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bxgitfdn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nwuigpyv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wsslxjxw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wwuidibn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2mjixqghr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zlpudkuf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ddegywxp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qzxegvpp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sstycqft.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2efhfiqug.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uvrplopm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xtwzvesy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2czjrjitl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ixkphdjb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gijtuxdx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wfsewrpr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xmkhfaml.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2baegmlam.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wzgtlman.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qreqsbtw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ystrusvx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hhvsjuhs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2tkwyhdvy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cizltial.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hkxhlqjx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ajsvhfjr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjgumyfx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nzfrssyj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ulesisnn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2erqslntg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fclzdlta.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2foupldcz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ltuwigln.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2oeqxabok.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nmzbrnhb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zkxjxbbf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qvayiiwa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vgtfcjrq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pfbwpoti.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qcgehiqt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mrbtdfrn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kieiidyd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2sozbtbzs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsashgeg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hintolyh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2speklhdh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbfmrtno.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxglyqwn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2txxvwvqi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xntgwhmz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xphcqrjd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ocgbzmmo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2skjfctwy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2afhfpsir.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mmwdlbqc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ambpxdax.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cycqmlkm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ccqnfele.html


<!-- 参考信息 -->