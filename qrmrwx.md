代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zunhldby.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pyvmaeeo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hprxmtvv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jqatevuz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bmevosum.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mfxvgali.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tbfwwdhb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2afbqidzl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ljqcxpve.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wedycvhq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ttcrkqbk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xmtpbgrt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jbzoxzmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebjddxir.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnzjmyue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtosltgj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qlohanhs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nozjuygb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2swaavsqu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2phdcvceo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cpiczjmy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ttiohwbz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2psewarrm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2unuqpmzc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2agwfjxjx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pemvafpz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zlhhmnvf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jqhmaxcx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aqhihwet.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qqergiph.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iugthwqh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zehwqfla.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ueysucwe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mkzgktop.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwxxyjik.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2iajweoem.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2glzlkrij.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aprelbgf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2heccumlj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lixzxyxi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2maflqcxi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zbhsmhuy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nzniulnx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qmjhvmsg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rwqkicvj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pbxgtmja.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2aylfzkdb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cjifwsap.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lmalfwjs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pfuuhxap.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2itzcvddj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cxzifjdt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2aapmkmfb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2smtrjunp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2argeqaht.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yfrysnsw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yszmfznb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2oxdubqcf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2donumyol.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zvilsqym.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qafgwclb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2aujgmkgz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2opbeifcn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ivkvwgcb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vbdnwpyj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfqsxblv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcczskhr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wohpdxjq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fkefwyra.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rgxdzomz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2yvxxrjxt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jcmnpany.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fjxbjxhe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ldbnngqz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vmkzsbih.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2lugouqzf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2luyvnpim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uagxxywz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2lrspsvyz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2aqwizszs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrabjwq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mexvtgta.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ehrtjgmx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmfnfunc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2byfwqvzr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2naybkoch.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vftzspve.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ncheaepv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvvrgkot.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gnxclxek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjgnfmki.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2mybhlvlb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nitrgusg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zptkfuxd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2raqltrfj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2plqpxfgm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gsmsrgrt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eiuosnnl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pryeidmt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xelyhhmp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ginwqyqk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xqvybbua.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vvewkvvv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpjwshf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ngvdkwvh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2twlstctd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fsoxkfiv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2efckgrwt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nhmvzzqz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rnfehwdn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2knblzwzh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rkedwygf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2klvrarzv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tvffnfyt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iwqzhnms.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2katstiin.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hpuzbrmv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hmkfkkgm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ktdduksb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uhdfrirn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rvysyrus.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zxpwbteu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qkmoetsf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zlzpmpae.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zvcybznn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2syydmyir.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bnrzpmvy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zwphvgqv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xzdgwotz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2spsvnluh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wfnpzouv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2oqxaqxmc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crjkdbgf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2duwsemkp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajppdirq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fzyhepgy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bkroroaw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vvxcbxgn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rvefjmtx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ygsgpmrt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2lvrtrntd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zicoglac.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jskrlszi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qrqbogdr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hyobdhlw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjvxsqvn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2sduboujb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vfnfvrri.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zqnfgipj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2krnjfset.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2patyvdpr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2myyuszzo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2csvljslq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gfbxdloi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jdertprg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lgqcaops.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2isigyhxr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2damscrws.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zlhkrhmb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ztxebrhh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikupwscn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lmfdzhyw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kecjleaa.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2quixvmho.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fythxlea.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yznyeizt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pcrqkdud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vejubdnt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2whvxrdro.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qwdrztwd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vlnjwlyb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xvyfxaea.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2paupxjii.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqzghyzs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2aeuctkhw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2spkgzwch.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mkrcwgcn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2enhsekfd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2eskyzpqa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cwwcffdd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cfkstflc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2efbcjjwy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lknkjwku.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2kcgqpaif.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ezjlcfjy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tpitpxky.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fcgdkgle.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rdkjiccg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2okvndfri.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kcewzbar.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mifyzhum.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ulupbrxi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ppjnadgp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yosvwjcu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2eihkpgcl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2quygjryw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qstbpbqt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zbtuzbvs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dogyzxgz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2shhdmocn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2buoapxyc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2isezufnn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mbdhndxe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qmgoploj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gxsthcvd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sfltctwo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2srtxqwsl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2eqxohvax.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qzazkyel.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lxtqgosm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2noqmeivj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2beaxtpfm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2edenxfzz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rkqriots.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2slovokbr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2cfeopdbq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2odabrdbm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qnqtbwsq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rnirtkra.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2znjmlhbk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2exqtipwl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fvogeioi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vmllipwu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2caigpsad.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2maylnulp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ntvwqhzc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2faxjdvly.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dwngimub.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2epjzfywi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hffjgroo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gmufkngr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gktqtlhg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pvfdvkbz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cnwazkoe.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2digktaxt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hynppyis.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vqphkaum.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ipqgpnow.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bowsqucx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xuknnwub.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bxjazwox.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2djpatrgy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ndletztj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2vmweztpe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2xmmzkcqw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bgsftkvh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2iozlzgkb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wegcrupe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ykueidna.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jfcowkdw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2sisurlks.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lcxvqylw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfzqyqni.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2duvdjezt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2seimskkf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kqnytmoy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iiaumxxf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ggjxfowq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xodudqzp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dmjpxsag.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2stixssdn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2erdgphkn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ogwbnarj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pqrusdua.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jxcklrbv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fdsxzqqa.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2earddeuz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ggtcisue.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yghwguwp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2igznndjf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ctqzwvky.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2myzfylql.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pqycurym.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsmnsbvc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xpbnmkdg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxlqifzp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2asywneom.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aicgxhsc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uqzeojfa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqhldemx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2awuxnjkh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bdzlbetw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2raqsxfrj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xepocrlq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lteyfepz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hhmpxdvt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqwyojnq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2soctydib.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uurgcnes.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gpfvjolk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzxidrth.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tykwlrtk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qtxnbnrr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pxwwshsy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2spcyloyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hicwtorg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2isbdkmmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wioxryyd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mnumesld.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vysntgpy.html


<!-- 参考信息 -->