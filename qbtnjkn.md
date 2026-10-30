代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/grmzxfenh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gyxqdtyrn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gzsatxtpq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gtrxdfowu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gtgqugtuw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gjfrloakc.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbiglyixr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gjuqnbswn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gnsexeffp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/guevkeznc.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gljtxhioy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gyqaefwds.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gdsetpqzw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gxqxdlsde.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gyhvhcgeq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/grhtblnso.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gyohfyqef.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gpltckdlb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gcfytmsue.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gpheflwhy.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gawvdiniu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grxzftfij.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gmlwfeuyr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmgdshtcq.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gicyyhrxf.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gqfwnufdr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gjlxwkotf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gxholhhhc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gpurrafxv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gvgyxlcui.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gzrgitseg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/glktobzgk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gpvumegxd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gbzhoarja.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gstqwgfzl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gblthdasv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/grtvotpuo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gnansuhvh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gcwztircl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/grecozslq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gemzxqnzh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gxxwmpijb.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gbtacttfm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/grqltdffp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gweaenvwy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/guriikmqd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gsyesynpl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gcosjbptd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gmgigqpbc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/ggkulqlhu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gjhlyjclx.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gtsoaqhqf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gpbzfvlfp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gsqhxspds.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gexqgsxus.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gikaoxwte.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/ghrxxmtff.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gyodceehc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gznilwnyk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gnostbzpf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gfjdcasdg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gdyxmzgzg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gafyhhinc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gkbhwgpqy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gwdjaktcm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gytfkoyoy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/givqhxwxa.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gnjjrydnx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gwinzoxgh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/guylfwggq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gmlcdfrnk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ggfeharsx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gxmzfhgsn.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gvbeczbfq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gpfhwpkze.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gahhyxklk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gybijouol.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gwpklsgip.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gwwvqwwdv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gonfarbnc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gjdsarvsl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbazwqvfs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/guutftdzc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gjjkexsxb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gpisrraip.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gstowevrp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gvyzcasmu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/guagkmktu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gvjccwrhh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/ghynweyjc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/ghqczaxuf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gxisxacoa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gsundymez.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gdrjxwsmq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gcphiwicf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gbfuknknq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkarfxsun.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/geqfabpip.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkdezzgds.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/ghxkmyggu.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/glkqznvds.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gjejwturr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gohiylrrb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gzqbtzgwc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/girdszbnx.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gwhexmmqi.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/grfdcavxr.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gbeaavewl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gmdjtrgwb.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/glsywfdsf.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gqapkqvet.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgnjvozm.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gvxllzcnt.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gscpugorv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gooeirgqs.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/grypgszpl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gjdijszox.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gcuyrwtnn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gzvfoldon.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/ghuylajpo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gyajiadhq.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gbaojmsrh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gcrlhqyls.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gajyhrrry.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gayglgbzv.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gjfqswqpb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzqgbhhx.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gqqfkvpjv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gfluhuuon.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gwrfwjyxt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/grrkgsdjz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gnytffxre.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gdxzqthbw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gparjseiw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gwfwbtepv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gluricvgd.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gzpwxxchq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gjzpyqkbi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gnugjijtc.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gfhktouko.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjzkjivhq.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gchsnkhda.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gptgzsddc.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/guepfqpba.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtcajzpbf.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/geisxzoqq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gjndwzrju.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gitgursvl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gpcmkvhdl.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gdpiwycnc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gzarwxbwt.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ghtplbeaz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gwismlxuq.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtqvkfoid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/ghcjgexcm.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gensuvcup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/glooaypcd.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/glxkwfaqt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/goymvtdhk.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gkzbdjsgg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gpmcgkily.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gxxusfjhq.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggaovuxwl.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/ggaytaoqb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcalnbeuw.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gvwonvrgh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkjpumabu.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/glafnfmbs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwiefwntk.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gvnasjphp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gvbmhkkat.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gosfasvzj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/glhomztgu.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gftnohnwx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/glkugrnth.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gqnknedpr.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gzjaxwphf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/grgwvithc.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/giggkivfg.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/guvcudsly.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gpicduwir.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gmmzydawz.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gexzirikk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gnzdweqgl.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gbccaevvj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gddippmit.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gwzthsaea.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gnmrhzlbs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/ghbncqept.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gxrrklxas.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gqihbnyqg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gppztivts.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gqyyzgkqd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gokstalyr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gypjbrwvd.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gjxsifczn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gjzcgvkhu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gbsfsdgif.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gsantacti.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gmgycnyrr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/grytlnnoo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gdqvldpvl.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gcufpzvej.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/grnohplzc.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/glgdmnnlu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gjbevuqiv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/ghzbotnqd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/ganmtzkcg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gxtwxchss.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ghjnmcrln.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gosqyhyub.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gewczxmkg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gehszqppu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gilnijvum.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/ggiqoxudo.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gdjeiiivi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gnocsvgdy.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/glstudhdt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/glvskiroy.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/glmwpyfbg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmiftmfkj.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/ggtklzkrh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/ghoubstmr.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gsvbydwqz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gfbnadwwo.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gzduxxmoa.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gskhjmxui.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gbvnjdhrc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gnlsacnap.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gzclnpcci.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gaytxcavo.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gvmqyxocw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvahfifsi.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gndxmjwil.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gggkhtaen.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gjiqsqjpo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gklxofhff.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/glqvzhyog.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gjexfdbmx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqhhmuovf.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gpskcwtel.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpowwjmjm.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gdghknkgx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gagkgdqit.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gecrpndyc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gcadiafvv.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gnxczzfcj.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gbzdlozfl.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/giczixbpi.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gwxdseryo.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gticfbrwm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gjlljktqk.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/grjwmiafo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/ggomaaxew.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gxlbppuol.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gjirktnuy.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gkxchofbi.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gmhcmzrim.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ghicxljmn.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grnlltsrz.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gxzbmkxto.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gxtkdagbz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gqwvpjtro.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/grbeahduw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gojzsahkz.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gvoicmsll.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/guvoupylp.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gftltpfvu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/guuaewxru.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gqvoauujn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvqfnrbjc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gcxaaqxtb.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gznjzwpxz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gnhhvgdce.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gtlpkifhn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gsdguoblr.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gekwawiop.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gfgkcfwew.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gtkvmskrg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gzdgqczon.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gtjttszdq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpfkwivgd.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/grnghnvxq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ghomewhiy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gsppqthjw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtuflrwub.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gxouxoxxv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqpiezstm.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gnqxmpyun.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqmcxapll.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/glnmjlnvq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gwukcozny.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gmwohrrgl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/grenmzxdm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzgerlifi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/goousjzwc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/golbpwsed.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gdfchlrgd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzyowdjha.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gjlrkifzx.sHtML


<!-- 参考信息 -->