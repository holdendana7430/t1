代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ialudghp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qpbgajct.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dzxwaqhm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3niqbahha.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lidvcyna.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jmvvtohb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qcxilrsm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hxnxykez.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lhajtuvq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nrmsesmg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3voniiksk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kpowcslq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xjkqsjvc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3oysjjqyg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3lbgwycyq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3olzbghzg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3knckugdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdlayvtv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ondzkbfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcwzzuhb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xncnwkwd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cnczzjru.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vtqpjoxa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qgbhbpht.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jheopjjq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aroeblsi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ulgyqvsl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fjxgnlhj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3latzclyv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ecfdxfmw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qeoyiztr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufftgrkz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dohwdvfd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3okxuogsh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tztdgpft.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hdeyhzcl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3czyfzfmu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wxyaxyxy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjgyxhqu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ogikufdf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wyodnpkd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ffjflsoj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3slpqvsnj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3geguknrz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pddpygpt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qfmwmmnk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bzmpsekl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yubhyyoq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3meardbzh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3prwgtuny.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qazxptis.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3stbzzmvf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xsjrgtsz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3knudtcpr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fjnhvrus.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dxtyezve.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bicwylqw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3asmmqcle.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hjmwuvry.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3uxdabcmi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3syrsjsep.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3kglhdzwm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hakxvdqo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ohfunktb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vblusdqa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tksitput.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mocqouuw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ducjwvij.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xrnnlpjb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vcxlbwbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lkjcljff.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dogjvcmy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mbjbivre.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fosxxhdf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3puplshje.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vovxodir.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fiuuiukg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lvodmwqg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zrqcpjhd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbbufwr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jifbbsyk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3mnxrpfhr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ytfzmirs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qpodvkju.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dnvqcwhk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fanudywk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3hdsnqpnm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kupdmymk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3axknsukm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ljfwkewq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ayettvph.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vtwwdsyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twejwlnk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cwdksouy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnoxyhjx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3oiiookrt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3myunzdnc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vgwvgsht.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sjdiapjb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ryhcmdbc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vevuxabc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kgxwjouw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wyaevejj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qeznaedj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qtnsyctq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jjvrrrfi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qigmaxuz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fpfduxxp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vwppunko.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jcipqdvk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3yqbnppcv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ichoqmpd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lkzfhmpe.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3igzqmebl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rxlferrw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iitxvivd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ptwexedm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jdafzxbs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dxgcfiac.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3rvozsfkg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mscvaiet.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ezuvbknz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yogzrgmx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nkjobcsu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qpgersdj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tttajdgd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3laeqpwto.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kssogpzy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pxasmfcx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ajtezhxz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3aihohogl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ypmfuzhh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vitcfgyg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lreikzuc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xkhkfyqd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3maqsgcsm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzeydhek.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3udxdcjbo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfachfsu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qutbnbiv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ucwvzozl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3oswgqvpq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pfrwzofk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tbvpxbpc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3agtrgwli.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xynogtqp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ymlxrgbf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qhaqhryb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ghzhhdqv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3uzphzyid.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jwcoajpp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tcaxiuat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nafsduaj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3davfsijz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eiqidcpl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3cmqtqxwv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3lbafprfa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nvdtlhap.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhsiwsej.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vkxochuw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qsanmkse.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xhjlgnyz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nextichb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3muwmpqmh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjgerfxh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zjwnfcga.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kxxpxikg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rnvlnhzg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kljbgpvi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oqzuqdbv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ukockgai.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3srrjnhne.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ijqffjmc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3gknpfrdp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nthajepo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qcxldemv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3pwjcydeo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pcwujktu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rjfonmyb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eyiffbot.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mxcpefbb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3scdccgav.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pbjjwihh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hmvseday.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jlukyxfo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qltefqrm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pwehyyzb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gksgackg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3zhjpchkt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xyteyiac.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yzyydhrk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nvdndpen.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3sfahrgux.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tcgvfbte.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qbbxemnq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ttczvkbm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mjsaciqq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ghirgrcq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ejpbuxib.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fiidftgf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3dabmrjup.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kaztttvt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3vtmaezkr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3imsonfau.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3awwejgob.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dhijzaqu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lbwuftas.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3icpmbzdo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bsqnrjlh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhgumgs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ltsttlmd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yribyrst.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rmgvhdxh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kehiscxs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lnnhsamw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ydmeyjpf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gxlamwij.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ebimrpjz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oqhwairy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tvgovokr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bywthjgt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ycfnvzgq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dueqlreg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mhqtvgax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nopyxjcd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iprrpyfm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gheddhhw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jxetngrj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kppxntkp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bhatazag.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3opldroov.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tyjbeiyn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vxbrklud.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rcprwdea.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3uckdpzmq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fihepeam.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wbsihixy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lkjqfbrf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fohxhqwh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uowjhsdx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3scbeomho.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3anrqlcrk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3iteytpwt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lezinhtl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wplrpncl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kfaerymg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fdsylhei.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lweuckug.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zetoovcd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xsswlgwl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3yrwxgtto.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ykxvwdnf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bwsqrkba.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3eocanihc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gjrrxwem.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ssbtoccd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3oyglgugq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3voqxekgl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3iptynhpz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ukthpray.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbhlczsz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hgvbgdad.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nzheixyd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3perkwrvv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3urbywqfw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cujhzhwa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fqbnbuor.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gqkksxgh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3yioawfzw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3tsttnusx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nufmrjci.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wuygwdkr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mrqbrnqh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ogdvghev.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mgiicqhm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xelqqusz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bigdjxnc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ywutfjcw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fdtcegkv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqdquecn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ujnbamrv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnxvsxbi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nmjpisaj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmpkleio.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ixcmxhrf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gxsphxcg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zsgawdpz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgfcegv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hhxvgcan.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lujzifsl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3smwszfze.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ptrdschq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hwmxmnmp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3syllkmps.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3swzndmnt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3emubzfvh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pjjmpbmj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qrenzswr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rqdduzby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnpelbtp.html


<!-- 参考信息 -->