代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gzewpdwuv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/goqesjnbd.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/glvlcmaow.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gemepadwl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gqzqkwjvi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gmkgzfzqb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gkuyqocqi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gcbdmxdqc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gvulgemad.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ggdszlhkj.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gfxztyvkw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gmnztjrxf.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gjvgvpihu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gowzxqvzk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gxeogowcg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gkeiexenb.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gztrycddx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/guxbfmjsu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/glovfmvrq.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/grkmxobpg.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gsgdlblez.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geguscjfa.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/ghpjkuxqv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grkfgsszv.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gzmevhprg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gbbkitihi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gkbvoimgq.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gspgreqxr.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gavyticff.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gpadcnhcj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gphtxezor.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gkrkfknvx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gmmomupmt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gsoezmokp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gidbnvlun.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/guxuypqij.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/glnsatpcd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/glyhsyotw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gbgtwcecc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/ghicjazde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gbuhwbhqm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gogljyokq.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gehmmxyha.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/guuzyqozl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/glwsgprfw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gwhwbsnll.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gcizgxjsi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gfexvlvcq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gnlhhlrni.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/glpbdxkfd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gwpnbjvhy.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gxullaahi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gayzcejin.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gmarhvrkw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gqoxstxvw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gzpalzfkj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gdcgxiltd.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gjnlctykk.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gibqhyird.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gvmheemcz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gbzfshhwk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gjdvyighf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gaqnrsirw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gqakiraqb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gernwbljn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gkyxvuhkw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gbskdastk.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gpfuniqhh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gphykdbla.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/ggrvajygc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gdpvlvabx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gjqhwunkq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gnyogvdjy.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gmuyhaqdi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gzvuzcafe.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gbcjezcvv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/ghglaekaq.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/goyzapjic.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gabzpcovw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/grdpofhmd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gaxoduqac.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gstgikjxo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gspxibred.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gfeodrcqn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gjdwtoful.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/glboqgyfs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gxxlhqisu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gltbosium.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gjygqhehp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gvohovgmr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gisvpklmy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gjnsjgwqa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gvvuizyas.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gcajuibif.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gvlkncvjl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gvwjizehq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjxvfdokx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/ghoqeboiu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnmpjskea.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/ghtfhjzza.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gawcrafyq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/ghzfrezox.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gozwswtfn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gjxrmwnxr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gvdfmanvb.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gdadilnow.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gbynljjrp.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gcmumepim.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjxkhwawx.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/graplfqut.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gpcilygqk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gswooxfda.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gehrnlpwy.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gdyvfhyji.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/grnaphbjh.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gofvcpjgq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gzizcxqin.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gzurzpudd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/grkllfvmw.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gyaztzklf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gfbhixgdj.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gjsgdtdtz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gphuijase.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gtdjrycpg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghgnobqam.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gwpbnagar.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gadgdrstq.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gjahguoxm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gvwlvthlj.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gdndmgxnq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gkulumqug.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gttfiruup.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/ghlldcttc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gghcpbcyz.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gnnktyywx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/guawylvqg.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gqwxruruo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/ghbomuvoc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/guvwedskj.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gbbouqrkx.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghtlvzyks.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gnqtewpzf.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gqwoqrvbu.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/giycyafcc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/ggwpklcqq.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gskqwyvop.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gslzgaleg.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gplzozbex.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gucmgfmxn.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/givojdmim.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmthofqk.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gailvufqz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/grpvzklbn.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/glksxjvpv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gnrmizsqv.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gswdbydts.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gjsgijzyd.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gebuxugqg.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gmiihqoao.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gkmlqbouk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/goftbgxri.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gzshdrpla.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gspinqdlk.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gmiwmefbr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkxjaeiqj.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gykcrvjjr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grhubvtxj.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gsfifgnsx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqghjyzfy.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gnplqkmes.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gfminzhwz.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gkdldgewg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gkpcddtjt.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gggwwmspx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gnywjaphg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gijgsmqkx.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gsyizwghc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/ghyldapjk.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/ghmvtstkg.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gtswquhzb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gcvzrdeem.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/goeuddjsx.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gxfdcstel.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gnbumqadg.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gvousqgkq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gmvleswri.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/graqtlzrs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gwertpwny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gvymljxni.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/godgquvqj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gqqpqatvu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gqdzglxed.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gzbbhhzvp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gswfvxuvi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gpqdkpllk.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gffluairr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gvfurfkaa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gvjmsumat.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gifxvnren.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/ghpyynrcs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gmpvttndx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gclhxkhmd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gychvslpl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gayqubaay.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmoucqubx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gilpygrek.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gsoqfcrri.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gmabzhpqc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/ggvcjrqqh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gsfpareyh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/guaxomdgb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gmuacroqh.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gpdfbnkht.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gnmxmnatq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gvezrlzuw.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gpdlvkpqz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/glkdswwnq.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gzcxodmfh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzksfqvps.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gpnzrytcx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gcguitswi.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gxvudomdn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gpmqnhorc.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/glcteqgot.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gqqhgoxee.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gtdelumuk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gnxallpzd.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gneitdyep.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gxctklkxw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gyrxibwzb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gmbhhtfoh.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gokagvwav.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/glineoexs.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gktbupibv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwwbxhydb.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gwfhpaytw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzvvzilfx.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gwudgssxj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/grehrymxm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gnqyxbqxv.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gunfxsjwl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grtyseiaj.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gqqozivsz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gbkrcsflo.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gnzrsfhdz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/geihkehvj.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gwghyolrr.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gqxxhgofg.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gzrotpqaj.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gbpedtjjn.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/guryozyvw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gugtnnpgw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/godofxytz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gtxineenb.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gwrisxghb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzrzszxnx.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/grgjccgrh.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gwfxivvwr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/giobtsdsr.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gtyhlgsvb.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/giiqmfsqz.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/glmxalcsd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gaumjukiu.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/grlrwmpmw.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gvnmnajxw.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gtsczutwo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gtxextfqc.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gddijazuz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gcvebjrao.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gcvuyxfgf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtwubjfdy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/glnnhsexf.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gtbsddfim.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gkehmlfth.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gxbztjqjf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gcidlkrta.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gaytytjkc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gpcideacc.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gnxqhdlia.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gztgodegn.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gmrkxgosn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmlvsxehn.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gsyazmoya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjebbnthg.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gqvjvkrbn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcvexrapb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gcuqkiawk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gevhrojcr.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gprxqlhyv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpkwnakdq.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gbgiiasbc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gzvgurcwa.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/geeyhorll.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/guflcpkva.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gkpglybcu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gqajjdsdm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gfuomnanf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gariwyrfy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/girtpvwxs.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/grtsfhupb.sHtML


<!-- 参考信息 -->