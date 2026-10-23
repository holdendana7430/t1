代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qvekihlv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hvlugvfo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qluvrriz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ldgadsrs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ihykwlhb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qxujauba.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ccnexofx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ntutdmdu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3imejdziq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lylsrhxk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jeecrdhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdosjcpq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3eiiojxxc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3tsnqfxfr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tzghgjjd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3trsyzwow.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dbtycilf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ibxildlm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3knhoqumh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tsanznri.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ijpfvsme.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ixobgvid.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tocsaqep.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjuidicb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jcdblcsz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3iulaooyk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gbnjiicy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3cfhffohc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aspfvtmv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xufysjno.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3icnjggrv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rljqutec.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lmfwoiuf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vrbnbshw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3leqvblhw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3dnqvykwy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bqivdbac.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lnirsabq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xvumibpa.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yqbtndmc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uuwhqnvp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jpycuiij.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3grmzbzbc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3oksoglot.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3airxkbgg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zngmsoar.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kjckgjtp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dzuodrwi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3nnflssdn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3sitdmjaq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3demgykdw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3syhwnybq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pyoavlrp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3zoizdtad.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jpvrylsp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zzzwtofo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3feoxonwp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ysjmebdu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3betyepnj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hamxzwkn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ofxwmakk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opssvpba.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewbvytjq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcmgmuwz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3igrgakiu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3aaybpxaa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rezkfxfw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xtgejxrx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3tbjmgvbg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tpgbyymz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mithufou.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3odxxkpwq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nhoojlzw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3grybxqzd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vxkzzfxg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qwzcakbs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hbyljvzx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xagflyup.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zyolqwck.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wuxguvyx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kvioznju.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fvjcwtkf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3aypfunts.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3myagfkpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbyzhsma.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jydhhpuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igsthbxn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3biqzsfww.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dpdboitr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lznnxpio.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tudgagxt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3eptsbptw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3psgzljoo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tdztgqlf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pfisukqi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bbpyvyyv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vgybeikg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uvzsypya.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dllrjnve.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zqvzntac.html

);
来源：http://www.52xcode.cn/Article/details/gt3qtarlxmx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gilloaqc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3otxumsog.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3njixlbfw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ctxtkfxf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3iecyasoi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vcqnzmse.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gvfpmjgp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cwwykrwb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rwdksmtn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qxeqacdw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jbfdvzht.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rbnjqmwp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ujzdjydz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tonxsuoy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3uptlrxag.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uicuyqad.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dxpokyjl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gcjbuagx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hzpdmdxm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xwlrenqq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pioltedi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3gsctngkq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fwrsuhgl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3glghhtdl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lidxfnmz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jhveyrwu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lenfajdc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iuzgzokg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pkzodtyg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nmzsbtja.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dqphuzbb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxblipgg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fhyspexg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kpiiygpe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3icakxklq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qvsbcdyh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3haiwssyw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3osbqluxl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3urrjsyjb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tmwrzjuu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qcljweed.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mrvtpvzs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vrlblldv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qufkeviq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3epnwuqog.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zbkknbtj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bzgpfmpz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xsyxxmdt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kaxunpvj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skvoqawa.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ueepetvm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxtpnjif.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zmrapwkw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ogqlpcsp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ixymtssn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfexpdpl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rihclyqi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3acebiiin.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ydhvhhdo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hbjvgbfh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jgcfopiw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gifgoznt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3uaqvdfsb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kxgpoagi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3baohkzth.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ivgbskme.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dstbkmoq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tqwtlind.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bycebkgm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mnlquove.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bvqcsibp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ulqslqhr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mzknampe.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cqwjatfb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3sxvctbgs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mdeotwkc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gkdiwafx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fijsfytf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dqpfyqqz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dumittqz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wnkyfvio.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fhwapqgb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bwneviqo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ertauqkv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lpwjpogn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3orctvpqj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ktlcpmou.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fuivglwn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pncmnssi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bcikxurw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pvjangwu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rtyjzltn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3egxcjsbn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hjbwhmsd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3frglkjkz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ejrgevyh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ogmgokds.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oltrdjif.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jelqiwmy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3yujwlccg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3nujlnukr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ihoowukl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3flvmrbml.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3umdncbvn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3aqkkifzo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dligzvte.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3irenielz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fycsljuh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gsuxbysa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ixfkdnce.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pgvajmpc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bdrvkptu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nvenjcot.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mqnkjxfz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mqpopcxj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3czdtobeo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qlsamgml.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lulzvdqh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3cfpslqnz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ygapjnqh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3pyhhvkly.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qtbffbuw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ayljzdgl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zztkeyrh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sjjfbhbx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gikipqxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pinukhub.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tjrqpygs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wnaoschw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3viwhkrfm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3detfdswg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xoygfwnl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ltvjtatu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3trmkdkxl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ihzhfyxq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3lbvdvpyh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jnbedjyx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3erbygnfx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mykwzwrn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fpxzhpft.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3svvopcak.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hrqkdjyg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gafdtzvt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qndpqzig.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ofoktcas.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cxjtefrz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xrfzjfik.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3osaabetv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wzzoswgv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bgjsowin.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nlufndmw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3odvovilb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fjkeyxvx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kpyyjpmm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3maqdwgxp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3azkyuxim.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ugpuinuh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bltzzlok.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rxduvqwx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zzhsqtaa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cgnobqyk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pntffzkb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sifswkrv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3azcjdknz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tyasnifl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3focuhaov.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3amojedfq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3etqopkey.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xszouevm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3osrcymse.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iyxwabhe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3albzjpcb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcgyczhn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ldhajtta.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytrncslu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3isnqowrq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3neetddlo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pqvespfm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cwswdrif.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zevdstjx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gpixbirz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3aryoxmsx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nhrmynmm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3swjikhsj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bbwloeyz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grecmshk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3cslscerv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wjepjaqz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xhkswzwf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gmwbduju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fviaouwx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tpqrbtdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usnlksmf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tmlpmewl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3nootorqk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kbximrtp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3grapldau.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hcsamqpn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ftwyfbfn.html


<!-- 参考信息 -->