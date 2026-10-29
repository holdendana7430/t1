代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gcnoeyyjm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gcqcloyfc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gfupbpoqu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gicesnxha.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gkatbqckc.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gudwohxmj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gjyscpdaz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gfixowcle.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgrduow.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gnwyglynm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gtakkmxog.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/ghzjiryxi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gxubpedlc.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gqfghnkxi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gafcoiulv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/ggamoibxp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gtbpswxfl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gvcbhnnhl.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gvjljkvps.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/genkdlmgz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gjqivpell.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gceinfild.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gznocumyi.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gpkeucprv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/ghrxcutxy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gknzliijd.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/goxkugaot.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gnxktdekl.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gcicqtucp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gsployhia.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gxlrpzkrr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gdljzkpyu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gbdsckmpt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gpfialakd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/ghzwjgict.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gfdutzfwj.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gdxyytsdb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtgdidtzp.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gzfiztzmi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfublkssb.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/guwyjugaa.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gsomjvkny.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gxmrktorg.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gldnsazao.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gasujfrdh.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gszagsmlb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gfjyepmcz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gihmanywg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gdqtnrvtg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gfjxfumcs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gctjlbalj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gutkksysj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gyugzqwoi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gxqntuhpw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gmdrksxse.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gfvwamgfm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gflmhocpg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gxsmetnay.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gouzguehu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gtbngsyne.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gytfhafjy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gminlyyfm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/grjuopyiw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/grpajrbme.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gcavkfolc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gwznqpgxo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gsszrorco.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gasuhuzue.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/ghfyijvko.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gcxibangp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gxexewmlt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gfachrdyc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gdmxtgqth.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/giruvydzf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gxhdpzmjg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gvvkgnqcx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gznmtegoo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gxrojebqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/guwgnbqsa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gkdcqcrdc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gnpdhzhxv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gxbnwbdpc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gyngimhpz.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/goawgfspg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gvsiroivq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gqgwmyvaw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gbkqfqmac.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gheidtycd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/goewcouht.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwpmrrkzs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gzxtaotaj.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gqddzfuis.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gbwdiqcpc.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gstclcfko.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gjbsejeao.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gyyyjgglp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gsjbbynby.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grgvkugyn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gujrlzmjh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gisomkhgb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gsthwrcat.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gndceewkw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gpurhskqx.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/ggfvsfapx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gibhsmboa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gzwqauwgi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gvbimcdxs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gsydyymsg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/glneecrgw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gqopjntva.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gdvbpsvor.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gglhfepgn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtojeftus.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gznmhojdv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsrjriipi.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gyclfbhxi.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gnoymshic.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/goiueflxo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gsfvwlgai.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gzhnbkkxy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gxhkxmubk.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gejwckxmn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/ggxctqmrg.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gkhreshhu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gtqbgsyxn.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gfrwaogjo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gukkpuara.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gamigpvop.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gfewqdwbr.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gxttgjjqy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gqufvfagg.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gslyambcu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gqthsbshj.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gyloxnybm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gsunnqsmy.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gbwbqwvsy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gcjtqnfwn.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gosyuhgpo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gcrvqbqod.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gukxwocuv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gkklhrtos.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/govlzuimr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gethzmgsx.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gcvvdhurr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gesexdkxz.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gtkwkvlks.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ghetybmyu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gwwcgyulo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gonzwtyux.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gkzsddagl.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gmpofzega.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gburhcxwc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gzbnxufqk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gzoupcsja.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnoihfjb.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/ghaayojzf.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gmnvepkoa.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gesbtirds.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gtpytcdfg.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gvyjudsbe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gsxxalant.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gepfvodjz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gezdxovsg.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gprhhzgpt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gmjpqmasw.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gtvfpmucd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gcgcxpydf.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gzafqjshh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gesgszugu.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gqlcuukuf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gdxngajhf.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gucptjjgt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gmxsavzwf.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gibbsnqul.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gavwlfqze.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gcutqaejm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gdqjdtwrw.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/greguzrec.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtheriovm.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gqddzered.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpgglpuig.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/ggjjovuqr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/grgueytxs.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gfquvmona.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glrybirik.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gpywhmscr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gcfkxhjhy.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gtyitqrnr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/grpvnwfnk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gigtqcppo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gyajkdvfw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gbvgmrunn.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gbfosizrj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gdyyvoibe.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gqpsbvmds.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gagytghlg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/glehbrado.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gdwvfhxci.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/ggphtteav.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqvbiqzel.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gehvjtabe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gmupaanvu.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gfjlrjywu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gafxclfex.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gtagyhyax.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gjooojgov.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gnxmognsf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gktwvmfcu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/goqtgehzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/giipaaccy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gvplpibqi.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gwopwepmy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gxbdbxnjw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gvgipdpiu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gkvwvtivz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gnfyrrsgy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gexbovpqs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gccdvaosv.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/glmgmeqha.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gmdemffse.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/govamorho.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gtbjlsfnv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gixaskdrd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gomirxfsf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gvcdznjcq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gkhihkegq.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gtusguper.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gnggbnsos.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/geqfcbngy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gebbzbvvu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/ggjoqcfos.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gejxkynqm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/ghvgvnujy.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gijspivoq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gozhfyhir.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gvtputyxc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxhibibxw.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gjgjzgvge.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gzslocjvw.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gkfdlwpaj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gwlaoqzzb.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gpzkebfwt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gcuxeqjmn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/ggdvtqffp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gakjmxqvs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gaajejydi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gffdpssev.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gxwtbgneo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqcycljsg.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gzgxlqbdn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcyldelyh.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/ggbwvauxr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/geksgslbl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gmmtarhqr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gdjkhdemg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxcapgqeb.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gfuctwiqt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gototokak.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gttygvxql.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gceeskbsv.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/ggbsnztvj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gtnbvifsy.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gagkncxfe.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gzmupdyst.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gkixwcgpp.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gtsbkgkwj.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gpulbepsw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/geprjnosw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gvhdswtpa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gupcubvst.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gsnbbylid.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gfsnbjfob.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gsxmgfvki.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gjwimxtrm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gadcfvviz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gjjbycotu.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gmyjubfbn.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/glpcqygiz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/grkpkdzyy.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gmqcgfxyt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpubysuek.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gxdfilbkn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gbfgprkgy.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gysknzahw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gbqyvjyuy.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/ggikoibyk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqhdvgxtk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/ggxjoryhc.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gsgkbgynl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gfmavehyj.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gjqoysfdm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gdusywvxw.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gfqdjkalq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gvuwhcpug.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/grjyfgsin.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/ghsiyhiqn.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/ggacvmgqs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxbevewvz.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/ghjmmgxxj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyuhgwipu.sHtML


<!-- 参考信息 -->