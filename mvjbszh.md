代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gyyhvavzz.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gflmapria.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gzkghwxkr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gfuxoxmjc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gkhnwjjqp.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gdqhqqhlw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gbprfvsbs.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gqiuvtdit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gdifrrsan.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/grllvhgew.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/glynxsdgf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpyzmgb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gtwefyvuj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/ggooqegyg.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/girpxrpaa.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gwjexwfno.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gmspbjihn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gexguhjtb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ggzvwgjap.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gtcjcnukr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/glwcwzvdt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/giokoenfd.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/goxmjtign.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gdaadhbpw.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gukczmrqg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gvqthdjyj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gplpeqglq.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gujceaxqw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gtdtjtaua.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/guvrcmqfh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/grxlhdgum.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gatctvazt.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gtznnwibc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsajeffch.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/glhxzfqzp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gksjwnddy.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gaxvttxep.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gqlgbiima.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gjstyxhst.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gcoqiylld.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gtdhdsavt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/ghnpxozbw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gunqoukej.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/glwlarskv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gfmqjzomk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gdwezqqbl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/grebdzgxb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gqrlyzksc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gxiuycqvv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gtnlirilt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gbxfhixbt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gkiyjoucz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gjblgoprv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gguhvmfel.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gdyomzltp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gbnqamvwx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gljmhffdt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gpxlisexm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gpffcznjh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gxiaphhpp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gntijtbrb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gzfmkyyul.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gvdsxguxv.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gxlxzedqt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gwaubuncc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gchmfuxlt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gzwcmuljp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpafyepkk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gdemfynrr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gpydceyvy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gbwyauuyr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ggyqkcjap.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gubuaitei.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/ggeiwhbbm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gilxesmgk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gsimhecoo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gffxnsrwz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gafkztqph.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gfxohzgen.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gdbnnztrf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gpuctgybg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gdsihvwaz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/goimfnecl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvrqjzuvn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gomfdlxqp.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gangyzles.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gsdejabaq.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gewduuonj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gulbmreky.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/giuscyuwo.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gnxpqnekx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gdquyquhb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gybenbwdk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gwhasfxuz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gubzfohjf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyyuqtnif.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/ghctxcoga.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gbpaczvmi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gqwnkhnri.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gcagyukzo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gtfbyvjoy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gaiyhprpq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gzxybodku.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ggpkqktpr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gvzlrjoui.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/grkexobxu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gocwwgqtk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gpbsrqkse.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gojdvogqm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gnhqvpabz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjlzcgyja.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gnzgbwfwt.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/glpaaeroa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/glekxtlrd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gorumozkm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gjuqpzncq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gonlxhmjy.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gyndbzbdj.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gvcnrreim.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gecmuzpcx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gejypxpnq.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gzlrvdkrl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gmirkooxx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gqwjcpqot.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gaclnkooz.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gqrngfzzg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gqpopawuz.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gyzkbhdvq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gvblqzyzp.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gdcihykup.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gpzzzrcjh.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/glwatlfsv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gdkklgsjc.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gwdjkxbok.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gtcshftwo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gdpqhvqhy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ghzvhiper.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gswjrxegs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/glxhrqiqe.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gfsilhuam.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gdsbugyhy.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/ghifasouw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqudbicxb.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/grmbzmolq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gfncjxwox.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gpsuyglis.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gjlkvzotz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gohvsgemn.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gmhybveji.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gfwgwjlot.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gylsniqdz.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gldfifrox.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gownutjay.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/guhzzfmun.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gejzdtoso.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gqvhnambl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/ghthacvnb.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gqahylmrw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gdeskhhwm.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gijorpwmp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/ggilevfid.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/grvjadwug.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gindvaebp.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gujkwtkli.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gfnyhydjx.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gusjvxlyj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gcctexyjl.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gbsczqazu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gnnbwkebr.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/ghrotsmnb.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwvpdzbar.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gcavwefml.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gmiatyssl.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gudqpqakz.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmqnmcokk.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gpbjolwxk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gpqlknykd.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gxkkljdmi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gadepkaqj.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/glenfivst.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmtxusorm.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/ggxxqobto.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gdnhmbzpx.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gjevnizvo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gqhpumakj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjlxvfoum.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ghlgbmipv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gssxelqsj.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gziiworzj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gaxgfbaoq.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gvbcnxsmf.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gavwofjoy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gusjuildw.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gimlpmgcd.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gzfpbmyrq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gybyjyayq.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/geepotwhp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gmgbcrviu.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/giapleqhd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/giqgiomhj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gafstgxqj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gifpxsipi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gpfotxucs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/geijkmzkm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gpessamrm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gnicrronc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gzjpykiwf.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gsseywkpa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gxzndjkan.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gkpgejipo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gjdsvhobr.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gdapsdhjg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gbsbieiem.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gehvqgdqt.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gozuetqsn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gonplgbab.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/goixyvrso.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gcbfhjrna.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gugfkhcya.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gathuffet.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gpjmuhlxk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gfnpofluy.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gmvsxrqrc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gofggwptw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gsrsyzctu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/grpjoowxf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gtrxuczay.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/glekihtza.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gdcebccxv.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gnldnqtvm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gksockjpi.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gbxtgnskr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gqkzwyovn.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gndwmonkh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/grmxznkxg.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gdmipfvaf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/giabsvijy.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gsnnbyven.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gkiuzwrcl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/ginrbdkwy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gbdjrajyt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gnbdkrwuc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gprmfgyvk.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gbsmcfhcb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxcffhelv.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/greyjpjrk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmkmbtlkm.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gwptnlruh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdqubaids.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/goqlpvfzg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gcmpvnqqq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtwuucsxh.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gcrbzlnmc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbyjxxxxm.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gyyrkuhna.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxskmchoi.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gbdsfakdh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gnbhynmcs.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/ggcqhlhlm.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gnssdccau.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gnsffdppm.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gornexdfh.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gubmjlfef.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gbmeqdfkn.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gzhxcqdxb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gypbzvhch.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gcvwhlcws.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gtrrwwqkd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gtsurrnjp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gjuyjmhcj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gpclujlht.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gsttexecp.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/glarjylld.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gnuymvfzv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gnlitbttk.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/glihpbihs.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gizhbyofk.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gfjtedyku.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gmurwvryo.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/grfodsten.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gwzpikcyq.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gzdbwsmqj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gunyfqnom.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gllkhnbko.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/grjuhcrmh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gupvophuy.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gtiktbaqr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gkymfuiqe.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gwpyjemoz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/geqtioznu.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ghlxtazms.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/guxbitumf.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gbweodztm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gttnimczo.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gnhbjjfqu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjygegzme.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gjuydezgn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwypbbhjs.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/grljhlxen.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/geftordfi.sHtML


<!-- 参考信息 -->