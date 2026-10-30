代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gqmpqotns.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gvnjdlwmp.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gfmbqkdbm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/giuvapnue.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/ghtgajlnt.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gnjbnltjf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gydzrmksn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gplhgkbrj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gfxqqmiwu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gvtfnclbc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gwsbaoqwc.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gskmpnelk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/guvewabtg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gfyvjnnhx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gmcjtcssf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/golyceluu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gcshrsjkl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gghtruten.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gfxzmlqoj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gkwurughu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/glzhmcxar.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gkfihabcv.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gjicegbbd.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/godkoxkli.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gfjlbiaps.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/graqhhrte.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/grphojzyt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gneucnnbb.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmghmmr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gmrgzgqms.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gjcjtzzdo.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gdeebqkso.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gnfzinanf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gjarfnpek.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/grrunzmcs.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gequsclze.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/grhdvjdti.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geixydone.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gmejolxci.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfypehaml.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gygbvxfgi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/goantdgyl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gpsduwavr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gmabswlfb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gepxxrwwu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/glbqadiiv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gamadckra.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/goejmssul.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gclgvjfjx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gwajvdlwt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gxbascrxp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gyfinwsrd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gvwurntyp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gjqcqucxb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ghdblehxo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/glnbczlqy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gdzaanwzx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gqadnpeyu.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gqtyjeeha.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gvhknoqdt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gfjcdmxif.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gkiumpzan.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gxejsmvgk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gikrijlpn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gshyvmaah.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gsvnyaizm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gtaivrsyw.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gtbwdkdpe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gajkzibdx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmgcpoxce.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gzfwsizoe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gsupewckz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gpbnucbpw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gwetlscmh.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/giabgtxbx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gizqlrxwx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gzeajebki.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gsbgpjxzd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gkyrismrt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gmkufytji.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gfrhqfbnu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gdrxssspc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gvuykkdxv.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/ghxjjydyo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/ggdisrwxx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gquxzcgxe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gxyommsxb.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gmzrsfamr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gdbcqkshy.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gtxybwdlq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwobzwofa.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gtsxuftax.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gvkszsxnq.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gvlxspcbp.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/geckvqxmv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gpzacolzz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gacyamtkd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gtwlrmoqu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gonctorcj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/ganeqbkef.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gvphjpjys.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gkqgnjacp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gwxbokayl.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gzkrlinqh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gvkukvzte.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkbhhmoy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/ginzqjouu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gojvgqjxk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gumptprfx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gyanacqdk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gbernwnrv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/glisdnpyp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geoptkbbr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/grhrrynmt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guauqocwj.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gfralvdmy.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gakujwfcg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gshcjxdcd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gxnshziqe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gjccewofw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/ghwqxygxc.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gvddsohkr.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/ghdbhfulu.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gbxrycvmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gquatmtki.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/glodxyadj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/guymkpiee.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/ggfkrotdu.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gdpdptqxw.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gdowbfhwk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gdeqcsids.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/ghlxjnfmk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gajadfpue.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/grdbenajy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/ghwnfgysi.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gdlroahin.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gczsijqjm.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gmuqpsjkv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/guiovhtli.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gjkrsdlkd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gnozueokz.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gsxmsqphk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gqmtjeuxu.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gxrqnrmls.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gcsxcbqgg.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gxnigfzcc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gwyobzgkb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gitcmgzsa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gktpnsdav.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gaixcxmrf.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gvkcwlkeb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gxkpwzydw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gwuqtdmvr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/giapmstto.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gkbaqqhiy.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gxelfymbj.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gjeiyumvm.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gjolzrisr.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfqywxfpc.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gxhubajdb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gcsfpjmbq.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gptztbcgd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gwdnakphd.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdrhffdtc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gplsjcjlb.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gfoelgzic.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxtohsoyz.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdeaneb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gpvwmlind.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gxykmrvne.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gjjlemuoo.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gcuolbndz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gtrgmroww.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gmfdevphe.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcmblhpbx.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/glkploflo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/ggfugrics.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gufkeospk.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gdmkqrtta.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gbpxhbqbq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnwvpopyo.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/glkawiiul.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gumhfqgne.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gpputfqyk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzkseibpd.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gnnjltjqr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gspvqhrsn.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gtoxsrndm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gkpweavry.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gawlaqwtw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbkiziw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gxzhcbcin.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/guwbsiaku.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gcpngbczd.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gfuzvopsc.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gisgakoxr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gubrvaitx.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gbfffyvcb.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gknaciksu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gqpepgpez.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gsccixxzr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/geulxbobs.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/giopraizy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/goagozmlo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gjsennjmr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gajuoynvz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbvgzdx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gtgmjdagn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwlzqisem.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbpajqld.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gabqvejal.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gwqbxhkak.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gnvsjmosy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gvvdwrkmy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzksesjab.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/ghtqdyrjv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwrkarnjj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/grefeebea.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/ggtbtfayw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gaicqxaid.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gjezcgvaa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gsqdyuotl.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/grgfeaoji.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gtqwsimwg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/glcprlhdc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gtxezzsae.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gabfrksnd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gzyckuttb.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gbovizlyl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gkwcxctyo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gqzcmngtb.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gofotwszq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/glwmvdpzf.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gakjvfjvn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gkbsmoksw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/guiwuxbeu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/godduoeyn.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gwociedsm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gbjgjzyol.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gcueolsxw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gzxgeltfn.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gmwfcwpur.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gxjxomygd.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gxmxgzump.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gmglexfot.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gdmzseknl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gripfifsi.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gryzasmuc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gjuhrqqsi.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gunlxmjnp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gifnzhlnb.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gkdbdhong.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqvhbudkx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gqszkowvj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gunvkzsgd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghwybsqxg.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gqqbnzbdm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gextqqogz.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gasylapwa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ggisqspkt.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/ginikazws.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gablfdwde.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gkoygxhwp.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gkplkknti.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gqmwyuauy.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gfmmlwkuy.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gjwfwnlix.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gnuezgxop.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gthxvnvdd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/glwrlognx.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/geyvtwczd.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gpbmjkutz.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gmcchzrag.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gwkkzuykl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/ggnqhvbpk.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/ghwhrdvrd.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gxmaidkrq.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gsjmofzim.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gfrubhxme.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gfyedpwcv.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gyyhbewfz.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/grrrhzazx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/genudywpe.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/goapkfpvf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gvgelvsuq.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbhdvvpwi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gopppzvke.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gpucecokc.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/goplntsnx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gouxtnfmd.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/givdbnmqg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/grqcfjpoo.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gmymeyfrq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gofvixbek.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/grldxbvio.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/ggnaprnvm.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gbnypybit.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glwjkfwbu.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/ghleqhfxs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gmgrxwiim.sHtML


<!-- 参考信息 -->