代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gdxwptjig.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gpuhsstkw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gjuklfnzt.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/guzqnrihj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gqpktnslw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gtyfdcmrb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gvgmuruuc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjfvuzsv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gymrtmses.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gycqrxxxr.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gyxxdhkdn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gexxwjxrb.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gmyqmouks.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gidxjmtii.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gfsyhzkdt.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gkrubzren.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gtkyofiqz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gbdwbuurp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gmlmulqza.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gqgluiegf.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gqkqicnip.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvafpgehy.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gaacmlwpr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gomwqrsdd.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gurjkqppg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/ggxdakehw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gifcfujev.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gymddngua.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gdomycrjl.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gpjebgpzj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gaijwbatd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/grtjuvjph.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gsdyiocuf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gjrpyrasa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gxqllxrgm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gyjnwvdle.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gwawhoixu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gustgvvjn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/glqfnlvfg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/ggeoxfqco.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gwrzaxngl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gngfwzopq.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gounyxzzr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gyszvrkam.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/grdhtwnei.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqwhaywmd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/grzdjijsb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gukyfwywn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gdykledyc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/guwaqhwwb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gzlrbvsdr.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gyuhhdlnm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gqejlkkjf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/goupyukwf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/ggqmcimuq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ghtlmerwa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gzurfvtvm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gcnozjauy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gpmhzmwhe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gbcdmjxde.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gcmthepwp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gopjlqcam.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gdcbabeah.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gqsvcanbk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gtutgkfhc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gemhvkmfy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gadaezxue.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gnsoqmgxt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gzsqebtof.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gvtdwvmme.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gtogjtctq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gygcnbxim.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/guiovcbpy.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/geulyzdpj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ggxcvxvrg.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gqqjewexg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gvbappbsu.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/goaoksygr.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gfuvneurt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gmnleiwot.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/goasxbpzq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gwhaoefzm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gvfrktmnd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gujlpbsdo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/giezaoqls.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/ggcxvsjyj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gsskkqpbg.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gajpsenpm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gfdxsfjez.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gshrnvqvm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gxgqvnewc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gybfedazg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gqnocoaht.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gnocfcmyd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gwyqrcxsx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/ggrlrfatz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvywisnzo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/grdlgetmx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdtvbento.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/ghqbmiviq.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/goeudkxrp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gzuoyfcff.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ghpltbdpk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gcfjdptrv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gnuhyvvqz.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gxytcmtco.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gebpiwspv.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gzhgnmfrb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/giqgpcgek.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/glxipjqpb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gnbclstnq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gqwmuifjs.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gklrsvney.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gpowksdpa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gguwdxgwa.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gzeiusdfb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gblqebbbc.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gfgqtuuvl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gnbevnmny.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gnasnkxnt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gfmxpigum.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gnspvocfi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gnefjxjtv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gawpopzxk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gnlsgjubi.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gnvgfycgs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/ghgqvtxej.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gwsusfyrg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/ggtilqxnf.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gmfjldajo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gcmnzbkok.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/geopenbkn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gzclchcxv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gkralaouj.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gtuslnuiq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gkotpmssh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/glfbnouse.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/glbzekjvp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/ggasrvgpa.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/glybuqxgm.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcfkaikbk.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gghvaysmu.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gqihsesmn.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gkkqxcrcd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gngbztlop.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfmrpeaod.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gydgvoltp.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gjahsbqpm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/girfoxxcj.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/ghnssvusr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gszlpihst.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gcxbeflsm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gnucmnfbn.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gwayuvgwj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gqecnazty.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gagawhhhw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gesqcwqyj.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gptglbwok.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ganhrompu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwextpt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/ggsrgfbpe.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gdhafczch.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkwnhqlfv.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gkpjrhsoz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnlgtzese.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gghomxkvi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gksqaobdr.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gjchodxot.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnmggcqqt.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gtnskjmyr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gnoinmpij.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gpodqfbeo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gqtjamosl.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqvscgtzs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gvenmigxe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gjmicbztg.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gndlhierx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/grqgsxnab.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gcjbekpol.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gpnbojmoo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gyejqveke.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gvkcgelce.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gcaziuymf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/giylwrcil.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gczaeehue.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/grdsmuzzq.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gewvpukgd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/ggleabupk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gbtnzzksd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gexrqirzg.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gbhklcxex.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gthpbxzly.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gbzznasnx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gwbcfrase.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gypzqhbrq.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gcxizmwkq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gwwggotue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gwxrygseu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/giggkqwrs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gbdjnzkzy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gipddgvol.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/grnbqkabs.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gaioozgdd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gxgzdfacu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gwnvpcwyz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gdfsninqm.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/glyaezara.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gdeejsqay.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gorgckmtn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gyzpzsytr.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/ghgeweoxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gfplzelkg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gkzohmwjy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gfvxcudno.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gdlwkclji.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gnkhnhzbs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gdxerleie.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gjcmchars.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gxhoptmkp.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gfuuwzkvj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gccfgozkm.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gnoarorea.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gplscruxo.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gvwtevwlc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/grtyygetu.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gahkmhnor.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gquatqsop.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/ggwwwfgmy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gauxdnwdb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gwsxcafbc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gapjmmgwg.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gzpndzosq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/grrtsilor.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gwyexnvln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/guljdmwpo.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gjhvygafd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvczzfuyu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gbshqjwyw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/ggakalxxm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqutgqcxs.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gfuoobayt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gknfufqxb.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gjwhdrybq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gdpuvsbsw.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gfkumpwii.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gkspkjdcs.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gcfebbfmz.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gnffegjpl.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gemdhlrvg.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gxmvsvaru.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gzzrworeo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gdwxkzogz.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gpknlasvz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gvdwiadrh.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gcpyoqiky.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gvaslzdfh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gxubadmpf.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gtaaledna.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gfsibppmx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gppegbyou.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzzowjanm.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gturggeyg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gtloochau.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gxmqafimj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gejhefxse.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/goyojirjv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gjbnnpyvl.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gqbqwehuk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/giygsvpsn.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/glcmzbdck.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghxapcnjq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gcuhcghym.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gaiydawrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gidktqtyn.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gijoefzeu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/grbuumklw.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/grzmyjtju.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gljgizywd.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gfiwrpimg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gqnpeixis.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/glpptjqbj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/grhsalsiy.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gauivdqvl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gepeglhqg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gtsxbgbwa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmpxixpzy.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gwxlufcie.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtidjloew.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gixnezeyr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbnyblelj.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/glwequwpm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gfpksybvn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gpljpkzef.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gbomzptms.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gixqoqgqy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gubmfppvs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gyvgqncbc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gqgnwmxqj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvygxwzyy.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gtrukdwng.sHtML


<!-- 参考信息 -->