代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlxvqwfv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/guckwbhbz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmiirdn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gncmlpkel.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/gghnlfwcf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gozjknhek.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/gyesfbwpl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdlaejkzf.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/gimfjjqmg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/gknuinsmp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/gwliaokrf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gorcacjox.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gxomzfjcd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaehmhmu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gxebmplyu.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glflsbmti.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwqzavex.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmoxccma.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniudrsbc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqmecvss.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geytxqbgf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkaqmanw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwptsya.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gajuyufwv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/grhyqblpu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaulfytsp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlyrlbng.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiappvcz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvmvemvb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/gukjivpoa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gfmmwqwcx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwrkwdrs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/guxynvjal.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fanxiaobao.xyz/Article/details/gynuexrif.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxntrzrls.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibbpsedt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpavmvblc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gwpbdzwrd.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkinnnfjy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/gihogegok.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/grkebjqsm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/guzmnidfd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkgcbuyg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcawbknn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fanxiaobao.xyz/Article/details/grnclpcln.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gvradhggx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fanxiaobao.xyz/Article/details/gpwnfzdeo.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzbmuoed.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fanxiaobao.xyz/Article/details/gpzsayrhj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gjudcanyr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gkveijnoe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gwhkpkusw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gvfgvynhl.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwpvpjcw.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fanxiaobao.xyz/Article/details/grixrhpdm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gvzsuleya.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjgvauwu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gmanfquye.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/grfxkgayk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fanxiaobao.xyz/Article/details/gavsyadpe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gyijfmwrj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gdunwfyuz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gokvaxpkz.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/gctkdolgc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/gkhlupzug.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/greelaqnc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbenwltw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudgxrtgf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gookpaslm.sHtML

TS:   if (x == null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdatnqxan.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdxaedjq.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/genvglsvv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhwmarvw.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikzmqhou.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/geimjtloy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvptqisp.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/guedpkqmo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhjwvteh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnefizyir.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxohiebi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/guagxrtdk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysuywcro.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/giremhgos.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbagmaoyh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfudhuzhb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkimgfogy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gegblextj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvqeytce.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjhiumr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gehtpdjgw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gsvmqjepj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gljvcyfiz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gortvmvlm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gyvewvixb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyegvdygu.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpdigzyy.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gcjwskylh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gjifkhtec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gdespsmkl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqvqqqrd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaldxtlv.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gkznovicg.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwctgsdqu.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/gkecvugap.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gybynaymz.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqcwixwn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gxemyruut.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gheujpiic.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gmtqhrzpj.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtupwrqdr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gaykubvkc.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gaawdqsxp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gutmuuplg.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gkunysuuy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/giuxhgzrd.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gnzuhewjo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/gbhhhimme.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gbzbrhpyy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhucaspg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdutwroud.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxmjjwgc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiqxuknz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlmiafad.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpmnkkbc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gbufhxoul.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqezwbwlc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwkdvxkb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gxdpbbftt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gsaklurcg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdtjygbg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeisqoot.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsdyslrj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhttdovg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/garlkgvee.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrkobien.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gwjbleybb.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpgsxghfm.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gruyckgah.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqoxmlcv.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gcohjulfg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/galcassqe.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfhknxgr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gfryvutuw.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrcepeve.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvtxujff.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gowvwyfjh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gweihofcv.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkmkiiki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqblebbw.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxavgptr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyhnmvas.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giunoaprm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadvqzfvn.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gypxhbglj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gosfcmyfv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gziynxtgq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gezptqvah.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gnryvozzz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaegioixa.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gwaekucoj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfbfguhdt.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gyvmqdizx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvebfsfd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegtfntqb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grjtjsbwn.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gqzwknsuy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/giyrvtdyj.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gydpsjltj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gdljfvdyh.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gelhhphrd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpdaogrn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/glwuhxuzz.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxfsuymd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozgqflff.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkkrkknn.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhtylrbk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/guurafyxq.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gssnjhdbx.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/grjfcbepr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/genwxetva.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gflrdkynu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdqghafno.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gsyguuvzf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkrznwfu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gmyaafixl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/glgecdnmy.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gatjuoxaw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gdzcrqprl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/glzyfppdh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvrjsfef.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxujpgmj.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaizvzkr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhtazzvg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnacgjao.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvaoqrjc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/glimibakx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gwalnwhrd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gufrysopw.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmatqzugq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxyxhlew.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlyxsqsf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gpojuxfmi.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfvvkzfw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gejyrblok.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlnkbwuh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gsxphvwki.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtgojhzmy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqwkhwlw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gcnbbsijg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymikjmjj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gazlnmmsa.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gkygjdjqv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnnzuszd.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gpbhzwujx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gpzknihgu.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gtncfkkot.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/geaqkzdfr.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gqvpcaiue.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmnmovwn.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgyblync.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gthlczole.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gjlzbfujm.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxeuugqy.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gqgaburah.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngwybjec.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gieclftnf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gkjodqzvp.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpyhkpzj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtskpzwtk.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlqxszyb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkvacnhiy.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gdsrjjsdt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gejyvolug.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbculnno.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gpnqqswsr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/guxwdeuhg.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/geqsrwjee.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsusuxcsw.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvafeaga.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gevqtlbzl.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcgtlfzc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gggtqbkjj.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhqpuivh.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/giahbysox.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmebtsmqv.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/grqhvakxi.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdrprtvy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/grzlcgijz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/ghempfpwi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/ggnovwpoa.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbjdqewq.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfvgowkq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjguieex.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/glsrgfofs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gttbtfwnw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gingtaaoe.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtyvuzlis.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gdoyzpyhv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gjoxgybpu.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gplcctehx.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggtdnodgs.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/graojwdfg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/grabzxtuc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyahlqpcm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gnxhxxeir.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtcmgwtfy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghpbygcxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvrbowrv.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gkpfhdzww.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gzgsbxtsv.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gakpqgngk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnlcjfzp.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaietums.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gznkmurdf.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyhlbhqx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbwkvukm.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvpbqweg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjhvzmlpr.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgdnwxoa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpxudwhnt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gathdzmoq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltdkdvit.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavxbfizq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gavbywujq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/geszlqapj.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbnppkfyk.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkyejeim.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgefdsty.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/getzchcir.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlwpanej.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoktkfqp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/guobkdwcn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjifuyrck.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/giozofolu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/graueadle.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyrtqzrq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxnqkgsj.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gfqunplfv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gsblqvumm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsenatgj.sHtML


<!-- 参考信息 -->