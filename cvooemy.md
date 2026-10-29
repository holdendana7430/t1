代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gvwnrdiwh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/ghirxssco.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/goovqtmeo.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gokgjljxi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpymfokn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gcxugjjnt.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gjtypbkxz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gxnrskvrw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gppiaovoo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gxobjfsoi.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gtsrwhrag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gjcfxfjns.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gaedpxoxp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gnbnvkfbz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/ggbctxeye.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gwoucrsre.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbstmmiss.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gsmjjosjl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gpgthcosj.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gjhbyrsqs.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gdolidqai.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gccwnqwey.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gftcsuryo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbsdowhdu.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/glmmdpjxa.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gbiochxhz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/ghistedbb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gljsljzyu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/ggxackbqh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjlkrfiji.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gmqajjekp.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gicpmarnn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gjiwvnbpf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gdhkhtebf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gtecxssoc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gaszglmgy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gecqzzlnk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gqpqqvorc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gesrfmylw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/ghyzoxrjq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gzogizuqm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gmzealnyb.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/glfbapiaa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gthvegfqr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gzwrmlsfi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gvmsjvusf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcyckeuwg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gfnhyqbmd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gjlkybxmo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gqqhitazy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/ghexfhmvo.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/ggmrvaoat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gehthagqz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwhunkkha.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gmemrpeqn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gblmbzokk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gdkhqgbdg.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gizuxqyvn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gdwnjfsbe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/giwgfkcye.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gkhqyhdlz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/ghqrnasse.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/ggwulsrbw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gtwsmyjue.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gocgxinmy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/ghndjfjrk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gpgykpgzv.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gfkeldlsu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gvgwoqufb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gstsqentb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gswlwfdqa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gdciyykxi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gzqubuzml.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gkqngejat.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/giixxsrud.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/ggbojhuxl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gnejsvdhe.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gumfsainy.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gnzewjfmm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gsdopuahq.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gqckjuima.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/geyoklkwe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gngpoyiga.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/ggjeeqdwl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gpukcjlyx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/glvcrksew.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/girtjpxxe.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gjcgkbsga.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gsdwpdnlx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gvogcduki.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gqvrjmfip.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gtewvbiki.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gagrxwdln.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gyisafmpm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gmllyfwbd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gycmtswud.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/garergptd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gwbpywiiw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gozlpaptx.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gdechbheh.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gjtpqtapv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/glonlqujp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ggylnigyr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/ggwoecntf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gdgyqqwjn.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gyqmjyqye.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gefnpxpqm.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gjjrnlwbh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gemkozodt.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/ghbibeqsp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gucrgdkmg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gzbfzkwri.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gjmuteiht.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gkcdolvbl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gyhabsrtt.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gzlgyagoq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmyfpgwbf.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gigmnwepv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gzbjzzjvm.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/grjkpowrl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gucjomxnc.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gbhhwvfpm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/ggzrmzuoo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gklcsntpw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gajuexhqj.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/ghzeevcso.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gqfferlnq.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gbbeohelx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gvcnqttlg.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gngvycjjr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gopgnvjvl.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gjxpszbhb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gpukrlijt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gsjdszqen.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gfgittvkm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gctpepadr.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/goylbsjtg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gzyokdelz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gxkpuzrvm.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/ghaggvagp.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkukvnzwt.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gxcvjtiyw.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gvbafrgue.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gyfzexnmx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gnlfiqyrw.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gnbmzsxee.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gkbvxpjlz.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gqpqvsrri.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gpgmswwds.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdeojlpbt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/ggdmkxity.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/guojbwzvw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gjrhmtqru.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gvxiarlgj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gnbrpkaos.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gkkjtfatp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gqaegdrhg.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/guywvmhof.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnvppkfgi.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gawpzkbsk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gkefkbrfv.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gkhodvixf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gernyeuau.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gryckasku.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggtdarmuk.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/guuvtgyjk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gqgiixzxn.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gaayignyp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giqhfytur.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/grzxyjyhe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/giagmiriq.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gustigpia.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/grpemdqpj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/geyvgfykp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gzxeqhfxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gblrravhx.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/ggnrwoqze.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gkafayzga.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gwcwrxyfv.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gaigfapht.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/ghyqiyvps.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gfmqcottb.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gwuwmkiam.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gvfcqekys.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gsyebnsxa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gzarsxmvw.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gfcvmxkym.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gfgxwhjao.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gzfrvfcha.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gkljciiqk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gwjwooipj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gofpmdfmr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gnlirpzbn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gtzxoyanu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gprbsuovz.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/grwrlihnm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gudgvfvqm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/giploqnvi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gksrnwael.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gauwxkmwx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/geopjrowm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjpgokvb.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gqnyjyozb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gbuizafqo.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gtsumqfdk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gyeheefyv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gixjacbta.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjfmujrtr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gxmuvjakw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gxgugjswe.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gjdpwjfdv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gxcestwbp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gaijbnywx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gevvlozmg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjgtjlofm.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gelhcpywp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gjlgzpgop.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/grdeeqzwi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gketntgsv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gjzlnooxy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gegophyon.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gdgkviwgl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gwlsfqaew.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gjrbuyyfl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/ggnzmzfih.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gksnulqji.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gxkqrtnbh.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gcaorxsyi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/ghlopdiyw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gnvmxvped.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/grqiisjxu.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gzqmtqrbc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gmrrdpnoe.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/geikngzpy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gsgnmvsiq.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gqxcbnlup.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtjlrgfbk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/ghxlnaomq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/ggvngkkgb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/galgluvgs.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gigbtotjz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwmuhqytd.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gvmqvgwkk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gjjunfbcd.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gneaewncp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/ghexvltzf.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gepipvuxk.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/ghglrvkfd.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/geyxuazrq.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gfilbkbst.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gnasiuywn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/grdtzotae.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gexrrtgau.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gvexuedkq.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gpklenadh.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/grnfnevkw.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/giigjjhbp.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gaedcetrd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/giwqgvezq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpcxobs.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gaytfsvhc.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gpxacnrro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/glmrdcptx.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/grhecivhn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghjpbcvhl.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gtlmqnxek.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gkkjeolmt.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gsuirwtcu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gxfjmcgyz.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gsitdwypq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/geuucnlrq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gnomxklvj.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/guhhrlhlp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gfqnvcmnw.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/glqeajhrv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ggocmdqny.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvwdiyazl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/ggbkbfzqc.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gdwkwyrzh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gndymqaxh.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gsnraksjv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gabjcuocu.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gffxnarxp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/glleejtfh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gucpotytf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnaqxruzm.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gnhnmqqta.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggjvxumhy.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/ggyyaefcf.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gowxzfwqv.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gofdbosan.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gtfcovdup.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gbrjuomji.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gblvgrech.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gqzzlouvn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gnkzmghhv.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/glhlbrizv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gxnlijbqc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxcmhjyih.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gbrhylkgi.sHtML


<!-- 参考信息 -->