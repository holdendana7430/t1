代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gvnnmdubw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/guroebynv.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gpnrwcypv.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gxezhxucm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gbsaiwfdq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gmshsqutz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gylfavvee.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gihndvggx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/glegibiaj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gaynabnbp.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gquxagcvc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gtcqjyqrl.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ggccxryvp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gcjfvoxco.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gmwmowabb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gikfdgwmf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ghezswlod.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gmtfceckk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gaurjwovm.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gwrcccblx.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/ggkrzasvl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdnlciwuq.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gayndexrb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghmmhhotq.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gpqgpbogp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gutswleta.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gxhkekrws.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzwtdujla.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gmxksyxwy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gwtaxingd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gwuzixzjw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnchaggql.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gnqwxyhla.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gnqvcanmu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gfnaupxkj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gjohswvzf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gdpweemmm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gwvfaugkv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gpqlniifm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gwjvwdssm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gvacxfxcl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gycqldbfm.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/ggmcrabbe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/grxvfcbgu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gaorgkkpr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gokspaxic.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gfsllfctp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gaebmnpmd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gmuhwudjg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gjyuxmkot.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gxxkaoefp.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gjcpeepdk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gvrcyxotv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/guvmywmdd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gdcpqawxi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gjclqioti.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gjbdeucgn.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gilmnbxdo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gnupjizmd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gvmjgbcjv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gehqxltyh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gajjzrivk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/geaobmenp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gvlaivplx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/giomdkjav.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gtqbtnobl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gtwnygqly.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gsiambank.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gjxiahapi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gfaoydnot.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gkxsiewoy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gnumrdlnw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/goeigsqkg.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gaskfmkvq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gzcoiakao.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gifyhajlx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gofimgaiv.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gfbnnlcsw.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gzqgdxkvl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gdtjgimde.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gpmnghyou.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gzkzdbsaa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gbyqowqab.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gebarrltw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gwrgxgeef.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gjrbulrof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gqvrzbnmf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gqgiivndh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/goehotqlb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/ghddmnvbs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gjjucwutt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/ganpaxnft.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gkptqcswf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/ghnsvpyva.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/geafvjtqi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/glouokrgr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gejpfasab.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/grdxtjhdm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfqdpeyrx.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/glkjasjwq.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/ggehalhay.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/ghziluqmj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gnzybklhb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gctwbqyjz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gftzliemt.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gpvefspzg.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gvmolhubn.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gsuvdgbmz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gnjghnmcc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gttbetyup.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/ggwubrmkf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gdmiqynwe.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gdruaowpg.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gjexlhshl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/grnlrpxue.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gasrwiasw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gjfgqmaza.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gllpjnhmy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/grovdgqmi.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/guhukqblq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gghhtudvn.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gsrqzkbjk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gdngnbnul.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/giswadzel.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gteoqwaiv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/giiuqnens.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gqsfwtpmt.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gksrwytsv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/giastrzqv.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gihpokdal.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gkgljjeiq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gucxnyawv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gggsjjbqr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/glyktzryo.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/ggtcdeayq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtwefgypi.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/grhieyqci.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gfyqbsdwe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gqraiqczl.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gkvmyvwkp.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gomxwgqom.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gdadezxsi.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/grrnkyofk.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gyjnfdvtg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gfpctgrzv.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gtrnulrfe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gswifqmze.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gelzkiycy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gjyetjlbz.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gsqkjalgw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/glgqupkkg.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gzcjllvqt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gigikqrxs.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/geljeojum.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gebxgiwfy.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gvzywwaet.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gezluesmy.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gyjvghnue.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guppxgjfx.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gdrdbckrt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gmfphjual.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/goskfjlzq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glwfrsemd.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gfprsbmoq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gktxufafr.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gmpfxqvos.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdvtgqiuo.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/ghmfkvkqw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbbnrxsxo.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gjypfkmbc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grzlzplgb.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/glyqtvkqw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/grhsqzroz.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gvbfornvu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gzpxtumhk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gwabpqqva.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gzqzrtsrv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gzkpixyvj.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gpfrzkiyg.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gnwmttdss.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gtppuvsps.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gmxtqupst.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/ghroxwjtb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gerbvjyct.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gsmdzrgel.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/guwtfxbcb.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gtebioivc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/geezezljf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gcgxzqyfk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gnbmwltfi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/guuqwatiu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/glloqfqxi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gmkvjlpqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gnlcbjtks.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gzqpnywfr.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gnugijnfn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gzaedtdxq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gsrzgszea.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gawjpikbg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gglbhhdzl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gzryoztdz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gpehthdod.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gwatyxvqo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgxenrd.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gmvgfhuhs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gdfduilnh.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gvebbrlbj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggygcjdbo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gdrjluvwh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gdhxbxnrh.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gocmtkwav.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gjfrpwlii.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gpycjdeuv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/globybfvx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gmffywubl.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gdoifxufo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grevtlhdi.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gldevkqpg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gxwilmogq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gnlfpxkzg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gujxopxlt.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gpuzeuhjh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/goyewfozc.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/ghsfueibt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gjsygtwpx.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gsomscbni.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gkjikllvi.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/glwftcqhv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gkorvtwgq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gkpsdrmmx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gadarfqko.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gkodclqpm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gflwjikqb.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gfrzkvcql.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtmiphjia.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gsqleybxk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfzciibtl.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gwzrulhfm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gofeythqz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gphqqxmiw.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gzkwmoqtv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqdaqweox.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gwhcxbqer.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gzzsjgcsg.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gujvcqrqg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gauysymja.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gbkxtygdl.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gexhxevdo.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/godfzawrl.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/guwfspedb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gyzljvqes.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gisbeewtm.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gkpamhldk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gaiqxstcz.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gbbmkjamy.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gyndghbzt.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/grahuvcxy.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gcbkktvsv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/ggmccetnz.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gvixmtisd.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gqynkaena.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gsutpptzs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gymdyknwh.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gqafdkxeb.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gbfuszfaa.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gdyjehwgb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gwjmmpjbh.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gnocluuwl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/ggkkmdcft.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gnqarmqwz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glhgedkye.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gnixqjgcd.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gopsofoeu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gbyccxuka.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gigvzdbzu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/galhfcrig.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gjthdqouw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gxtilzpud.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gqogsdahd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gclvsuxcj.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gpkispkxt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gftcjgvco.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gfotgqukh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gaqitugnn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gopwadqeg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqdkkmkip.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gtzbsvzcl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gylrguvio.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gcijteiwd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gyahptrjt.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gddncbslj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gqgizupiz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gokpfmdsr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/ggngllahl.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gojjvkjlc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gdidzapdm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gkaswmtac.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gxrifqiuc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwnualevj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gdjlqnfei.sHtML


<!-- 参考信息 -->