代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2mxegjirt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrpbxqzi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2iopycbjn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xornpwpw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2skrysmpr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zuexiddz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jkeiucfs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ujgzrdxi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yeonjmnh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zyomysvq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sdppppgj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aaxgznyc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rvkgizph.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2iyppvzky.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2itclkazs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fltucmbz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2njaovcvs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2inihxwpw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vanepbmv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xdgusgts.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hcxshixm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bgmqxklr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eoevmixt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ovyluljn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tuwbnqcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tchifkuo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytmkqhzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icrxfggu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sjysydya.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2tclizada.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2suztqnbd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ysydnddl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2watyfzdc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rodbmdrp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ylzpibbf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pnzwatnd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2sfawmlen.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2cnpjpdxs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tjbcgbkn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhrodta.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dwzufwcv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2uaciekmz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nnibeoou.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cucszvre.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wswdtseq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zqoctamf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nqhzpiiw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2uuotkymv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bnfrfjbj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2myeeejep.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mahetyhv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fefwynrb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2sxlqqtdl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fehaefxy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2xawanptr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wivbizsa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lmykiemo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2auhehzuw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bbzfzkyx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yolxirbg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zjhasxjn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ctnvcrrl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tmektoea.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bmcxvwwp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uegvdfig.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kbkklzqq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hrmxthbl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rzlxphqe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rqzxkpmn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ujlxctsf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nblnfqcj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lrldsrhk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cajxetvh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zhyzrzob.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2abbxmmay.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udtpmlwp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2fpkfbfzh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2amrmzcjd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eyfpbgoh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2opgxodeb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zoltmfcx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nsufebpl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tjquzwgc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xblggnzn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qhxalmsw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zdxdarrg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ujumbnhe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hkoozlgn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ieejwzhx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xdhvynsv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xjcpgqar.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2grprxnbm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nsiwzcjs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qtuokfyn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jlbzgjux.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nodrnobq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vblnodlt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2taesufcj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vjzrnxbw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2iaexkeve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjoyrlub.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zkaamszt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auezrdxy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2oeqzpxdd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lqzptvuo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zqkxzjnc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2whsrjtix.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fxfieliu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pqshtrkk.html

);
来源：http://www.52xcode.cn/Article/details/gt2lalidksi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2nversiva.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pyakvtdn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cshmsrof.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nfmvzust.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ptidnizz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lavjquaj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ggnpklku.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2deabjnpi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jrtxriyx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eljfcmvj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2oeyhsdme.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gowpcleb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nuegeeoy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hiegcyjl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2otvxcgjn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xigbickf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cdrxebpo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2pivemgwe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yrtylxiz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hjjrtigz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nyippaqb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2byogglom.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tarazutm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ycwyufcn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2botexqhy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kvhbqfkj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pbblvafd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jesvdcnf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2txofqtsp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aumoggib.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2sgzfcntx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ullwxgai.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2awkwzzeq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2sqrvheda.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izdmpfpd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gpiptcyz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aesnuwio.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qvbbzpgk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ifrzmqzb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2firjixvw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vzwpieiv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jbdgrfhi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jawtceet.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wwvxbftn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2xwxmsykc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2guyjhruu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mqurwwxq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2aasbgyyl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dibbcexk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2buexyeht.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mijltwfx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2igsbtjaz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nwfslzfr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jgkwnsqi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hweiasra.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xmumrnbh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qiukxjfy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gjptjndw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggtxxpud.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2guuijbmt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2afgsvtla.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hbddzdyb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kczmbbhh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zoqijrpv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vyuxbihu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ftbfxtgb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2iblibutt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bjsmeprg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vbsifzoe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2oobhpsnf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hylwtocx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qshiihpz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2aipyflgi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2btbbfbxr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bclwwsez.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wegxtont.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tcyfcndb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xjznpxcw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jhkqoyjv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qbxfxcvs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ohnqogae.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2icpqnupy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lbmzvioj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mpvxogpf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hqnnzqfn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ffcgvixw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ycdjigwr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hsoyprxm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mnecsqkr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2conhagiw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lagyhemx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jbvkseky.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mqjsjllg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2arznfrfr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oavzaxwh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2luthptzj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ghflzkdu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vfnacipp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yjczeeqv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vffflfzd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2haksbnkj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cntewtjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zuniojym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2butdkptz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gdeakjux.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wnfecgqq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2txmqemjx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fcckrnqs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2smagkchb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pjqerznf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2myinmvsa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2arkulern.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2txzkkoqn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rrrlplww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kzpbjsoh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2swllnize.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zebfpwmm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vflycwkv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xsxwvuqx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nnclmiru.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2exguytxh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jtbatfja.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2adaffkdg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2odoymdnk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eklxjunl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2muvdjnqx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shyrobzl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ivzhgjjj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ifciohii.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lsbmwhja.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fmtfawdr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2onqqsucj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wnzkksnk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cvzxdcdd.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rvjgkbkb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nbkdckne.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jmvlizqy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2luewajgy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bsdompzg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mqlhxvag.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rsajeeba.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vacmdwlk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2eilplvkk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dkjvepkq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mxxmpxyq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fbabpjie.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nunwqlan.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vzxbeurs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gjzqexgm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dfnololc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rzwrnqun.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2onpfuiak.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2etnboqzb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2epnknoro.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2glnxwjxy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2oncrhetf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2brwwgybd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dyduvike.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edmoespj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vyjdqjzz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qbkdnbea.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2euraldqx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fytsmkul.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mjpeohkr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gkhoxwpg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ytjiikci.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2potipfcu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2oidtkjjt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qscbldqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2cxkltuvt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2osmmbklu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zeguztrz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eijcsewi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zlebrxuc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qggjuqko.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgfzrqpg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ycfdebpg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vnzmqbex.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2iznicgag.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ucfcxeqm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rgaaexyb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pepckuzi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kqhxaogm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxuhfaxc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mjfrlfvw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ulvetteh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2opkxalha.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ukiuttje.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2unitiqve.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2otqprubb.html


<!-- 参考信息 -->