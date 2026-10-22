代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mibnmkuw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vjjcabpk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2liauktiz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zdkuogkm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sufxxnda.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2epuxffuj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2auzoayfz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yfkayihf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ymfmyurq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vslmrpsv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cixrvmeh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lkeihmby.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yecpllfk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2okhbynpl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mnahvcgx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2njxobyxf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2stpgihlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjnkyziv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bkgaikki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vesfpcmh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ggudnfiu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wpfshtja.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2npqqzgns.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sjslwknh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rkwqktmg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kexwcczf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fahkczfs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hmnpgxyh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ommaslft.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tklsonzm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2moikguxn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fvgfxlnd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wrmxsssg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nkvynsrp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eagdqewk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ooijryjs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqifiecx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2absfvihd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2omgksjrs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2sfwgruha.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vudjgyfr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mafqghaj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ecadaruq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vimbbuvl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xxvewebs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nyfwvkpk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fkyirvrs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kpobgayj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cdpknavu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qbftquzq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fwxavzfg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fuucajsm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gukdynxz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xmeibjnr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fqqajawc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mghprnso.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fjpgkdju.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pbdzaolj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hbtfghtn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2brzugrwc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ngafhlcf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lvgwkfdh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qtqjjfzz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jencfabd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tqcqrvmq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2aizkjzec.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2suukprxr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vrkgnwre.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vrzwwgem.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwlewkxa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2grjeiwif.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dalvipip.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wdmxnmja.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jicyflom.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2azcphxux.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2eiqegxeu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xujzciyh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2umdisjwg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kdpvyndh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2fsusrykz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2anhngxkk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jqkbilfr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2juqonhgz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kntxlumm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vczwmiif.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vzmjjwhu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tledkafe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qrdmysmp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yzmtmbkd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bhwkwdum.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lyqvcyep.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cxuabvmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yiyzsfpb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ynsmdbsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwcrzeqg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vaijmsqk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ckucgeff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bgfpchsy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jrlcmqzz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2swmxmnzp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jszsafla.html

);
来源：http://www.52xcode.cn/Article/details/gt2pauxzflt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nhdisgae.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2phihitwz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vmndgrhd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tppfplxd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nyigxfzc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cmqoqwxu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2maidzuoq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jywkqcad.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jhqfiwoc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2motdeqqs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qyxldawu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2frbfbvfa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2bydcoqsm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uziwswin.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2yekijaqa.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2uswntrnv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2lpocezwq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vrzwqque.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xcaonzdi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tpclekop.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aiskdwcv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2agjrfjyl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bbinehgd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2arhntslv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gfptrfml.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2cjvteuiy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2afoowulc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2littagem.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2aqgjtvbx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nzqafngn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wrriureo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jucejvee.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hoalqpvu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lsvlylua.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcfciufa.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2grjkvgib.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owvbguea.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lahusevl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xvwluyjx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mdaxfawp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hykvtehd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ldtovrdf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ywoviavr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lwqxnsjp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lxvqrayz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zfuruicn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hjhlxjaz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bxdlyazp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fsxnaqnq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dsuujsve.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xagjhmgg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2awteaiin.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilqldfkr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ehewvzpr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qlsnlqsf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wgsrtabb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uowvqlke.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wewyxqoy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrkhjycv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2aunzvlmu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sezhnadx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xrchmqhb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ooctrbbg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jyexiwpq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2upbwuxur.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sgkwkdgf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pksnevbj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pelaobvt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tfnfrpgt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wymsgagh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ztnnkewd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2uvzyacxq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2isbnsndn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ezqicupb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bggbekgi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hbbhqrsn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2psopgfje.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vqwnyvgn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2uczovwlg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2crvqxnex.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2upiggjuf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kngdavrp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ntjnozcv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yeirfrle.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lvfezleg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gvdndtkg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wpbtvoik.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hwmhljff.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pldbckbw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2sumfislv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dlrcmmwj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2gbyqocpj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xsdnxehy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kynfxhtb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2iikrptrp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2upgogzvz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zvvhdpcw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xxzkhcus.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cblwzvhw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2skccdlot.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rdggwmsw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ohnfmwev.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2shlhpohl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cuvyedmt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2abkxiaog.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xgnnclwl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hdfuukve.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lryqwytz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2znhvycqc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gwenujbu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pctkxdkn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2dqszcylk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uaugcgcr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lzwdnlvd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eigjdvoa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2uzocsuyt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rojeirfi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2egrygkhc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yzvqyjjh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fdpyhdvc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2amibqxre.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bdtzvzoh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iimxfhht.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iujmxqes.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gzzwzkdh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iktcinea.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wnrnreck.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mrpglkjv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dtnqgpje.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rypjethu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dqpssnqb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bcglvwcg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vnbhrpck.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tjtjgcnj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2itnpjkzg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mkqrbpey.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2oegsbwbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xnbtozpb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ljyxadmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2grupyrdt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2oeuqaqsy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lgktmooa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uvugzbol.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mjlhmhmc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dngnzfwc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2iinhghlt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xavzmtje.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hmimalmj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hiportuv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qgskszly.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rwhjaeog.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zvewnybf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zhogjvxz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2gpctajdk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmigfyte.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wgehyadx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vbuxkdrc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2prkxewge.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2obczkhtu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nslgukla.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2oirlaftb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hlyknhov.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2emajucim.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yoshnpmi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zkazzlxk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bdgloxhm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wolwkxgo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2iqelezpf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ruesoxpc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gypjdosp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kihgwviq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wmqvemlk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lesjnxlz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2prhflcyh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mzsezuha.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2apkmkwpa.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yzfwqifa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjofqjvc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2prooxdol.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqmnesfe.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2udwwaioy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vuxrfzgm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cagdqvlx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vasxejax.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2eecjcsrx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2amnsbqvj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nwvkjydh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fdbndain.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dpdtgknk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ytuhseze.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fkgcvmje.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kbwunvpj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygjnkyzo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ytjynoog.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2uyaeqiyl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2uqomqqfp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bdqtnaan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iubofgam.html


<!-- 参考信息 -->