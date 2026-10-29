代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gnnexhvpr.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gxayyopbc.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gzbqivcxg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gxscmwufj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gsyqenjmz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gczylowir.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gbvspopkx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gxjcuaruk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gcdkmylje.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gcstkrcdq.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gkkdermqs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gbkbidvft.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gnurjynpo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gmasqxilh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gciaaleak.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gqonakhrs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gxcugyluf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/grdhyblrm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gcyqjwpfo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gvyoxqhwu.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gcbomcdga.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/guuvtceor.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gryrhhfst.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gcvsktlbo.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/goxnhraxi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gbucazssn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gwwohhpzw.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/giqxzwcxf.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gorgxnuci.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtlxvkfzp.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gzhwjpokg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gprtqgckr.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gaykyddll.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gvxjvicch.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gezsugeta.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gzbfrhyrk.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbkczeez.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gynzjgjwe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gwcsdoydi.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gyqumwrxa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gtjeuhdjh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gkyyssyps.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gadkqqbkk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gfqinvddh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/grjrkdstq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gaatxezqb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gghsytnik.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/ggfzoigob.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gthywsqdr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gntzrciij.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gfhfyeres.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gweiduubk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/ghjrtmsjx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/guqvrrpse.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gjdkwtzlx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/ghrzqcsyi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gjcjndywq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gnzwzmkrw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gmzgbzqke.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/glddenotr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gerrebzvr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqafdoaus.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gymlpkpcx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/guatgozmu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfxxvnrjy.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gzdclvjin.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gjccyglkf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/ggtsevurf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/ggfsikcqu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/guiuscsgg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/glpmjvqmh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/ggrfikdjs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gxolfjprv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gvwaxuvnb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gsnbgfddn.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gphjssahv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gbjcvhuou.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gsidprrtt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gkhhosswb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gekskxqai.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gznmhjomh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsnrpfcaw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/grmudyzzt.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gcdosnlok.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gtbdxscfm.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gmvjewkbj.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gnexaevvt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/giklcvpxf.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/grmxcefra.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gjuzmhpwn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gbrhqgvdd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gtcicftna.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gwzcimxhh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gvoinymkb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gxjiudyes.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gsrvjsxyw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gvfzmqjci.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gmpiqhvou.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gskcwlayg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gfcrwdvsg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gwwwqwzbu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gjuwnlqyo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gzneqwbbz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gifdihuzf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqfhltyha.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gmlostrot.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaanpmfnj.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gbinjnrfz.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gosfkcwdf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gylubasof.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gtfgyjsiw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gkpwiznue.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/guhjbmvcu.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gstnqargd.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/giauawjoq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gyovnvogq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gzxjnajav.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gxwspnmud.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gsxnsulyw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gzawclffu.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/giuqnysmo.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gonjpchhj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gntttnkkr.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gojpyhath.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gmdwvjccd.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/ghkeivvcl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gsjfyaetq.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrcymxu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/glohntgrl.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gpgafaemx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gcmjnvref.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/ghajcfsbm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gtvefxkog.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gflnwxycp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gvecsbodh.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gtjftbifl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gzlefdfzu.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gzhbxanfs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gnrmpgeaf.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/guzxqgvpj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gafxpyaqw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gyaiypmai.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gwlcazldn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gxgtpchou.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gkapdgseo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gyskyxvja.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gphannnif.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gylvvawzy.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbucgjjbq.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/ggjhvplag.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdgvbtflx.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gtjqqhqyc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gixrtdagt.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gzgvmrxzu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/goyrzzktb.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gkqluhhwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gtcgoddzu.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gryefgump.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gbrjylmwy.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gkcbzxemh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gzrjvpcjw.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gitjdebxr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gjgrahdpz.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gzsviyaac.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gephpehua.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/ghsiuuviq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gfjturxjn.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gcievgzod.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gbapcmgqx.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gadmkbvvs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpheeqlfq.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gjbxomxcs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/grqkgbcgw.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gpdidobbc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gslrpxmdf.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/geqemcokl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzdqhmlub.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/godiqobyx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gwjkbxiuo.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/galypivhu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gpzjexsqn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gpcqrhfgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/grvnrxonk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/glcusvjcy.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gnfyeneio.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gjniqzrhk.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gbbxxelqv.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/guqgmbcpb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gfgdjeynu.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gzoirhoaq.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gobjwdfpm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/ghxlrowvy.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gyqhruoub.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gqwyrxijw.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/goxijijkt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gbsjfdjjb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gxigoyqbq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/ghuzcfctr.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gumaqcyrc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gjdxutrfo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gewcfebbq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/geqeeatup.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gimbtybjt.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gxrityrjo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gjgbnetjg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/ghnadneyd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gsqmzivpz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gsrshmehp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gaaxzzizm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gkrdpjdbh.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gnpjviivu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gjilicaxc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gumeqshvg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/grutkqapu.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/geuxrtsmv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gvlmkyrmg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gwwtjaiuk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gvftwxhbt.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/giflhuhhs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gclrdkotu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/geofkoony.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/ghghvuqxy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gawnmlhyq.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/glgwmaiuy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gqcbnpkeq.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gnkpgpqhy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gztspxhbq.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gqpshbwle.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gjpdcmiqc.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gyjaacvan.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gdhunbzuy.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/ghndotrrv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/glopndsqz.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gzztrurqn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gncxlierc.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gyrcqqyas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gjvvurbfo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gzumdpwuf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gpticdsnq.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gevkknvrr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggrzwrvbh.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gftosejxh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtfjakcrh.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gcxhjgbgy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqgiunyjq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gnamxkunm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/guvwabzhh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gshvxyjdo.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gosvvxndh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqtzhmaac.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/goatqruqp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gaflsejyb.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gjwafjnqu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gnmjoewnl.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gztyrnlie.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gzdzxyubs.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gimtsjppb.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gyerkewoy.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gnjsiiviu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gfffrrerz.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gdvqowgmb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gplizsoyy.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gaimqtwib.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gbfhfsbtg.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggekcwzlu.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/giucawafb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gvrzfemyt.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gslphlweo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gaicndndl.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gfhbvgryk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gkvkmlecv.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gcmoqspfv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmbjuti.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/geubxmfen.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gpbgeuzct.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gfmufgnnh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gybgcbzpc.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gtoopmhde.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gnrkczuec.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/goixjfpdx.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gtmfbqcjf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gvblrwoxk.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/glfxyjygd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gbamuquyx.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gavvigysz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gywqbeudd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gmfgqmbcm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gaehyzayp.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gncefeezb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gussrhvuj.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gbesibaph.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/ghladfrnu.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/ggyxrnklq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guakqbdbh.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gxitaxtmi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvtuatrni.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/glfhtnagv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnqjlkrzj.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gexlyxutz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/grmpphrid.sHtML


<!-- 参考信息 -->