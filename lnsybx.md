代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3psjelqqf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ncuwintu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qavymitu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zszcdycu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3itamyvvw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3uiarbltl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iwymyvmh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zwrqfdeh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mdgoewrg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dvfxrxpt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3utixlait.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ufbnicto.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mxwjowkj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xjsjvbbz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hlpnroaz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lssffrao.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3yuwcjxlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxpsejrb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ptdqutqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnzkclhz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3unjngezf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3sasusosl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nyvafvti.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iolssgts.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ukeltrju.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3thjuzeid.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rxhrcdpf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pcsbnxvd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lrdypppw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jolubtjo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bfpizxoa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3sohcwrmc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mxyadara.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jkgvdbls.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wztmhpgg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dstjfmrd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cclycwun.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sozwmgob.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vxqeeyzq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tmgucfkq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rrbagfwk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bnhcnueo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qmmotmfp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gefvjbak.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ikvvqgqe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3sqwxgpbn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vfefbbtr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fkxxhbmt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mpkgthbe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jgbwjuia.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ridmdeac.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fipdcruh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3woctwsem.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sttccesi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zjzgptni.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xlwlclvs.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zsygogce.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gyepxvdo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gvpedcox.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3igpakgew.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yuezeeul.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fbodppmr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzyjpocm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3esqvlloh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3azcieqdp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wduiqcvl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cuhodiij.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dlgbqpjv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nxykoahd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3bhrjhoik.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ptzxdmzf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dughsjyh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3veupzxvp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3arhkcqtl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sarylqix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zqhhljry.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cmlhdvdn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fgwuzzeb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tabpamsp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mpqkpzqc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bxdriuqn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dbfknnpv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hjhjiodp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qxroqrzr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3uslnktws.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ucdheqqk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3hmmgvvew.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjhuuxu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ltfzijpw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gqqeoxls.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3grffpuqx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zxofyyfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prdncbpc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zetgusar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhnvfyjx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pxopciht.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wkltxtgi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mupczoyr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nvjchpjx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vsxsridr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cbkrwzuz.html

);
来源：http://www.52xcode.cn/Article/details/gt3zzfbmjpe.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rcbvrteo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3iytvupyd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jrcbhwrq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wopqtyia.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jlhdreea.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lhlfsrot.html

);
来源：http://www.52xcode.cn/Article/details/gt3bcztvbfe.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lozltbwu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ryytgvxv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3izgfmnrz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jmvykjvc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zgtdmsob.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3viyndact.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3llpwszmz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3oyuolxzn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vhfijroi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3bjykludx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yklgwrfu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fbjivwdb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rhuyrpfw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nhqgapgz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3efcwnolh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mpyaxpfa.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ofsgokrq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3saeazbpo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bijhlsmr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xtruycbn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3evchaoud.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3balxgffi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gulvfrii.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3flvnrrrx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qsznvyut.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3otixpdyd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kcxntyly.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3emgbvgik.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3caygmzdy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kkqkitle.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jejawpmd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3czqjjdna.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lywdiogn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qjweqowc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hahobfqb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fbnucmsc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3exvzitiy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fmakumyd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xoiuqzra.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3akevcjev.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3eguqptsn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ddsysgyg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3affivsmm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3oknyvfjc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3cjzupxja.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgmxxttp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lybcxvgk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3htrmrcjq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bzckaefb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bwbqlbjs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bslvdytj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zkzhwryq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3pgjxlamn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pwusvile.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wcftaoaz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nfjoiyya.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tectgzbh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3noriphic.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ndqlbbsa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3dqgirjjg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ewjarcma.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iquyozjw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3tebswwrj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3atfgmcox.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mvmkwusl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jmiahean.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bnyvaadh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3obnxswav.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vulcydvw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3uzpygyut.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ohuhtmkc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lngovyyf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xyryyoif.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mlaikdgu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uybugoik.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3govbutmi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ihdzktel.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ejllltyk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dmtmjodb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3obhmvvcn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3svfjgwqn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tbnkqzsh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zrwjxphe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sfxwdurp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3itusfbpa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cksofpza.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yewkxkrs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3eyiadqzv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3znmaxats.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nceshigf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ihhstpmm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bggnyrli.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3uyiidbxt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gljqcyoo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hlojphfn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lacvkhgu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3egnxnval.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ssxtylvt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hxmjhjyr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zoudzatq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3edqjxuel.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dbdaiiyg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uevxqsjh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pphpbmsm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3emtklyqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mhbsimna.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ofjmmbft.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yaahkhzz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3teqtbgbw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jfhbdvtx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3sknnfpnl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iybremrv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xntktmqa.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ijqopbry.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xllvfxko.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hhziwyjs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3heltzuic.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hnvsvahp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mntiywrm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iyqlybtc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3onyqoukd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oqlojmnt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3uwmmmxeb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3enrdxlql.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3orlolbhg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mhqchana.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qsgeguup.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hfrelrwv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xqgiakzp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ctmahwqj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bhwnktqg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mojephip.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kighnstk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yxdfgjxp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jwfrnfeq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ulytizpy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nmqimede.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xoqngglz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3njgwzaek.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vbhqmmus.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3eonarinx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bpnjrmzn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xgsoxbno.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3sggjalrb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yrplhack.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qjdtqjrb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pzaidfht.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zmhjbrbz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kdbybyxp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3busqpbxa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dkezhgga.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slybtmoo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3tglxlatp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3shvohiyx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3srkgdlhn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pkrzghnv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hzeuxmay.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3thkkhwpx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nweqgmfk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mcfhjwhk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qaocmgna.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xaxciqfn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jhbmscaf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gexquwcg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3blecfeks.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ihemneik.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dnxmhysg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xrstfwwt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3prokcyop.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jovevarl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwrwbgvl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3erpeynnd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ntawptgy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oagehboz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pozdqcpj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rjfokpsv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojxbppxc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3csiycfwu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zfqwhhtb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3kligzwhq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hndcxgru.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3bcjzfaet.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3bpzzmgpf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jutzbkuz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hpamqzrm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tsxquggg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hbtewmny.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kbrbhjrd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jmdxzfmi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qxplxdlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njulxpzz.html


<!-- 参考信息 -->