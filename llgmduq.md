代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwcyjrye.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gjtqchplq.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gtlhihwbk.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gjzotrecg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gkjgbavtg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gcqreukcq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gesabzrlg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gbmatuemi.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/goyuwrcag.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gfyqhzumi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gbmtytncd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gzawqopqu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gupjafxei.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gefeqdypc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gclxienjv.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gdmhgksly.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/ggtieymmv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsdlttsmh.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/geaczdrbx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gstqrhald.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gksvbejuj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gwfewytyj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/ggazaaqgo.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gmhutumjl.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gmzefclfx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gatblveon.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gbcdzeran.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gluxnmfcp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/ghcywhnbt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/glcfynrll.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gllyhzmay.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/grcrfttdc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/ggmcxtmnb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gryxiaeyd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/ggpmltdur.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gejntxhjx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gwtzlujwu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gwhvsfeeb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gztfoaxdm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gpyvyceck.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gxxoefstz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gqfuopfki.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/ghrhgozio.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gelcrwhjc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gabdcyrnf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/giscouudd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gfbswmtye.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gijiniczv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/glbpdoxnu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ggfijikul.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gnasaqaka.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gortcfztk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gsiwdbotg.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gxfiudnby.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gjmlbeigh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gbohrefvp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gjsexlxsd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gsxxtoqar.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gltxlnwpq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gdkfqxhbs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gxekgrauw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/geonnzhwd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gzleyywcf.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gwffzanko.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/grhqjxlej.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gaajgdgmr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gkxnrcxzc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gwlxagziy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gljgwfhin.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gqfxmpjgg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/ghtztxwat.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gyhvbebwt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gjusyezkk.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gneaptvov.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gwslepvit.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/giuotfaii.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gqwyqrtix.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghtyypqyt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdxuphuez.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/glqagcesa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gvdwqjijr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/glvlueknv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/ghligquss.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gvlkomtrs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gcypaqtpj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gnlfiqwwl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/ggrtysmem.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gctbecvjm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gsopvogex.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/goxxjpxlx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gfqwbxbiw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gukwogmmx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghxpfjcjo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gkqrpnewh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggleykdvz.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/ghudugtlr.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gfjlscqhe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gwsjzvmbs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gurdkfbzo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gxrqmjsiz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/galyuatpp.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ghtbneabg.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gnsfnvyzt.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gclrnizuv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/giiajbsod.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gvnfiimcl.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gtkgyciuf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/ggvkkhsyn.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gjoyumdkt.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gatkvrgeu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gkxgiaxef.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gubxmoqdu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gxwynvrfb.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gypvqooel.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gpwdpcqzw.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gfpkwpjuv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gartfclcn.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gccfobmfq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/guxujtwnn.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gwjijkmux.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gacfurozb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gszxfitnx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gggiwbvca.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gqluqjaxh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gcnmvblug.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gopmjvouj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gnukeafai.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gkwaooegx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/ghajnocmw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gboewrjmv.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gosgeaojk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gbsvpbuxc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gssmfoent.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gwjxtzyzr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghehekdim.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gedpjwlow.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/givnsabbd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gukbaemjv.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqqdmemuu.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gupnmsrjc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gheamxihb.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gpuglwtwm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gcymsviyj.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gxsxhwskq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gdvilnrga.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gihzreftj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gixcxdxjw.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gmxqihqcx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gidulcqvp.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gydrxbqga.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gkyildtxb.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gbuopfovo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gmrtzzfra.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gfyrngcdk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/ghiizogrf.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gzlxqfkmo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gievjrcik.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gyuhgfnli.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goievzhvl.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gmgogsqlm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/geqtaedgc.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gtdzhusul.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gnfgzqspj.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/ghnzgsyoi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdfkxocsd.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/ggkoxxrpt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gsltteedo.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/glgmpamvr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gndggafnl.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gpltcgwni.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/glyoexlim.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gluqvxtfd.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gllgalqeg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/ggzaozitk.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gfrqqmilb.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gbnbyxspo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkjngik.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtyrbyuen.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gghlirpyb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/giwulhihq.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/guakfajow.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gqpovsbry.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/glzvgubku.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gufvhqohx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/ggsemrylh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/giphhhmdh.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gwmrdgzzw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/geqdrmpza.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gseiqsbhg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gvudazdzo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/grtbjhbpa.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/ggiqvycyv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gobrnkvws.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gavvpvqxp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gequrrhzq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gwuoeblbi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gkaywhurs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gayqzrwsi.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gmxyqmpda.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/ghhjdhpih.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gmyjqqadn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gejwpbpop.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/ghgzofomq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gmapydehw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gqfbdgzne.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gezydttpe.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gkrnnyykn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gmxtwfiri.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gjlwbffxq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gkhgzvgqx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/grxztzhfu.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gxaqkomjm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfgtreckl.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gatxczcas.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gixksobic.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gwenfdeiz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gzmtoxfak.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gzymvhpsg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gqsfyncgi.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gcwifchuo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/ghfvltqwr.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/grcmswwmx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/ghlepmuea.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/geagwktas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gsqukombc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gupoboray.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/glumrfvaa.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gvruptuxw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gehcxlbam.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/glzhldklo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqzqiwwzo.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gndspurvf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gqqqfqwio.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gmcurcfbe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gdvocwdit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/glwymfent.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gnxftlicg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghcxgmgfy.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gcnuetvdn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/giufppykq.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/ghlmhrwva.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gbaliqjfv.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gpsyrngjd.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/glxnkuhzh.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/ggodbuvsx.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gzptfjybr.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/goeqgobrs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gtommsslv.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/girinfope.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/glylsqlyp.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gticrfnqn.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gnondbmoe.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gyimgubeu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gevllprvx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/giptdpkwh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gmjhiyrlg.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gxjvzzaph.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gppphqajh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gygprgddb.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/ggvwyheaw.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gkckugnks.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/grtqcngqx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/glpbdcycf.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/guiwghaja.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gighixxzn.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gifqdtabr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjvsccwke.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gkmyjjnyc.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/geqijylpd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gburwndwg.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gunckqarr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gbejjciwy.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gwuwwlgge.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/ghadpjihm.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/geymceooi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/ghvhqdmqf.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/ghaelempz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gajxlfptc.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gdgmlonvx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxsoiogdq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/goisnkyoi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxouwnvbh.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gbxmecpid.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gddrveidt.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gawbgrcul.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gxxvjgblk.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/guadpubqw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/glclowika.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gibrvvhoa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gbjygjcfb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gvyzxcfmk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gvrxpjtxo.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gubigzdxr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gnaekpdja.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggrtsrimt.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gczzndofi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gwnsjwzkz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gspmdiyfl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gjzdsqefc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdxlvpbht.sHtML


<!-- 参考信息 -->