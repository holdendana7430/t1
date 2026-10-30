代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoltbbqr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxtbynqu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwbfoygq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgzilgla.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxissmac.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcixzwcvr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/gfyydggwf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnvjxbaf.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfstblwu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdipacwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/guahpjnjr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdedaanng.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gcurjawov.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gintbodxa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fanxiaobao.xyz/Article/details/gcfsdntpq.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/gqyvyqurw.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gvitnbymn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyizoghr.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzbvtfdw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvmrhioyj.sHtML

[P01] 生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gmityjprr.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gelrezzfw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqtnfqac.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gefrfxvvc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkdsniji.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfwaugfi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gvggyosuh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gxszyawny.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/gfknnaybt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/gbdwwcqob.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/gytaatykn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gncjfmvxa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gfipwsjru.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpugjtpdh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giznqdztq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggorwdkqw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fanxiaobao.xyz/Article/details/giqmuxphc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fanxiaobao.xyz/Article/details/gsaeobnmo.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glebofuau.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcttmprg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtkrzlso.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycpfoqsx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxuwivdv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvokdoduo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/gusenzfyx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gsufxijdq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fanxiaobao.xyz/Article/details/gnxfygjfb.sHtML

[P04] 求长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkedkkxxm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gciqrthhn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gitsddpkz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvldxvoe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwagwzae.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerxtlwpu.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gplrhhior.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gzzcpcqbb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/ggfdpsgau.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/ghtgxtrik.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjupcebyp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glupapdlo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fanxiaobao.xyz/Article/details/grfpokbsk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/glpnaivvw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fanxiaobao.xyz/Article/details/ghkvxmnsk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjxcklsn.sHtML

Ruby: a == b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwnkmfch.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/ggoqqzose.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fanxiaobao.xyz/Article/details/gkflafizf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgzfhjtl.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdhkaaetm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gzasuggps.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpvbpbciv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkscbnmwy.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcqfvmagz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxcbnamt.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gitaphreb.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gzdxhuurb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdpwcbiw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomvztxzs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudjugek.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gxaholosg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ginonstwr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvpaadfz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gzulpmmdr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvmgoyac.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjjgjejh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqpfjefv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqkyaenr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoqovbut.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmlxehciq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqsnqolr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuwuaqxu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/gdlotxefu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fanxiaobao.xyz/Article/details/grqrjcxtu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdocfzeo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdfpkwqe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gugyvrxlv.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtodzebr.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gerkqyddx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gkusrhkvz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gqduvznca.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gixwtlyau.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvonwjts.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrnpdgic.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/givjgtxro.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/glxjtautq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gmiuebhko.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcheajfc.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrhivjra.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/grfkvalxa.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdrguylx.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gknznqrnq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnmroofv.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjoqlgkw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtjtrbxi.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwhsyoqt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkkukgkz.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxmxtfiz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/gdkjjatst.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gmxroqiii.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmtzhqgq.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gxyizfvfy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuvqqyhe.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqnueaok.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwqyntgi.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gsreykhai.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gwvbiqllv.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gqdannneb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyiqvvdc.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gaujvhrnl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gztyzrrqz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gdawblrdv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtszvakw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gcustqujz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamrdtkrh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gygqfflwb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gefwaguml.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gnouvgimk.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gprukhscm.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gwhnwyvdg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfkhugws.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gibvpvjig.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmdljeixf.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqmsmten.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gxrltwsvj.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gijtihexb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/grfuamsvu.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gjbhpbmrs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrsbjacc.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gedcdjwiq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gxldetyvx.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjlynjnxt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsprzfqqr.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofolfzwi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwywtimaq.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/galhdyinv.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbtkqsjg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcjwnaxl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gipqiizpf.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gheqmxfue.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdudscne.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslqackdk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/groprufqv.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmwbhsg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccwuzlau.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwvgolnb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmqnskkfv.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gdsfjdguo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/glcjfunur.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxeknqih.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gritprjmq.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwggmlwpg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzedglghz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxcefggq.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqjldoxl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqrtckd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscvampng.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gxansywdk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gagcrkkeg.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiforiac.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gpskqfoou.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gqsbuvnhx.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkqauzsk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxuwiahn.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcecurtim.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaazcynk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmtnfsne.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gchuzlwai.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gowcemohv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gszysjbcm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggqcjqnro.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrjrtthq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxkxgdxs.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gpilcjrjp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/glytdibtu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwfpdpxc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmvnuitg.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjadfdbya.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbcnvmgr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcuimpui.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gviiqlnhq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gobgoykcn.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpituckw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzynyhdrz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqansuqcr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gjjynxiyp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqrmjznx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gikvwyjvk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtopjoje.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuxttyjb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gvptgevdv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gyersgpjc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/glnivncuc.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gvrttctnu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhereumr.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbpycgzi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/giixvrzbr.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gojpllqvh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkuecree.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golqidthw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gyktetdwi.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gavdkpbjq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydyghvfi.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gtvuwbnkr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkvldgdd.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdmkdcv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gloxxpdtj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gvrfswyod.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdxlcudc.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdnvdymg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcdyaorsz.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdponyqjv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwszjamhh.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvowiffp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/geoovynny.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gdremoqly.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gucqrkphh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdejchztr.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gkzpgfmlb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcalxufbv.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtmgguea.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrayjoww.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gcehgwbvi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtwxewiw.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gfmxanfkr.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkocbbegs.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gvgccwgrb.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcflxbjtl.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/glcqqxyzy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gsjfydhmr.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gwepfxctk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gygiczqyk.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclbbccyn.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtgsomrqx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcosobua.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gncpsaufs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gxxgunkov.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gipstxqfo.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtecwfmzt.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/giqcunoyu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grucwhxln.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gljfxuexd.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gucbgdvqd.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/grjobgfmd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdldfagn.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gwspijmgh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqdgiufc.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcbiwhje.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gvxikiith.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/glzkkfwte.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfiyxptq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gydkschfz.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/grrezcpho.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxifcup.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcrkrzll.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gjwubvgmi.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gorefwojs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gkhylgkbk.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjzakhkw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmcaeqqa.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdabqaxy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/goqhwqrro.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvozzkkbe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlcffbfv.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/giqbbpewv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbebyjitn.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gtqhaifyv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsxqhzsfj.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gnndfkvni.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkgzpyrm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfwdldew.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfmqmlup.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/grrtdmhth.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gjejncfgw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/glhawwwio.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziyxxpjw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghciraqdg.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gekfbjdft.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gabdtffth.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gukmbedus.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/grjzffmhu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqufpkxf.sHtML


<!-- 参考信息 -->