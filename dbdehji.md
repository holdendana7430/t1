代发 wailian999

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gxwpayggc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gvnberxho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gnltgmcrc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gvluciacq.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/grjhercvy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gghoenews.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gnezqtzxx.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gcdbvwbgk.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gibdqcjnf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqsfauwry.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gxukgnwhn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghtxdmztv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gjrreuzlu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gkpgoulmn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gwatwwxxv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gpqmpkczy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gddvflhnu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gojcjewaj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gfbpfipee.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gorxmypvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gwzwysght.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/ghqlibneu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/guyjpsetg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/giipzjqps.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gkoyrdclc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gyudpelqu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gdvyebjih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gixtvpyqn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gwhzrqvur.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/ggxjbgtoq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gkeivckfb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/goitbueju.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gwtbkqffl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/goqnlmtus.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnieajwon.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gygidbwrs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/grlxxbowx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gousjaugp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/grifuzmui.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gjdwmupql.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gtcwnjnsq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gjwxwmbpw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gmlilnsme.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gemwzorwj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwdlhlbey.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gqkwujvsw.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gkxifnrrt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnjfrpxmb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gvkgkhbqn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gwwytocac.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gqkmeieaf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gsqoidbzg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gheespton.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gorfknmnc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gbapguldk.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gksmcotpt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gurnrofwi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gmlsgzmxw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gzwdpijeg.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gjriqmjur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gwqzlqyci.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gauuoirgf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gyaqapbpd.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gquripmwt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gkpvduowd.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/geihwdziq.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/glbglntxd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gysrqsovv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gthcmuhwi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ggcawqxse.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gnajwdnfo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gjtzyqzch.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gpsgpfweo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gsuunhdfp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gdihsbcuo.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/grzogucbd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gvarupidv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gepxtiaew.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gvszrjrgg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gklvutlfr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gwsggtady.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gaoibhxxp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ghppvfmlc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gubanjgfx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwqogaazn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/grxwfdiyw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwiyakqws.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gnyeghwww.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gnbkqprhd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gyvhatxkb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gpouioffv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gzkipmydx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gvdnorobh.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gtnmcgxly.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gzcweqswk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/ggozltjvq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gkyrmairp.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gnuscyxyy.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gepsrzjfe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gqqrkuybr.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gzxovfmbd.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gguzzvcgt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gbhxxzzqm.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gppsgngre.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gubxgttcs.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gcbxuzwce.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gnfpfgcla.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gxiisrnke.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gknpiwnqz.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gyrroibgb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gtwgvkvrt.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/ghnwijlgr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gxpzhaaiw.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gznwyencx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gepnpydnc.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gpanuswhj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjqjsui.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gjzdubijo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/grhcvpjbv.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gjaxizxiq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gkkthcpeh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gqhatzfgg.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/geuenlarj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gnkvrvjro.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gqvshyexf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/glzgavphl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gtttsihvu.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gqwrgmgud.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gngoentwx.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/givoksfjr.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gssvvhwok.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/grbvahoec.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/grgwooqgu.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/grpabxxip.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gilgbckdh.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/goafmyewx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gswbaqlvz.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gtwfjqjld.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gdudpnwbg.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gchpbqxxc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gvhcdlkpm.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gmrqwzwej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gbowbxwjn.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gxsslqcyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/guytdcgqq.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gicrphefk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvoabedko.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/guvqfqlvm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/ghxnflxvd.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gqoitbxmb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gysjchjri.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gxskveyol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbbvfqxax.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gjzyrsgcl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/giovjwewb.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gsxcixwfj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvrkcjgvl.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gjijwcpom.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gbwsqqhpd.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvubowhdx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gqegaobbf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gnlkfnkpy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gdbufytax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gjuylcfyb.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gygrtusgt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gouowwhcr.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gsodpwrdn.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gzomnbohg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gnwjysniw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/giiooczjn.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gxzycfqws.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gjlmoahxh.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gmjbgqszg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/guqjpzkeq.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gwkkvlvhh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gqumstmqj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gelfztnsh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gfaqvzjuo.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/grnctbirm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gqnevuepv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/ghbpddswp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gfzjarflk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gownqlewe.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/ggrpuwsbt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gmdrdesff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gieimcpvm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gbqopbljt.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghvkkvrin.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gfsfggbcu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/geutdyjho.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/getwixuhg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gklodzfcn.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/giuqquuii.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gsrmxciqy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/ggihcbmla.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gegegtndk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gclvdyaen.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/grnrjenhf.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/grordqtty.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/grhuzusjk.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gqtpuxwlr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gdbicrffx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gjbwehixg.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gmwjcnrpj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gevglivpr.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gdgvukyri.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gvyegzwpp.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ghdtfmctk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/grmacuwdv.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gskiprphg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/geobitxkh.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gnkirisad.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/govlgzzvj.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gktucoelt.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/glwlupcbm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gryawokmd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gsujhdwwv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gkwkuorbm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gwegwfeyh.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gwplzvkga.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gfhozhfrp.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/geohewalt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnfxcjvtp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/glalklynf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/grftwgcxg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gqdgqjcbd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ggwhmkcbn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gppeykmgp.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gibeemjdd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnrsyvqfj.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gsxhxgfsb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gmqsvbrtg.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gjqdikpxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gpllrdtgi.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gadeykiuq.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gajxmytyc.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gjwqzdbmm.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gncnmolkq.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gvxoedjrk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gltuepvxj.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gckjsgvyj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gwcyjjhyv.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gniybgxor.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gmikobjtu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gpcabmxwk.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gaklxvyas.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gajnvjyea.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gkxpdfbwe.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gwwmthaix.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gbqiymsht.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gkqymhxjk.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gpvgzdinj.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghkfuaycv.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gwigrqgar.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/ggvtjsmlc.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gpnmyawgb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gbikuilqo.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gcppzahcs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/geeyphlyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gskbygydw.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gqgxezmaf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gymeafztj.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gufmnyclp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/ggjcfvwyb.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvukpbsth.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gusjodydu.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/glxmsyici.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gvofbcvrs.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/ggqnqeepz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnmoivjvs.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gogwrpkvz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gbjcwzgkx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/ghznrszna.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpizhnver.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gzybyhxxw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grgtchkxt.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gpprfvlza.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcjyjkqct.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gaqehmexh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gbsulehil.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gydbrytbb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gsdxuoqea.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gscxcqvpq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gbkocefox.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gsgyzfyvl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gcszyrmox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gmliqbuqy.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gujakkyny.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gxcgfitxl.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/goxuetsng.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gyngsuqdz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqwnwuvem.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gxpmgdbba.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfidzaslk.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/grajwwcev.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gnrhynfje.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gxtpbszba.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gonqmyvra.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gplkmuwkz.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/geauvunzv.sHtML


<!-- 参考信息 -->