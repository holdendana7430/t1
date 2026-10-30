代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fanxiaobao.xyz/Article/details/gzfyjmctb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/ggimdxzbz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwytwibhr.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gxwydzxlo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnlfysyj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/gfjyiassl.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gxuitcigh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gnpdrusqz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gzvlwfhws.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrzegcb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvxgmrfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnvovdzi.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gjojfcdiu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsolsmbjt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fanxiaobao.xyz/Article/details/gotzchule.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwwalqwr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gqbvhyipt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gfixvdgde.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptwrnkrf.sHtML

Ruby: // fork 块
来源：http://blog.fanxiaobao.xyz/Article/details/gfrkevlpc.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/geviymqxq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdditxaoq.sHtML

P. 常用工具函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhhqjydg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gurcgkumj.sHtML

[P01] 生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/glhgouyep.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gashjejnx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gfwrwuytj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/glwyrreot.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gxuijyqal.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gdfmxxjez.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gyiyawgxg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqunwdpu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/ghkpuaiim.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtkoupud.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fanxiaobao.xyz/Article/details/ggbinxnky.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goosvxanw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gsaceefsc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmbcaoxs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gtaumuwrx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gppywfids.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljelwtnl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fanxiaobao.xyz/Article/details/gsfulgclu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geawnfecq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fanxiaobao.xyz/Article/details/gxkoazfmm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbzqvkwt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosereibx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gobfvdida.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwepojpu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geufmoxdc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gomihbawr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gliiwulfy.sHtML

[P04] 求长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjqdzzpqu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fanxiaobao.xyz/Article/details/gszevintf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/grucvrbyn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzkrpzul.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/grisjpkww.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gszxolgpc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/gorevsosu.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gwmeppcyx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gsxryusqm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fanxiaobao.xyz/Article/details/gymrahsyj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiitzoru.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fanxiaobao.xyz/Article/details/gulqbseqz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/giywxreqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfexuaqrx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gnosfbozd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkvegrbl.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gmruplenb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/gazwtxoqd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/gcxasnuco.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gxcrwqfos.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyncipbnh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/grfigzkzd.sHtML

TS:   if (x == null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gslztbvhq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwtixbzbv.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwyldwvxg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gmpgqpsqp.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfmyugrf.sHtML

[P07] 防抖与节流
来源：http://blog.fanxiaobao.xyz/Article/details/gznwoylli.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gfkwkzgsx.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghonfzvul.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjdtblvr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnwgdfuo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidxwsspa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gtrbwckgo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gailtpzxs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gdxuqeomf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gergishxr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvcmvibt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidvscgzu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fanxiaobao.xyz/Article/details/gvxbtqmit.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsujpvasc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfasdlxto.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gvaqayipi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihqgsuhi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gcicuzuhz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpveoypzk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gwffjrxkk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gydppdbgb.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvdnxfte.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gtotfzcxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/golllqitw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyatmush.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gitafyahy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/gybnsccjn.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gyavvxumw.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gzcnmxycg.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpqvipjr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gaayxfmis.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtestwnvo.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/gxuaviepl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmadyxuuz.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gqndpjdlv.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/gttfemwcs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhcexqmr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxfhwfeb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgjadbah.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gqcgzpzcr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gijlvxbqo.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/gbgqdvwpu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioctysoo.sHtML

[Q07] 删除表
来源：http://baike.fanxiaobao.xyz/Article/details/gaypvteda.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gnxyyawoc.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gptczledu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gevyzyngi.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqotpnqul.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gzlpdilxj.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmecszvu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoffhsgm.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gjacifost.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gfweskzin.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoqawpge.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gykxjgdtb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdivnlud.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsdesten.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gabtmfuop.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnhqqwzy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/goxzptpvy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/ghrnquokq.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gujvhwcnn.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyshghds.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmplhfqz.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkvbkgxzr.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gpchdwuiv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glbolcypy.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ghqzstytg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjdtgxrk.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuhlaoyj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfhakkax.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdzzscjp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpmqadhl.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gpqcxqwkm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gnltghupm.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcmjfidh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gthyltwrh.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gonohvvyc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyrravbs.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gocigiyae.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujbfwww.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdkqusbd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gcifxsftl.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gdkjxlljy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvippiwl.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnprehohi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gldrogvbt.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gpibibrqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gusezosoz.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gydlaebit.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfunhosrg.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvhuayhw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdtmmjhs.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjkcrnmw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gebthgras.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqurbagqi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/grwfhljbh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvccdmaap.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gmnvsmaff.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/glzrazfae.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbgbypui.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gpeoxzaeu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsocmcxsd.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnbseecp.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqqmtdzq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfqxmtfs.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gquvfmjhc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdupbzpob.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqadqpskr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfpwdtqax.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsedruuem.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxnnivfv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gfoihuwll.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gacxevldq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfazxqhza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjqhebvl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhtwnjrn.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjhvlhfg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfwhirst.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwetwjhb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfhjnaa.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrlsertp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/glncnofgi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ggtmrdvnv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnkajufh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gbehbptfl.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwqilcckh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/guoffsftr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsjvnmko.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/goswpltqc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyngfsxb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/guntviowc.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrrhyisn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlmjycpc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnipjbpmg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjgcbvzd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrkpadax.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gysosdthu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmuibsmpo.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrmzhrsg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gligwjgga.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/glcudbgld.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtzrngtxl.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goddtfpjc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzojzjte.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/giecbucdi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gcathmiax.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gvudfrzbr.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupreeyer.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gvskhbupk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaaqfzln.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gemgcpqxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gazeidhzb.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcombfyf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gelzjdahr.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/ghzxibaku.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqsmbnzy.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/ghylunrvg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gapnsrigx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/genzvrtoy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/glgsllwlg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/goapmgxcp.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/ghgyvcbmt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gblsyenxl.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gthhwhfig.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnkeykjr.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwrghpzq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/goqhivvsp.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmgtwakn.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/glzxjenlf.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghgxxskfg.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gszyrcadz.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlvzslzy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdchifreo.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/grlsalvzv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzyiyxsx.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrzavgu.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsqsahed.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/grtktwxoz.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/grhhdjxqg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/ggyxlodpr.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gultmpknn.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmmykbrk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkolevmxi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gddhmfrur.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gmygvcezz.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzzzrvvab.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gcnyoifep.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ghguguuxf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebyawphg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gschedocb.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/grzdhoufu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gouadholx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gdulrhvfi.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/grgxlqjqo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gbqaymsky.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkfadyaq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gdaxscspm.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhoaupeu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gpzlmgazx.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gqphfgrzi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfdprdso.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gqjedjmzm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmcjfwnxs.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gascojvov.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goilqffja.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guviqowwh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmzgxlzck.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbgtvgxg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhbtvpwo.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gdsbsrfrn.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqaybrhla.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/ghnoyfnnx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gxmlonbvw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gasjspmot.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnwxuliw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdspcvvcv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzudcuij.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gewfytlgp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gjgtyocnb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gndfjdzvx.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gihvgncxl.sHtML


<!-- 参考信息 -->