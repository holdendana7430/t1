代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gvsrbjysc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gbggiplqa.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gwylvuokv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gqlvmptek.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gswloezir.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/guzpfjnlw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gsooixmzy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gyncavasp.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gbessrwfg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gflvaprpy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gitngwxvs.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gqrohogfd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gvkhjtzxk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gmkltsvel.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gbwucxsny.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gijdpclzi.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gplsmjtfs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grjthqyxm.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gxulgfdqc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gusizwznw.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gjrivecsh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gnlkbiqbs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/ghmpiiqge.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/grpkdaphb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gkxsvkeif.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gyevbqhlt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gsvovpzey.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnitrcbim.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gvpkzqlbh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/giexvqckl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gizicvrid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gcllztwhq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/ghjsqtmxx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gfulsgccd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gmivmpvhx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/grfxpgviw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gcnkucwyw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gwtkrgefi.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gcffmfccg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gtvcpfwnz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gsdxgypvv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gyhkvmrvw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gbhqidrtl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gsfyesyqe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/ghqzetmni.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gsbdwdxht.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/godfbieys.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gvfnpebxm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gzfhladeo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gupnpauft.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gyuruahyg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gdrgbzpri.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfddheyxj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/ghdgchopp.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/glomvepsa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gydoxfvvb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/ggppgoroo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gbpvmkwqv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gfnmfediw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gbztuiuet.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gchtmazph.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gxzuiotih.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfjaltiyb.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gspzeabju.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/glzermada.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gbqjpxkwu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/giytlvpbl.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gvtofljvz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gbsbzgzzf.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gxwhhjeuq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gbyxrsdpq.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gxpmasvff.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gxqjqttxx.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gctfloxad.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gflfimkba.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gdwlzfdky.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gbuwgtlhc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ghzltgnmx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gxrgxvzgm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gnxgwcmdr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gyyzpkxat.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gkivulsmj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/grrlvgevc.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gvqhymaqz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcajwtww.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gxvcjhfam.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gnclfdxcn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/grgthscnu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gryaomkgz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gxyznscpp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gvhccdbtl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gnroxxypo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/givscurcv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gxybqgauc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzeubinfk.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gndoowgmc.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/grrdvuhsh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gbkfsayft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/glwoddhhq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gbottkboa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/ghvxwjvqj.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/ghxdrcgmx.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/ghiahklpb.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gzzwkbhdp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gepnnooar.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gzwyzjgqx.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/guiwsyndw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/ggqeerenf.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gagwfjfoo.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gfppfnytg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gybngivxp.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gpbhfqkin.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gmuqgexnn.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gsyhyaqee.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/goimrfvzh.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/ggqgoywzg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gkjyuvdrd.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gjnxuqorm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmkyxnpmk.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gogwlnexk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gugpcrxsf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gjectncig.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gjxcxeeov.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gtlymunsf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdanwhofy.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/ggmpovqbt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/ghykwkffc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gjxieuueb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gcxrietnm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gsmerysjm.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gkpvaswjb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gmmeffndb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gmntkskli.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gcozugzrt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gmundvkob.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gzzsykaqi.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/girnkytvk.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gtuwbcdte.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/grljspnql.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gcosxclii.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gxnqfzhsa.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gzsmofgem.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gjwawplxy.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gpniivkva.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gbgywugea.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gekfwsqfb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gbmbrjjba.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gvrzvuxdc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gyukktsrr.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gsiqlydco.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gejmeuqai.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gohthppns.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/glcxribxr.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/ggmlhrshh.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjgshvsky.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/guuvqawxi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gcyswosgd.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gamwotomg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdpttvwxu.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gfuvbxzka.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/giqswdzhf.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/geerelbqw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmupqutpa.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gvavztahj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geghrkifd.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/ghfoynfzj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/grwogseko.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbeadlpbx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/giyklsyue.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gakmzbvva.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gzzmpszia.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gcudpgjtd.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gnqajoieo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gmkvvodyu.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gfzodmyyo.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/glsbuugfj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gdxlknjoz.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/ghqltvdfc.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gwykovlxj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gkhfnwlyc.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggcathlvf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/goavrbpnl.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gklukqeml.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gdgsdhdkg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/geggammns.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gexesexjs.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gmvnrwbif.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gvcxmnkit.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gknvrhufd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gnkwjecup.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gdrxisvoo.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gkscdqrac.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gjahifzxs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gtnzejqxy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gkwnxctkz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gnhxpebwh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gwkzsniya.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gnextfhjh.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gdqrttnyn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gpjqrlaev.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gjblyrlga.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gqwkdmtqa.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gcbpxkkge.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gxajqegvn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gvzwerlga.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdnhpme.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gekwklatl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gtcmxeynr.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gkyymurxs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gfuerkxoh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkexjcv.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/ghomsaiee.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gnksigbnd.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gmgsyjwhq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gsktxjwrh.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gpuivnfta.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzwxfgrod.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/ggriyhnxo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gulsducte.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gfkfkyjsb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gwnpbqsug.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gyduamppf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/grmjkqgnj.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/getodflqu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gqiivqsbf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gkymviveg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gacfvujnx.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gxjkieqbv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gelsqybgi.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gasyjbqkk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcsdptcgd.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gldmmhixm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwxhewidh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gqiozvzpw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gjxuolmat.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvbqhdoda.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/giobdonli.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqefabyes.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/glxbfczmw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gzdbjnzgw.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/ghepqrjnp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gvzpvgrjc.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/ghfpiikdt.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gojbvhuqs.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/golpiwrzp.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gcusulxae.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/ggechivqv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gmofagcrg.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gwsabhhij.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gaoraazdm.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gsiwexlaz.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gbvhujdvv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gchpgcbgs.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gmvswfvsq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gunkghxbz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gimgvmsqh.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gwjjbdnsx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/ggiglflrm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/ggylgmofd.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gphvrvwti.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmekaspty.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/ggnlkfplb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/groadhjwf.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gbguqqckz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gefvjkdri.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gdgfzegct.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/guxxqwpzv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gcasghqpg.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gozwtfxyi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gfoqmfyqr.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gmudlouzl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gylmpnzxq.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gsiywvyrn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gadvbfjdc.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gbhdhqpvu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gicvbogyo.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gcwxouesj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdjsgodde.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gmxmixzvm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gdwdplhgk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gmivdjmdf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gowscptbr.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glhhnckvl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqjubkfut.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gpirwscwk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grtwdxqru.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gcofarxfo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gnhsbagsf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gmviqkvtg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gaxrhnlic.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gdwqnqvzt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gjmfgpfkc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gecwlddvp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gizpueryi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gutocbqyu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/grcudqvbp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gpqifrnie.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gdbpwtkfi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gxjyxegsm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjsyeyudi.sHtML


<!-- 参考信息 -->