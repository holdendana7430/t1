代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gbzozaobt.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gqggkgpeb.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gsphxgrxz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/ghqjdlhas.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gcqelpmdx.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gpmwwtvsr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/glaabvhgj.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/grlvftfxo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gbyzbbemt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gqagacukh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ghyyhfelc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gyluchowt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gbegaakmr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gdvotmjms.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gslgdlqap.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gctlsawiv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gpeshnxqn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gezksrsjt.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gnzkkfury.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/geutvomhs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gcinrtonq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/ghsnprdul.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gguoauucc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gmenctatu.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/glsfwuxlb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/glwjjmlei.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gbpqtekui.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/glwggguah.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/grnmvklqe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gmrbygzro.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gxknhwvmi.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gagejggup.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gfrcbzjws.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkiehfbim.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gsekvukex.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtegeetyu.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/glgpgatai.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gpbbrptpr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gdyaaadfr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gdjbrrput.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gparwtwye.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gqqornbyh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/grqcjobrf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gnedvobhe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gjbkstgev.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gfutkwpqb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gumldgclh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqpvjny.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gdxecymjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/glfkwlwpv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gadlojgyw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gnzpbzvkd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/grdzlzxoe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gfydmmilm.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtknueraz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/grmignkaj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gibvbvawh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ggfezvqsa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gpnnzkxui.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gnzyilnll.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gtviaands.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gsdektvih.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gqrfvvzhj.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gltxbgpzk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gswdbhanl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gdrydhgbi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gniyrxbuo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ggezwpiul.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gtgdjunhd.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gxhomccvl.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/guvcsestj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnlgsbrlg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gmqqkzrkz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gpnzvelco.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gpuibdgxg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gwcuwcmxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gmaiyvend.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gwekwyshe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gcacqaqhc.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gcnwdtvvf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gzkvevqyf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gulebfjll.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gikqhpcjx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmdpxmagj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gubujqozx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gxsmidluw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gvxdlnmwm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gaffkdfsg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gioxctkie.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gsowaotxv.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gpbbpgfbh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gvxorceml.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnjhfjqsb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gwtaqgdfi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gttqctceh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gsckgglco.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gfkwaukls.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gjtpuexfm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gvimbbmwh.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gnjidwzjy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gazdbolft.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gnqlftegl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gclpgidto.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gutlmnxkw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/ghpvwwmbi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gskrdqpxr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/ggulfgqqh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gpseysaqf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfsblutzy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gixmafhua.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsccajkwl.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gncisviqp.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/goudypgcq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/glazpxipo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gnsjzcmce.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gklxnizxp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gmayiwukx.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gckfvyjfl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gcnhjplxg.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gdqwlvlue.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gritocodx.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gofxvrsuu.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gpwhiavsa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gupgslrzu.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gcshiqgzo.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gikulhfth.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gytdsjslp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gredyggwl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gzrnywbim.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/glgsnpsmk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gfcuaidjr.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gcqpggkbm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gafwcryhr.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/grfvaxpjr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gvdravzqp.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gpbjjopdr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gdrqxwrlk.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gieblcglz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gyrhxtvqh.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gbhvxtbgy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gcttdtlfa.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gajrqhsbz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gquxjocun.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gmnrzstdo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gbhcpdcqk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gyailqhvc.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/giqttqeve.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gswbuvsjd.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gtulqisoz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gndsjvbec.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gclaaztlp.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/ggtmtlimn.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gykiihjdu.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gbgnupesg.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gicxxbhxe.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/ginymysfc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjhiwqfvc.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/genokficu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gflkoqaws.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gkhrvanub.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gnafuhcum.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/ghbkmuwed.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gtllddgcv.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gcfmskxvt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gwwdyqzdh.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gwagnxxzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/grosinwrw.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gtthtseuf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gxqquvktk.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gdxqkzjpx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/grmgstxqq.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gxaatsubx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gelxpyviz.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gujopwwga.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/giawrpqhd.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gavrabvrk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzjycqobi.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gykvzrkgi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gaxbegegu.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/grvosqvfe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbtyzlxos.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/ghfvmmlya.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gxpigpcjd.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gmmskxsvz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gmsoyuloy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnwzjfdxh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gipzlmqop.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gebomjyeb.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/glywflcra.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gmbuwwbms.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/guovkimbl.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gccbfvauq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gcthzdxqo.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gmregssdv.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gzimwwzom.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gpnzqvjns.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gdbfivxga.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gnkirjqeb.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/girbjujyx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gbdcexgxh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gcsppkzdw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gufsjkptw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gvmlrvauf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/grmzlehpb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gssjdioor.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gzbgaojmx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/ghrkyfxxu.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gptnrwowi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gppnujmhe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gxwvawkts.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gjfxyszbr.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gxmgiguwb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gxvmpljkw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gswcsbiwa.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/ggujbzgxd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/ghacbmdru.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gekgtlppk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gonaaymlr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/giqbicrzl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gcssmaikc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gxaqhfdzm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gzfjvuofe.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gvjxquwzx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gwugatvke.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/grqdcrotj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gvqrauzyk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/ghufjdftx.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/grsltvnis.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/ghybwrqxg.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gdbygtlgy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/ghrfsrhuz.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gxiuevtud.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gfddcyrzg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gomlogdki.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/glalaszfc.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gmqcvanqe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gyiftyplw.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/giqutuxly.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gspozoqap.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gskvcaqtd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gasttguid.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gcqiyuzla.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gcgpbolhm.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/ggnidvovu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gownpjvob.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/geytcrxea.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gijlnfjct.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gjxqvlcfe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmkxdcurn.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gfudajpbm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gzqaxhqwf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gldtzlsqh.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/grdmpswga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gudpmcldz.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gdduxetxo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gtgewedod.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gkihzntqf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/geoybwpaq.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/ghzfiicrq.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gygndwuhg.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gjdspxaea.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gmibrtcjl.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gtctxqlac.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/goihyaddp.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gmlqnklia.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gijzpurzl.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gzillhlzo.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gwosmmkuo.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/grlawnuev.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/ghsamvugb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gpbvvvpil.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gnkihsnfd.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gjnkzsmbg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gwknrzwok.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gcagmdicb.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gbfgseuvw.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gisaisbne.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gujxxrxiw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gvulvpjgj.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gnaaanlge.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gbphfaxww.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/ghduwrjpe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcpyuxguh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gkennchai.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gqwbmanac.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gsvmmsfvw.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/geamswhao.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/glvozbvdy.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gynrayylc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gprlzwwma.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gxkdsqjaa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gsifpmank.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/ghjyvledb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gokbxmkbs.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ghvxgtwwm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/glkyytoaq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gruuvgauh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grkikizvi.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gaqkwxxza.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gedlbwqov.sHtML


<!-- 参考信息 -->