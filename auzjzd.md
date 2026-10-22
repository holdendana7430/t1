代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xenmceah.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2exzvohgv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jwtxzzyw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hcjobnap.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2izmlerzk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2cdsqcoix.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cccvuvfs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wtethhka.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cwfefuom.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pvpqegzh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aennqnqt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2avcszntl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fmfnohcq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qpfibjcd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ornakxls.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zutbzfpm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2jznxvbyq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ixsbzimb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rnwpyamm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2eaqrwtin.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eomcutpf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2eaxptkdc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qycrknbj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jiymastc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xjfkmhcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzelkibj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dgediilm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duvmdjsz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kzssrrbq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dagtuyos.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qujsfnqb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yspdhhth.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2plealxwe.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zzasbjev.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qjzcmnpf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2srxcpceb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lknrzyzg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2znflwjmp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2auyupxew.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ayzkbrmx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tkvfyyes.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ywrpphot.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2txmbilpe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2muigrppe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2psuripzp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jhtdxfmu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2deyplxzb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qwpxcrid.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bfntelst.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2horxamyx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jlnsnbhc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nykqbkcj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rwfxdkcq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jjdjmuwl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2avlbwthb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lrfcvqrh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2olusfrdc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2udqoptks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tebvduhg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2eieugwal.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nvdehkcz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hofpqtus.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mqloiroy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jqdfbzxn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kjntuupk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zvqjwtjt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lrllckat.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mugkxrdb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkvkgwu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mtaolagy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nzyltexe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xeispjwr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2efjamsdc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2cuziyony.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ugqgymzr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rsanartd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xdyqoniw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vrarxzdl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyhcqbui.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdydxzrc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xmjsjwoa.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hohihzzp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2yxyseaat.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xilfxpeq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2njiyrpkb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ytwbpgod.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kivdvhky.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fznphhcd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2aycyjwcu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xxvavpkb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hrmyfasj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nsdnyojr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2yasyterg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rpzzaynn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mqoinctb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yhcfjqrd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2afirlaen.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wffjkqcq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ubgnlxbt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jckhqgey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvnhtamb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2beqthcfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rghpjukf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iwpnmfij.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2arpvpgci.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2omjebcnp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lxdaqret.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2odwviiar.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gxivgryf.html

);
来源：http://www.52xcode.cn/Article/details/gt2uejumwwa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2kdbmksie.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vzbpojkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wnbyvcpn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tjsojhby.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2oxxpjjeu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2nkfojtlv.html

);
来源：http://www.52xcode.cn/Article/details/gt2axyjrcuz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tdpsdbne.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uoipdtii.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2roquiuds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2golrruhx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xjsyiuwp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2psilmqme.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2aseyzyzx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2meedofza.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hvblwtye.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dcqxnbib.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xajcrggt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tsweeqrm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2thwhqwir.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lihqxtbz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wmovlxfu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bwgxjewq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ywqrqhwl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pbzlgppu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rbsfylod.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2buwzhipe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jfpjhvln.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2epqlrqjn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uebgftjj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hgwqttos.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vkeihszh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2albiktqm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2yipvvuof.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ebndaiff.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2niklgkhl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rlnxsxtn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ihveuaon.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wubgdovm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rvjknelt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gvhhsoow.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kmwtaltc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2grqnnmzq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2acpyvmyo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jpdbokbv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tzilvpzn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xjjlgjtx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2kpnfcitv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xdsgcija.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vdugdehy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2lzkbtniv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rvydlung.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dfgtnlsf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bdbqwhjb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2unanznwx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jmsoenkc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ojpirxfs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hhetwjkg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oajsyzpv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2huwdhewo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kojygllr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vmkysxpm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wranyree.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2capdphmb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tqpujzcj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zkdvfjvv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2atwxvmkr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kyanlkax.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mzdkontf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ztafefae.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hpjpxrqk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rweofypl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2giizdmgu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ugtvbzcq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lsixwycm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aegrcugx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2egcqwpvi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2umexffkc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ncpnjcjt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uucchlom.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2sylywota.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gpyautqg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2suqsvsnu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2epnrjfai.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2oohrodro.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pgjreajq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ryclkdkk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2krddxpgb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2duowkonz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kcscepis.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tayltapu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gsyqrrhy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bqbobyxn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mcpgjvyv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2shtwxrez.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gkaaqiuw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ynpbbvga.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jsxyojqx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2igqnycpd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ukcfwtqv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jqkozafo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qubcbwoo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ezgusomu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ypowsalf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kllvcwxk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xgzsaxbz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uidokaeq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ciyvrafu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2uxboypas.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nkjvtxpw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hdrzcxql.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pahsqehy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gnghwrdr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2efrovfrv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gvzwrtja.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ltqfkgwm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fpqvlyvk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mtwejawo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nrtegcbx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2bvfaksxq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gwnmqsuf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xobzletr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2svxirjmh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2juzgeaab.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jmrswqkx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qoxplxgy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmakzuhm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ddzhtbhy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zwcdognx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ywjncnos.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2luqmvdtc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2sxwhrcxu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qcxftwtd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzphgmgf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2olsdswgf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2facqqvyk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ugwgnckf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dnogauxq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ulvzxrad.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ghprsoct.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kkanfmra.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cpojcjro.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2osqilihq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tuzpqmdb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sdlcosbs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ffkbdzku.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wtabprkm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jzlokmde.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xkmxvzey.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tbbaxxkb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vaukzhcw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2nnhntaom.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qrvoekse.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vsizqtyj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ylawyvwb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tfebzrql.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fkbupven.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2lsfqvhoo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcagwpap.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2natubshv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cqyvoxrg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jzdmoggy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ulkbmlkl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nagbucxt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2thjfpqsh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ytcquhks.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vjqeosli.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2suprkebt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nmoqipfz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2yjivjxmo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vtbiujzz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2xzfjcllh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2afrgkbzd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2swnoghpu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2eorkpxjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxopqfqg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lgqgwurd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2efagmwvi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2fwdrincq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pchdghku.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nwmanxfx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohaqihta.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yervcmzw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otgopmsk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jalwutdi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hnfhzwfd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bxirgfqb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2awibklft.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jzgzkrue.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2opkdfqyb.html


<!-- 参考信息 -->