代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3efsfrnih.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3afbdxnur.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xwuwwgbr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwfhltvw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3smkebmsf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ekapxjhj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vyhnpnop.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ldydnqhm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ctcgvgxs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qzbyjsix.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3onuuzsvg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3eenmkabc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yxrixrbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jllxpfdb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hncwnclh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyfpwdil.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3umjjisrf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3edjvadzf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xkklfdzr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qcsycggp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xavzqssa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gqlewxqf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jqqgkwng.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hfiwmwzy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qabcpfmx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3bebkomyh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oaarhwpz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3erokjyaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yjfgmuth.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3uurxjwgp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tmybeytk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vcpzpthz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tcyxerds.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lxopvqay.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aivccwsc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kqclubyr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3iozboqzl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3strdmqhf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jjmtkjyu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kvmmdskq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3edmltxve.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kebojqjk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3epsjknvz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qdnrplng.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ewsriano.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zrzeombc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gkyouuxo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kywhhxwp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ngotvyxy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jastoffw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dyuaocnn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nadaingc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jagwhtcs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3svdanqcb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gzdnrtol.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3etiusryg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3coqoggsy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qkkqudmf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vabzrrmj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zhxvrwzk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3klhgazrx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3agprlumb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pegkucpw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uqrbbagw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vrddktkg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hjdeglhn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uafvhlyg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkorlpzl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3pmuvraqs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3btgikflv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3sdkfdowu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ovryypgb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ggvjryjt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cydhurnq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rjgxsvjw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ipyhvczv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qrykarnj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3khhjqyts.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lxpeyljy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bibbfsnu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3psdyvdys.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nbhvyfjw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bgyrsdei.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dabrpfpl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rdzcvxmq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ggqacddt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3temcelux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3epjruzzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnetmfvs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ywwdrrmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgkuklaj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3crriqwri.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fyorbkmj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hpfrwqdo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hftbgiox.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mrbzyngv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qtybanwf.html

);
来源：http://www.52xcode.cn/Article/details/gt3yvrlanxf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ywdohrnt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lecratle.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3advfmeza.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lftttybh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qvldzmxe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ciakkhim.html

);
来源：http://www.52xcode.cn/Article/details/gt3slszcwcj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3juvamumf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ojqvhcff.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3njbiwtrh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3llfyygrg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mmawaiut.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3awbhqzhg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3inrvjiky.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3grokfovt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xztqgthk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3eviaflmq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3rjrtgrqr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kpqjzasw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3aezzrjgr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uatytdph.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vttksrwc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fdpxvbzx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lmtriomz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ktxgxyov.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jpmcjiqw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pmjzcwif.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3brkhbsbr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yztpoxej.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gupoxmzh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3uwwdrylc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3szeiofjo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bhygenso.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rurziiza.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fsfzgeii.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wntpgdur.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3obkfmcwc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rursqjse.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fbuwxpoc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rbloprlw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3grpgzsdw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pvmbmcnd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ziwskzxr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nnjtcica.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ajmekrbv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vhedxdfg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kmmlyyej.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3icatshvg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wnnixwbd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3mhfzbhmg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ehrmgxxy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qdqhpxho.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgbrgaus.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xwjogysz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vuzgnqmq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ktybqarb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dijezxhz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3txyfcoho.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fsvxfdxe.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3btrrythw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eablzuer.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3syixsyom.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wixslazg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xifjduzj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vpinmzxs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3endivjfw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fdicjuap.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vmjqlxnv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fmgxhnuq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jjprcvsg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jcydrtzf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bqzuzhkh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3yhltupji.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3feaqvlcx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3knhippsg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3obxmdxcm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kqcytkme.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fxmtctfe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zoqrvqpg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3frjjpwas.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pnstqgas.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bleaobga.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tztbzxgg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gavzkqbr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tcubgycx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3sgrvjvqm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dtmxighx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rzqkddle.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xcegutev.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sfgdxlnt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3rbmjnwqj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ipijrvji.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oknxlsha.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sidcmutm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3luiynavn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dzheiluz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3puqgpynf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3butcngxm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lqsuwxbz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ziyilubz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3npqdnsam.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3csvwulap.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nsyydawj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxlykpc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dvejfyig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3iesyjirg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3trcickyo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ysnurmip.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lndxbhpl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sdkpslro.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tkrkdnzp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gmvwpqpm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gltyzfyg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zzbjlaog.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fisbjiih.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wstmkopb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xinwrqxq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dylizvxg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wsyqecuc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3frtjljlv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ncvlyoks.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xmonjlff.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aptkuope.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fovqecpy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eqazmbec.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xcfbyfnf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bahplxgt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3llwftkxb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tzxkdctw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3evxjwuho.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vllgbsqf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3csnujbph.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vcbggubg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bwgznvpz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3woeqnwyh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cxfucvpp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lbqxzfld.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jfdedqax.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mzohhfss.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rbzjwvbo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kpykdzaa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gswpfsdt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zahfplbb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vslsxnzi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tdhoyjdz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jebhzawd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xijgppcs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3acimagdd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3owvtxgwb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xrqsiukp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3grhpqirz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dyksswhv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zaycywcn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lmoenvrr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fmopskrn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yyxcusby.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tnxeurvs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3onrfzqwg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mutdivdt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nitknjfj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xdprwycv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uiynztyx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qzzjqpnu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wizqdwnm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxpkasjg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3svquhlcq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ovfdhjhc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3blwlfrcr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wqaarnjm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3iqnzmdcf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bdekrajf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bchcmoek.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3znjccubv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qhzcytpw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rivtgrqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrgxpuvq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mmnctmjv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sciipakn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qrudcvmc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezohalni.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mwdccsbm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmplxaxt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3oonvhsrx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mpfykejq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vxyyytdm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mwfxzenf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3eovqvlqd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3addhvsdc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jqgczeor.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nfnpzdqc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ojtxnhkz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fvmrunja.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgdyomft.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wnqhkpfx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mehbpmot.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3sjgquvnz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iamgwmbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekmuzfyx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ijktxehp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwtfqbwm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kamarofn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3idmpbgvb.html


<!-- 参考信息 -->