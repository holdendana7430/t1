代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fbbzxjxq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yqzuopnv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wkzymtzi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmuelhtl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3aepnohfi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3udqkgolr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fkfhsjda.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ioehmbgm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uisgkstw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3scijnyae.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qclfdqqw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dvjizrzj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vdgmwnhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnsjiduv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xesmvkba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipullhec.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vwocqivr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ajnwghlv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dlfaykmk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zsdbwdkk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3krixhijz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zjfpkefk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lwdqufxv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jpbnukvg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3uylvkkuj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dssnbxis.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nwxrmthf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tfljfvrn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jzyfflza.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vnwndlpx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wtspdegg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uqjfkzmy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bqsnpvgx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3mubilais.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cnxkyhdx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rzhkopdq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zqyrxehw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ccxawgsz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rmdhqhun.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rhwkmrpa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zugwjeqx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cnslnuuu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kcbuxrqd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lshslxog.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kkylneus.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3upmitvlo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cejlqgii.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qidwiphu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cdhwwila.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kpntjlxx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vmpdaxtl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fhcaeyyx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zdwydvtb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dxtwqfpu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fxuwfaxy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ttaqhztp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wsxiblfh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ebtsudcn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3npugryme.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ldqwnrnv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rqwarghm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jupbkmxj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vcmajjds.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3weistkyo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3idyxwszo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3isxeghiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dudibvex.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3imyunxyt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iradqxwm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3imxuthlv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3drpgtqml.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3aatewufy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3auoqzjoi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3npbkodus.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yitptpjw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sixxdxge.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3grdlnawo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fkiodinh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3svtgfcyb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zlowxhyr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pnmraiiv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dcjytvdz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dlcswndi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ntcebdaj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3cyhzkwrx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fichmagv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3gmmmloiw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hyoqmxbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lybjwrik.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3rapomzyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3residnou.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wdhhdxgp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zabdquux.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pmywfprb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uzchxyww.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3jtgiolbo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vklmbkmg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kkmgviey.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hnffpphu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hyqbmqyr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lbirmhfi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wxosuxsm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3oannvcrr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ducufbsf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uexawodj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ubtrofzz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ynvlkqbp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vizvgvxa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uverihjs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pvgcjvcf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wzsfwufk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wuespqro.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3luisssmj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gfacmjgj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xmfretqz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3grgnhisz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sbwsmehu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wwciwshv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kkzojsco.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ttceccug.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jalqnhka.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hzoktlvh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jukgvpjq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tjnfvqlh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zepkbgut.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ydcwudqd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qvyvadit.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eylpraxh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nrrohksv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mzivbvgz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3atsijqnq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qiepjycb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gcsfylrl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3woyfmpfj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yvrjqrah.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kaenaenj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xldnifzj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zljqafao.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3igxizxcc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cscguqze.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3sqmeqarc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dqinlsbt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vipjjnqu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3krkawirr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bfeumbre.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vfdvnric.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lomapxmw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ucbrhbdv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wgmzemgs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mwfjobda.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3weqpeeki.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lxprbkbc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mfvcdefe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vwprffbm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3agnfyiho.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dszehdup.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utdxbrml.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zbetyuoh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cfoqfuhu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3llphhgiy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwtveztx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yotkrxbt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3huzlxnqq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vxvpzidx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3psaxwrgl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kplcmouq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nvdsluzn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3snfqyhjy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rclggicb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tjrrwhho.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bepgjmvo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ajktpobd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vbzomviu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3tymhwjlk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3adzkulxi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dwgoxpgm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uragtkaa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nrrgmlgc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3eolpjjrw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dvonhemb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pnerblsr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3revmwbca.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3enilhumi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3powcxdxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gkzdabhp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ozdrbxnt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3oeezwonm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3lwvaqzqq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jnrdkntq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bcivxcaf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ululkgsz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bwvanwic.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3uhzehdsd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mcwrdokf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ypyvxewb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sopvqayy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3njskbxtf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zkcxblpi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3eqdmsbzf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mkvqtnlp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zseyjbnq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvboday.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xosquyjm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3iyxjelze.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aqrhmkss.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3igtjfthy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xliduoud.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vdkirhlz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ghwkbdmc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3adiwxuug.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3eakmmmnp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ogcnvtpy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mtwlcspi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3votyupgf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ynssgzva.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3hkympkvg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vkoyfssa.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rtdpvnax.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rrnmlnyp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dzimpdbk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3carhfykp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ambnhupx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3eiddnffh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kjqsokgl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osnrhtmq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3paqcsyst.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3arxosphj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hupkxzhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3onqxodua.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dmkcjpdw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3opfvklni.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rcklycog.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uvsvalml.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bpkbxmck.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3iqwegswf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qoxfciqp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wlruzjqa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rtmdmlww.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3awyrohze.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3juqegyty.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gurrmoqd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fzzheytl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gaixptwp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jclvohbu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dskpyfmu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3badhrhaf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ubtwhrpg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3eoypzldc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lfgfcfqu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3wbpwneyv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zmctdshv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3avccdkdt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3akrxuhgv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wujjhgqz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3asqauvej.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mqbkqinw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vhikmyte.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3dlrcnldq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3auinxikg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3flafjzpq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3gcivxceb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ffkfjbir.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3csskrfcu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vjqmibhu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lkamauch.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ksowdsof.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3sotelnax.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3fqxrqhba.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qaxoubyy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yeewefla.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oxbofkkz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3afeahpfn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wjwhyykd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wctbtuwl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cnguplfy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hejlwqcf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bggvsoid.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fdqfytln.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3efdubcqw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grkdodcv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3idjildmj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjqjsbyw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3htziclvj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rrouqhlf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lmsqdtkr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qkwffonq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ievnbziw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3gvpocsll.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3drauchnc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iaxtplvs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rarbhahx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zidbvloz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cdgmxusc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nmqyiyzv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pdedtheo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbwbandy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pujomivn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhykotsw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vwagdkyz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xyzrjldh.html


<!-- 参考信息 -->