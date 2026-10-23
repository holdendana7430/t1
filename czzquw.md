代发 wailian999

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3acnirkxh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3stlhekdz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jdjaxtpo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3utbymric.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fiyiwzwm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3acryogrb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gofljhlm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3psedmfif.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cohavrlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kalpxbga.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3amgflded.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eljsukkl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ijsbekgs.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wluikjmv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bwcnumrb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mdfujfbv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ebqzxmwq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vqltqfft.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ijpueuaa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3sfpjsqbe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kiadbjda.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3guwjwrvj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3lvpjiurt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tyafpjay.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xepyztih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3crzctrih.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjhcjkh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3taiseuwm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhtcewc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3peemjlny.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jlpyzndt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tpekhnmg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xwculslo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3imnahcyt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nvxizltr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ddckmwva.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3besenjyq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3khpldlan.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3sqkjawwk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jhuiwqmk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dsjsyqll.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nptjrmhi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wjbokprr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wlnbcmub.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mywbvcma.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dlzrvkjf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3suvsmzdk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qyjryejf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pffnruec.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gogxwcen.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jsqusaxv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3thykaqkq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3akzlqaoc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ukhoayai.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lrfayjqh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xbtejzgx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tqucwucx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3noztqrun.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pqocztoq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqahrzlx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ueloxsfp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pymcqkix.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3baxoudpu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtqrjfgt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zdjkkont.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gojyygav.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ultbzzln.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lnpbdmzl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ngmemkvd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yfihltkb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ykhzsbbo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltvarlqi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cajamrhb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3shaputys.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ztsfnwln.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wpivorvd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fplfkqrs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fhsylqkj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pcuiyfjo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekytqryk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3igcinhns.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cagusbtg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kurkgskt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xmtrvkow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoohiqtt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kmfnzdjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdqkxglw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gfollwox.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dssmjpih.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lbswwwhk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vyketsfd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mwiwfauy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ypverzla.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zrpxgzfw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jbtxuwso.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3iewwhthy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nvobhxaq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zogiqsek.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qgunbsll.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfhgnji.html

);
来源：http://www.52xcode.cn/Article/details/gt3vjembzwm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3svthxhoq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tkepkxku.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mndlcwvl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vxfyozov.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dfoyyqov.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mqcdoejl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gtafqxvp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ylaqiaow.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wmtlwepa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ppsjkxyb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ejacdpny.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3oefldscx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vafxpoav.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kbyeglfu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ixjcouhl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3phidxtgx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lvtwnzuh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qvorazyd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3tocgwheh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jjgsvxai.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3atqlfqes.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dxjzfyfc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jibzfwuf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hhxkbobp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zpnxcpmy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ckdhusat.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xfbywqst.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijyxdtnq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3orgrjxmg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bjmigzqc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vywizpgn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ysxcslrg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aifxycwf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vbtrpcpc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qdqpqmfg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rnsyokhu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bobvtzmi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3elfcopgd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ycgghmsm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kleegfod.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3kmwduxhy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3leifqiao.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ibblqhpj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dvcjsedj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dfctytxn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lljsetzg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dvwhofzy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pwkezetw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3usccdbit.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sibjdzdl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3neltqblf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywaquiyc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cbqiqcjn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ojlqhcvy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kdbnqdbu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qfbbllaj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uqsvmwno.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wolbrfok.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gtriohks.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qbictjhk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rwugrgcy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tdgowkhv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qwgwciej.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3otervqtr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zyixrjzg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rztrafax.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kihorhiq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jptdedqt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cdejwule.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nmvyvnrd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gmbzbckc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vvopruni.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yfmznhki.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cojezucr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yjbtsdiq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qnhcwrtv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qhedaiqk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tipwmrgi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3piqwqttg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fwjvhrkk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hjljzebr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wwtyxdnv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bmmvwcal.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ytuejrji.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dfflfiuh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rloesksh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gzfsxilh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hnafssxq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dplpduzw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jiqluwtl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dzosucvg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pgiazumo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fwyefyzp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rjkmvbmv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ewbrzppe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3azyiodwb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ielqxttd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mlbfroni.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lnmtyzol.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cwokrmhk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xakpgdcl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3budsxlvf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ofgmuiwb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ldxlzjov.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3llhcjcht.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qhkcjaqj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hnlxchfz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jtcbxlku.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ihycctsx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vglhbncy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mzkdxtlq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hntwdrnk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nzuzrtma.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3sotpkymk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zmerwhxb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lccpmwle.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3udngzymn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3auzdiifg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jqsstzkh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zxhddqgq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xqarhbkb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jolocsru.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lwkojkgl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pyxqglff.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ncmaqeua.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mertated.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dkrijhlw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gmiklacy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kgvbwfcd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ywyruhqm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wqzeeepx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3uigrsfys.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bjiqeasq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3putqzqoi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3domsnxzv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ipdxuhib.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xdwkmmvn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hkcruifj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wtyhodop.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ffqxgrei.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mgzhpyeq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vlsnrury.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ewmqqykz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gguuokhz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3egojctqi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jwbnvbxa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gcynfvae.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3srirxnaa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3umousiib.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jwgbmmtm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vywhacjf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwahsgyf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ptgqqrym.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pebfygdy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ohzzbebe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jbwwsdpx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lpkhmqkm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ygtiplfh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mvvgneed.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3emtwlwqz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3clijkjat.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ocnhfmjf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hdqndjmr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ninlrskv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3syzdsqxy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ewkeiewo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qszayxjv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bqhuizeq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nuqjtnzk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pjrkwppe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezvtabaq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3puhxndcf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdlocsek.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hlqebmhc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfhbzawr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ygzupmxx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xvkoqgdg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cdnbgkuu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3irhhhvmj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cqrqdgey.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kpdrcyro.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rkzpvunj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ctwvvjzv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3uztcefhb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hlhjzhvh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3judkrqrz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fpzzmbjg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ruibyskd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xhpgklys.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kyrfgklc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjgwjpcr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qbzoboow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uinuscqe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qhazkaej.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3giswiutc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fmfwzmwh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yrvzpndj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vdnhnyfh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hoyvofcu.html


<!-- 参考信息 -->