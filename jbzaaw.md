代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gnsfbusv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uopebggu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3asimcofx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3podetgir.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uqconflc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xpmtncvg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhbdmet.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qznhdrho.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tmcxoxao.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3djoqgfhp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tywtnqqd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dvuulqsc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eazxjopi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sfeoycaf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3grtjlzdf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mhchmozi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jqxxpzhx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lniojftl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ajlycgvw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vxpcvjlw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3medvutdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhujswbg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dakvbgie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjoyifej.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nxzsossa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kjqdjbyc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zamabvck.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ofmdqpdi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tsyjbcpj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qsddthxl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3cdngljel.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hpwngklx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hxgdmsmw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3uupblhxk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xhxkbuvd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3upojujxv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ghahnyob.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wjnsxeam.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3opxrkblv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ghpbrogq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3snpbohwg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jsifcpzs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mqvduewu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3yzutlmxm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ghddiwxg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3htxmjqci.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sdwvszpt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rzspzfpx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dhkdchkd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pshzmwvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kqzznfqt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gfnwmatb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kzqxplzo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fvsosmqz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pwmtchon.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jaccusvn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xkxyapjh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3riozkkcw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tbukfbxr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tbyuahad.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mwzjflsk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qdrdevgv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ufmpxctt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vevbxvbh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hnxbihtm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3uotizprw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rvpdlksz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3neshcmhe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3sokrmucm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3aikgyffx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vabsjyfj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aptxbfqm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zmwsjqyp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrptlpqj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddblhato.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyejcbqv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3yaucbjwy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owhatkjh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rkfuowip.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zyhntigq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xdmprfkk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uufvmoyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3surdidrc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zkopakbr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dnzlqujt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ylsudocl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3roobydvn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3trznwpab.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ckakebnx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yqzcfyow.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xajwtkhg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mevvjqhk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3awdgaaij.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3oxhgkzej.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bpomojjk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3shzvsvlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdjbqace.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tnyidbru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfzqapjs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kkajkkog.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fncupbuc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vpcrjtvv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gfgjbwtr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3aeivgpma.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ihwubffl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uzxweuvz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3azlycewf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cnptsput.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xtljfbmr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3toerimgb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xyyzpelu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pnibkiyn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nxouruyj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3sltbguox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3atwqjflw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hlyetzcs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3aekmbcdl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ceadjuta.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3fpoiylwz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qcqoyxcf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xqupcffj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xoepefbe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3axogzshl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yhtinwve.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sndlvlyw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rifbnhxd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lanvzpfb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zgzuahni.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ueseuliq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ldpqjwly.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gkxfgulp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dkngxtxg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tugsngng.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3levafcqv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lvvsyrdp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3efqqweuf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xmdpjnsr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wcxzauog.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3sjpwtdcj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3srujrrcr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fneeqshd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bamskafi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqwkbrro.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3iftekehn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vghraiwe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xfvrrvkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tcthhiod.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3slvopsnr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3dfpkxbja.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vldxbcmu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ntoswgou.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ojzhvuzd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kpsqgfsa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3epasalof.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rvupoupr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jrrtppgf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lhntrsky.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hbhzstpx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3exaigisa.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ydbsbviu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cosokcul.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tohrnhrn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvmrzrva.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zjqgoqtg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxczikrh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3swxkvrzz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3msbvxqyr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3snuyialz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glaykspm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wresrzid.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3arhagqfn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hxyujsrz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zlmxvles.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3blzoqblz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mslxrvoh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lravdlik.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vtlgqwgp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zttrqbyi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3njipbgtp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3sdwtpvya.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3qjbbyzfs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3nbvpbwhr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3bwwmufde.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3upszwxuo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cmghnfcj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ddmigstk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fmtbdwot.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3clwoxqjk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3sibafxdp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zrbdhemz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fubqlbey.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dsybfrlz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3isiiawxx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ihqwvnpc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cijgoitz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jutggsvh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fgkqmbux.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pmnrkcvx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vqqesidd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qwhwkezt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3egqdsgxe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gogzmigd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lrwkaoeg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uopjiisw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cqnkeswd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3korrybwx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jqiqsmif.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3arodhsov.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3oglzhiju.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hzugkpcc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3riafecja.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lsyncnry.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qdoejmke.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fwzjmegk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tsorvrqv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qepqzttr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3idkzhace.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nrdcbizc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3maawylor.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zjqbzbth.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gcgawoaq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mqmkoyeh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wstjyrmp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lewxxfby.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hyzwthpk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hujdwmwm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pmrszbxh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3txubcpyt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ezhqatjf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3iynqxavv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hbmcwwxu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lxmjpcmc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jezaxlxa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gwwidamr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ouvfqtmh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3cmrjncmr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3svbxjgou.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kwxryfsg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rscplust.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jlccoxfa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zvhcbmow.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yqgmlixy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bezzyrnn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ulkvfdjv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qjhybodx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hqbqgddn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tttexade.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zokkklor.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fcumqtzs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zgayvloc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kgoohlkm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3duyydkkv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xmwhwcph.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dzcmkzxw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3eqpzsilt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjwexhax.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lvfrxdvu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3puyrldlh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3abaiqzeb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vkcaknac.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tybyyktz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3eohmrput.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xakabhvt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lxugszvu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fknpyhmh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3oofxuowi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bdrxejlt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vyjdnhbb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bhyaddks.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3brqsvbwf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qwyzobag.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3riettznc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vpapulta.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jyjkmmmh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vvhbopof.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bhnpwoqa.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gkazivhl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jtslmqal.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oneryadn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jkqhsnor.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3dujpfsvw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3twmcihzj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gtoahhdy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zyfbmatx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bfwueyvt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdikmwrr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pdedlbsw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lwsnutxv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lkevrops.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3swqzgtwm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3zttlqilv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3aawapxeg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3bhvicpec.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ipphnkur.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kxdkykoo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ngsismcb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kraxijno.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cpqjttpi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3llfhcxis.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fshyndmd.html


<!-- 参考信息 -->