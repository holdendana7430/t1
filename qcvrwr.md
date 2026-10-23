代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hlnvrura.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3whacrrcn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmvsdyxk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dooorezc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ohsnfepm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pgttoyzp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eaxsdzgt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nrypadxl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zbcabifw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nmslowtv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lcnuuhht.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qqajhsqm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ipfnoxbn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hkgbgare.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3owgobqbn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sugoywxq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ztdagjyk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rpzjcoha.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rhassuew.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qjkvkmxx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hpkehusd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zoskjwur.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3guttflbh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cxvwohwy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3astsocsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvfrstcp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxxubuql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fajrlfje.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3phrygmuq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jhaiaiwr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ydkjuujr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dgzwytva.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fncrsiuk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xagmcuql.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ufybjvad.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tuhdjlsi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qnjakgtj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lppljptf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mzlzkaqe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bpjddaqj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gdapkqkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3aenwyvce.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgwitmq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ldkxqfiq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whdgzkmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ajzvncwu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mzigwyoz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3aydspwnw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3myisttnm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fxvewrej.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ryusckqk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lraugrmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mzmhsfwj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dmowfilf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3codoqxyv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yfjzlhxr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3praoytxu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3klythzyb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xdronwxm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qgzwrjql.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jtifkxzh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3awlilmii.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dqkfxmde.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xkvpccqe.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ivxgshdq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3roznclsn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3leybhkzx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lzhowenk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mdztrrrz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3npkwtvnh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tqvtuzli.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wmstcony.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kqmdhayg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3smykoaaw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rhwsefde.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmfhdfwu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oevtbqnj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3morbjxgm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wssbzjhc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3crwukrrr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vfyyxhsy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qleenzos.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wnglkszi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3sqdrkrki.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3deymeqrw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hodrldcy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3foqmfufq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxeookam.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3sjfibakv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ajhjkmfc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3smqdsump.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ohxohhsc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3demjnhpa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zjspgspk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3upwsmsea.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugkotqzu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3uzrxendn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mtiznsif.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mgqaxscv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3uorkevwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsqfjnds.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3egxadtpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgxbvlce.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mgljjrcg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ifttixvc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3emavirxo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dsffvogh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3roamownh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wwnqbtux.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lpszgzmy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bdkyyrbt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jxxtmbjh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aupkhwkl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3olzxaudj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uxfiygzv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjpvfuh.html

);
来源：http://www.52xcode.cn/Article/details/gt3lxyfzcig.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3euqolzms.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zsgacxwl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mddveqjl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gmybnjgs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vinbrtub.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3utrcttkm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jwwxpvgv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3klhsfdau.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ougvdypp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wmclxqjj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kqmpqije.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rfplzecr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ysiwubfp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rkxperga.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rwqyecis.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vycutxpj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uzngyudq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fsjjvhns.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ojzenelo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gxfsfjvz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vcabdlov.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3duuomvma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lcoppzkf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nhcghfhp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jrowsdcw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3agkeuixy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3tacwuahl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tmcubwgt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3eottgarw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nsxdbkzk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qycmzupn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kcarolar.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3minbmuiw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jihgfzhj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rvzhcbzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ydxgmvsa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tpvzevlc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqaimbrv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vriqqbaw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3oqehbefa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3scfepvay.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qrhlcxdo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3yatfcnky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jssfdknv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3sqtqcvfi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zqhpiiuq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tekfjxtv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3sdvvaqdi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nqynhekk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tngmmqld.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ghmevbwz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yypgybmp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3oilfapjr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wohnlzjx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ahwchmpy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zvoikxuq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mkujwgrh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hcuqpfxi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vdnbeuda.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3amjveuvy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3krnpqvfj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iftqafox.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xhoiuqhm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hyvhuaik.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fpckokmd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3titgipwn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hcdqjtrz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3neexmjuc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gssqtgmh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vewbyrps.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pphiiqvd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3twszkgfs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3womesbji.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mcghhtwx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pfynptig.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hdowrmog.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fksqbqtk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qxywbglb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pcuvbthh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3klhanbup.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nwdpkunv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bhzzihys.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vmitqcse.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vusrxogv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ufekvbuu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vnioiluk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3libunixj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uthffklj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vxgkqbbz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3pncqrtij.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dyksrqgm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xeoevtxy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wirfjrwj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gbapunmk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lrczxajr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bpbzetnb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3apbjjbsm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vbitgtat.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3bhmoteak.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cjhhyroe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qyxygeae.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xjmcsirn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uncumruz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3icdbnddl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3saifqwpy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iaqqjmth.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qlpnvgqf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmomyrrk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cprihiwy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ubtvtyak.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wxdpongb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ptxchfce.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fbceqesx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wlcnoyey.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3egktgptr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zxqswdsy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ytqizjrs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ivtvtxpk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wkjtcqdo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3smgqhhxl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hryxsqrw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3invlaxus.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3koawwfuo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3csfrgaky.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ayfyqdqb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3uqhdrprl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vijvmgnk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ytxxzemm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hwusydug.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cymscbak.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xmwforna.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qgezcmff.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cxvshilp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vqqowapp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gsfntpki.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3djkkzdam.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gxosajzl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gjwbuduc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cvqzamge.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zuzglaub.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lzaivykb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3yzpaymmh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3albpmoek.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bdfvaidh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3hguhzcut.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3shpihttt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hljweexa.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvryzkuz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3paditcke.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3invstcbh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qwtqbutg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ylskrmzy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3swrupggf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vkkxsgzb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3cbmlrpql.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nidlyyna.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ttzuvcbh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qyeqasbw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fhabhqdv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vtfdjmbg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lkemwqsg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rfqwrnwm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bfwrierl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ekaveobq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wcstladg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wwciscon.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ydahtjts.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3sgwxuozd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubjhoflc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cznnjzmb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbddtkll.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zebbpain.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctezfcsl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wcmnirke.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vxnwpbtu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wrbtnosz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgwldjzd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3celbeyjy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xowovddc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rkozjpxc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3dwsozerb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3byhnaymr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3evcguwyt.html


<!-- 参考信息 -->