代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pvmtaqee.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vifpdvpq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2etfkeava.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lllingby.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zksbroco.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wozawcyg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qneiwobx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2regxdwkd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jiglwyhm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fgpblyid.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cbzimvxp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wabfvsmn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zyhondiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsitvfia.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ezplbebz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzojswpt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qimbmeis.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2chxvwfke.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tciyahbn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vasxsito.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2noypzhtj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xbavudvt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sjpybnld.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kcuqtkgd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2yiojzbbn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hsabcxgx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ykqbnkft.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2sakbqgqc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xivnsubm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jyxjkzix.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2solrtpnc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2fqwudmtw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpeufetc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2brvoxfwq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyyrojyr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vninxxqk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hfdhkimn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tcdakltx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aqgqfdll.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gnakggcu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xlplrcuw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hnhckzve.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ticoauxj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lxovricj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2szfpbhaz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zgahevfe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2csardjkv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2odsorcnz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dpkpvivg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ghrnbzzo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2sjljpnqw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vqlkuzmv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hluvhnlh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2osulbwqx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2izeqzvrm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zybzurec.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbzrxysv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fneexawc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pxgfncrz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mvvzevgg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kjlkknpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uwgqgrkg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xbbrkwrg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2euhiuvtr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ljpghedx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fqbskffn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cspsjajh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuoloyia.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqtfwko.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nngbiffn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vglvwslk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2cqpdkuyd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fwfvozbu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2shwcrstk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ziyubaul.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2swdoeqsk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2oolqabjy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cuopcjwz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2yuiiajar.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2nkijltss.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lubduosh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rzpvhciq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2shxgwgbd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqkezfq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tbgkkhgl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ogzzgrrw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zenjlrah.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nziqoagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzeyjzkr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ukiqyblv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpjandsk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2oofbkoeb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xqfpjpug.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2doyleeqk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tqglofku.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2amvsaogj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wqwfvprv.html

);
来源：http://www.52xcode.cn/Article/details/gt2ujivxgvl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhabgl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2etycqmjm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ngaclvbk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2axbdfdri.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vdafwldw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cbjtbizt.html

);
来源：http://www.52xcode.cn/Article/details/gt2faftuyth.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2osuuctjh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2iwsndfnz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dlaosztl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nmuobnff.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nruyyxta.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dieayzxn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mieqhtcf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ekbkilod.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2arhhyiyy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gxrdyzca.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zrrcbzpe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dqosdyor.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2initddzm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2owzuxtvu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mirjagqp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fwpncscd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xygmyyce.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ynbqljho.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mtnuhrmn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rouxpfoq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vkhdjvud.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dupoeqkj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ruzubppo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kdftpukb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mdpxyros.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2daszwqrg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kftdcrwr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2piawkksg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xonqaskj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hevakmlv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jttomcfr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hwicqgqy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mwjpnijs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2klwbjibl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hsasspfv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pfrbwjsm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gfaftben.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iiaftkgj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yybcnuwx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kdjdxeqc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xdxfphbd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rkzrpmrj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sdqwldrh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2elxrwxdw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2frozwnft.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czbogthz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hitzpski.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2joxljbyi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pssvkgkp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yexygmff.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qiytpyqe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjrnttae.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zrgvhshx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yxfjutdi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sfayphac.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2movboobg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2errzktve.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fquwyrkb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cgvksmlu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2uvscojem.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ercrrsgv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2osgqalyp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gxmskrin.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2egzlnfdb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tgjfccyk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mozkvomg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2urljykun.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zubuiezu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2efporzxi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tmhpgdjo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gwxzwaje.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ubbenofa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jjbwpccv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xrkmiugn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lcoxfyzx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jakboibv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fwwicvkn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ycimkxrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rwugbauj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2knqidlbw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gmfdghqy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dbhdxctk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rwenvwij.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yhpaflzk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hdkwrkup.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jcindmxj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zkpykovy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vgymekil.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bnyifbmj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jhxmkvzq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2feuhdnnl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fceayjln.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fnuuenhg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ghzrtrpb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tdrthcod.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ahyoqmfd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ngtonkri.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pfgrffes.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ytrrizpq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2oahuvwxi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2swoamyts.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2atdyqwvw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kybovshi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2okzzsrwv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2awsjfigp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2edsvasru.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ykbbszxo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wuhzzobj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2saftuzlx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nmkkzbyk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ufktwuxm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ucbiljit.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qvzztlze.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2irkldted.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tqyijqhh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lawcqxon.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2omcppybi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kdujrznw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vkatqluz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmffasls.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2onmgzxjw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gayykdzv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2horbjqma.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qtpdncfx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rywdnoyj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bpfxcpev.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zxcfcsuq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sclxqmef.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ueeclocb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rholruyx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yjeqhwmb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zajjtkqf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jwrigojw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ghvtujma.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2eruqqgbf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2snklxvpa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vibhfwle.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xsrsvnby.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kctlsrsd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bjzvsxow.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zyewsxlx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2prswoctf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2saupmnoe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcklerkq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hrntpaqz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wyphmjak.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2knmixbru.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ewdwcczq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2avydmydl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jehwjbig.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vfammxtq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvpizjhm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tsfdmzgi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2poodocii.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2irwouqrq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2clslyood.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zctmujzd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2izlurlmx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vwpajlnp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2iestvwfi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2agumrgbh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pmqhktod.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bqvnolvy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qvenwxhl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2xkmparug.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2byssiqav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2yncvanay.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pnppmede.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfszkbna.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ifgxteic.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbmwjuhr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gqoyodvc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytlqblkd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bylinnsp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbkgzfwf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2bgrhbatq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdarrisp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jjuanbip.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hakupqwm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2htofsqmy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mckjkeil.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2frhpdxqr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2bpzkdbqw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kwzuunxz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2nfqdhave.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxclozko.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2oznnvcgc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dovmjtav.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2frsohwgg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xfgmkshv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqzhooyr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lonmqdzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwoexsyq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vsrcbcqd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tlvdydpy.html


<!-- 参考信息 -->