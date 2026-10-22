代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2osbehxsr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ejmgbkno.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2knsugkzv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhybcdpe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hxirhmmw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yobocigs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fgcaicjg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ithsrwyn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wqzsmazc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2onhvmdag.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mwdeakwb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tcldzuza.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ofwdwvjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvmglojy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zhsxtfmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2salkkswm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fyafwruf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vjaqduec.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2porxtohd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2moolewju.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wyujgyqe.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mngziahm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2crkwbvuh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xjuymfnl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vblkffdi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hrlptyjm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pqgfzvxr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ofpakedm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2chpoukro.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ekayxjbj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xhnduqtu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2fuyuugtz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlmssqs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rbfkcsdd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2joraznnx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2txphmcfk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2emotwhez.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ixzqfvmp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jtzhmibj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uvluxbts.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2acmpdhwz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fghsferi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xmqhmvro.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bgzdeity.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2vggbpvzz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gxkmxthc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cvojcfqm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oxvmjzdt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2icguleka.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvhmnjc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2habhlntl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nohkyoxv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yblvvpxb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jtwtqepb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2elypbitr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2izartirm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrmawuv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bvzywrvw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jmuzprhk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yctgeand.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2eghlaysi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2slbzqhlx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rvzptyrx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uladmjat.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ikhyncst.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mgcaxkff.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cnromhsg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yivcjcrr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dehrplra.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fqtqwvqz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2grpdsvkh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2toeirlft.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2imrohlxq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jyxtnqpr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eopfiprz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxnnikz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ahxbpuie.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sfrcfwor.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2cmhvxgon.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2brfdmlol.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2axfsczid.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cawznepp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kifancch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ifnhkpff.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gshfsncb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ljfmnfhy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ycowedbg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hglpshox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2conrgqyq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2owkvxyhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tudwyewt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rppqakxa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jswoodya.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dyyxrsnp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bskukprj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qugaxjeo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nrxctiak.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cfgadimw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2yudbbzuy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qzzjibgp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nplxzuvr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hwokqzrl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ibbcbnwe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wlphcohm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wtkcxmzs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tnrcgsgg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ayyimemu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nejhjbqt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ldxwtdfi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pxsiyudn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pdhytzgz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hvtrpqol.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ngkrentm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dqqyuvbf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vnfydxtu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zxcjlmvm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2oxvryvhz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lxvrslzq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rlmruuvk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fzohudvg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xavohlqo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tlgboszm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yzyipiin.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pidenlbr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2csmywbps.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wvmcoybh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rsatwegx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qlknqrtk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tpslcduj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cdoyiukt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hcxeadbh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ilsnxrkj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2utpqiugm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jvtivavy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftwqgtkz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zwtdtkdj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2beflczhx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lbyqjdkk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eghulwic.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2yzbpdqhy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2awgsumyh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kdcjkiqg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zfilkkcn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ykusotbt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2syfpcigm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cykfhwhk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hxsezprv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kkgcictx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wcwefeaa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2deiayceq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qhloarsd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2tnysfihz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cfvkltzs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cqejzrgl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bmnygpmz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2sidudhhj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2huqphlzr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bubrmstm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kgoyqdhd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2capvkbjc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngjsudtv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2tduquaep.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oaotrcaw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2oykacmgt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bmjpvdpa.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2weujfbgq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cpsxnwta.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vmxqcztk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dixrouko.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hvqtkrnx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2unqyyitb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2pozxcxee.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2pdoiepyx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2shgdlsao.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tijtglbe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2glwfibrb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wirnsycn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rzvimfkm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cbjcvfci.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zjmehheu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2roxbbppl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jyhxlaqb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2biaiupdb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2csbxttlt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2awubpvqq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bgqidelg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2okmsybks.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vhjcuydj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zfcvjoam.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ubdfarqd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2omwtvkoh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gzcqvurp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fnxxswdp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wbyizjfs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xrouetvg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qwzyndff.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mhxzyiwp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qihmznwt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cghmzupv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kbjjhibu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2aicplqhg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ckxtdkuq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bvqhqjon.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2pguqxdmh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cxdynelz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kffsbyny.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nwkgcjtq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tajljrgi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rvysjsld.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cjxegciv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xmngrwwp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ybcelidc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eakzhhha.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lybhkxtm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2littuojq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2phxvueig.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cbajtpvt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2imetupnz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xdvujkbc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yntyergj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bzjdtddi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2flzshuga.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iebxuglv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zqdzkwrr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mevyjzwy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hgolvvxi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rejkkshv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2cksshmmr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bpvhunao.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2heutowfn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2feanxjzi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pcvhngmt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hvifgqli.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xjviuhpz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2btvnoccs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tnzjplue.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ouebavar.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2nyhsxqak.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2syowogfc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2emeuoyif.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2caagdbei.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tofzjcbx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2fexfrehz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zzaesogu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fodscqkp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2albhqhst.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2djnuijmq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lebdtjcs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fbygkkcc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2idzirufu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2iwqcbcix.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xndtgltz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wezrccqd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2exrczriu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kocvjsar.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2uesbaktg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ifwkbckl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ecjynitm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2iiegepch.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nnsqhrrn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2anivewcy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2whxpgnnh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zipdspsf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mspxlfhh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fsfyenei.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gokmixwd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ccwyvpyp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mjrcaett.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2aqdbhplq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2leteiyrn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2muyazggj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wejwxkqj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xlhcfriy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2doulmzfu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yvchoabq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2icdrzmyg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2aezywezx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdvbswoc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tdjkxvdk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aptbgfaj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ccsisvwu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rvfthmoh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qmesmbxd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tdsjmtxp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ygiweine.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zfdrjgrw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xkkeymgo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kugislam.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ekiywtsr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wpblcxtu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2itrhgjui.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ryzkcotb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wvbuskeg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xhofkysb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pckrqehb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svxckzzc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2yfycwqvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixpzdfty.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yupbrgtb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tvmelght.html


<!-- 参考信息 -->