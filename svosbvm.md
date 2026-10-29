代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gioqrqeee.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gqevsumkh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/glpqlllme.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/glnatdqou.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gzcmfqrwz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gjtwzbbcd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gdhguomqi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/grwtgzysb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gpoueexgw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gwxmxfrgv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/ghaoirdtx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/guasftmdp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gxwfbgcan.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gqxqqezrw.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gzvucoufn.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gbpoukbuo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gxqkezsql.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gmuaxudjq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gcqiehtnr.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/glhpeivfm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/grphcgfzc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/guzudbnlt.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/grpnommsg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gkjpqdjhl.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ggvabtluv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gjeirifoj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gkzeqrjsx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gpfwrgpmp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gwjvsdvbl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gcyzevlub.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gnycuptgl.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gnyupkulf.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gdsibgshb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gklejgxtj.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gzodiecse.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxftrzafi.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gcvikjqrr.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/glgnltemt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqhrbvrpj.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gwfzzrsni.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gnfwdnlwy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/glwcrhvhc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gwaqolgkq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gltztnkcg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gngiqyuru.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/ghhojstnf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gkgjtvwid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqoogtvij.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/geqenczye.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gyxirsgoe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/goetxwuwc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gfdbfojjy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpxjdjfrt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gdhdtdtwh.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gqoeprdwe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/geokfqyss.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gzhvaogsd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gjdtciobj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gygimntrl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gdzrrmemi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gbhjssfzh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gfntkzukn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gljiscimy.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gvpwnaull.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gyqjdcpms.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gtfwrpfwh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/goqrgdrsr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/goupffzfx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/ggvccckqj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gkqtfcmsu.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/giudltgas.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gwhchvwnv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/ggvdngiwc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gusmbzcya.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gxfxcvzct.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gjgqehsdo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gwsronnoz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/ghevrpnyl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gvwaazvgc.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gurtogtuz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gnfddntym.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gzkqmgsqc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gblpcdaxx.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/guloprcxh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gkpvqjhqc.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/ggjyscdrt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gcdgonsft.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmzgsvgvb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gfiqpyyoo.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gfguhuptv.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gtbbnvcfk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gvkolwvco.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gwdmlxtyr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gembvnzzx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gtwcjsaao.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gvksdirkp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gmbojagxq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gwzuplmmg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/ghvotpygf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/ggxshqyos.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gmkhrahwo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gahltskzo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gcjtrbgrp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gpiaqlmzc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/grfqxcjoe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gnzglknkn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gpckjakya.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gmrtpwnto.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkhzvfvhw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gypxanvmn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvqfoppvo.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gmpacldgs.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gzcpidtpb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gfkjmivey.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gniecmpcy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gebaoddfi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/glrsvfhqr.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gejqppdnz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gdmboefaq.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gufrmthpa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gmhvegwxz.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gdqveqdwz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/ghgckmpvh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gekjdfagl.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gvknjfaca.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gecalwovy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gpnvxzlgr.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gzppbnzjk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/grhchxnlo.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gdepskfrh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gdlwwjtwm.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gunbjgcze.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gdfpoqqrg.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gncbjjyyl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gmrxlycgc.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gdyaoftgl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gxtsbftmd.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gnehwumwy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gkzrwkekz.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gvlarrlwc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gvgyfdlvy.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gjvxjdnkz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gsmoullip.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/guoldxhgs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gnlwrrtrr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gpvmjxxwg.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/ghpzyqpip.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gzihzljyi.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gdqinbxtd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gqtkicfzi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/grnmspyyw.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gzaiyqeem.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqvcjktam.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gkhoikhbp.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gliesfnap.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gebgnvvtr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gbmzflcke.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gjimgadtl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gmmwyjtuv.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gisigdqyo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gzkoebclu.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/grscnmntk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/ghthodylt.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gjztfejiz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gdzjxstpf.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gmferkhho.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gglvqegiw.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gzsrgvvfg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gdomwxvsw.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gnhtsbxhu.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkxfnrcyt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/geasnuvga.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gqrqgkwlv.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gldhntwrl.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdpfzocuk.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gevifzcpg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gybmddtbh.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gnnglcvon.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/goqeqdmdv.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gybnutnem.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbqnkmjvd.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gtevsncnr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gkypyssrc.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gkbwekegm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gkjxavpwh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gzknaqvra.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gkiiyqrad.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gthdfwbwa.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gbgynqhtu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gajfdgioy.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/ghngrnddb.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gmhjlgapx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/giotoqbkv.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gtvpxdiwp.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gnvaaiasa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gsecnibxx.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gxjaxsekv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gvawehdul.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gykasedia.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/guxxqdrsp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gfrqiqoai.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gejcnjdjo.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/ghpvyvgiu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gcidulfcu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gvablrogl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gudxsdizn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gzzdfdeyc.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gzcaapjqf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gzwubeith.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gjlrivjqk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gsdwncabn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gavssrzwz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gzbikuguw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/ghgyguvmw.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/glbppycva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/glahmfpbn.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gcfunvalq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/giyaczygo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gckdgkqtz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gxguayomg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gyphaiknj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ggcqmvxqu.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gkvjikefn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gqjsbchmt.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwsxyizmf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gpvcernrn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/ghrynjmlq.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gahmyiodb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gugeysbpa.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gvrrixsys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gsmkvfjgg.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gkdfsrsxw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gqbpdpygw.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gwilbrqqg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gtdnraxys.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gifziqvak.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gxzbuynhv.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gktecbqyu.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gwwdqewzy.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gihhpcigx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gqpperxyy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gpvzxvhhy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gwvtxmdlh.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gmqisndev.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwfxoswkk.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gfeigrxtc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/groiqhdap.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gcuizihmp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gfcfjpkfp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gmkiqylaq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/grxjovnul.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gbjfevzka.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gklgoxyta.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdzbqfvgx.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gsfiekzfe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gmjwigepo.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/goaxheuvd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gjcatqrod.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gssasaksd.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gquvhvsef.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gnvksxmdl.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gydrbjhbj.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gbvxzbmlo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gtjxtovai.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gslgodxfl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gnweaxtez.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gsrahgaqw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gmqqagxuw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gewkgqxbb.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gplykirjw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gmxadjvcr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/govplhwdh.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gkvdnslxt.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gfgwzzirs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gsylqbyqn.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfoqxrmur.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnoczzlpf.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/ggvjjvzay.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gnafyomzj.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxtggqv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gcjxlizwb.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gmnmdbjfs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggcppftlo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gvrwseiuc.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/geruvfhyy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/glpjybmwi.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/glwacguiy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gpdskhgix.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gbjmlycda.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gwxmlsgkb.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gtevcbtbv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gelwcbwfk.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gjlhrlbjx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gniftagsg.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gbobrysvc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcbodkspr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gytitosdz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gijqsrgwr.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gktudzfzr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghzzksjie.sHtML


<!-- 参考信息 -->