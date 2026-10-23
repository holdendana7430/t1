代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rvncoyqd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lunkkitg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffqdmobv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pswzedjv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3anyiuqxg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwmdrnlv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3sbwcaykl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nrhcwkqc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3scmoayho.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvynkavk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjmxbsyc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qhfywigd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3szraemoa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3tioqcdap.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfwdtxjs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ekmqofgv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oomxjjyo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xkoirhfk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wjumsvkb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zguevcmz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vvsmzcmx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3eqmusegg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ryfrgajv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lpzwkvqs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3uzvobuqd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ogvyzexr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ndenodel.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ynfisvzo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vraxveqo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mixvezfw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ldwmgpki.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nprhbotk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cyeewwox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbxrpbwv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcnrfdko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exdeeidg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hemsufbf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3diklzmlg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pjpnjlrx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jrcqljwp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bhxkcljr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pxwwbmhn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zscxdsrb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kvyngdam.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3emppmhwm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3iufcqwox.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pjwovuef.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qukkyhvo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gmhijpkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3idiwqkym.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xamukdff.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zpdlcewb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejkfmxtu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zewyvmqr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zunwlpjm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3haycjqpu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3scruqjxj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xlsixvmo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kfakhcis.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tyjgykcy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3gkytpdld.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bsykdecw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3msevupjr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lthyyodp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wdtzmutv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vlszqxxj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sirueqlr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rjqlganf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rqegmbmp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwygovw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fpqotqhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3peseeiqq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ycyguahk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sjvvqqvq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vinfiezq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oifwlclv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpykqek.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3uoeegsfk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3btdznrrv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bkwmrquz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3tgmabczg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xgdndkre.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dkfpirfn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tvmtmelx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3botxkfar.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3oqwvukoy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkxjnksc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xsvucrio.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kphnmiuc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjrtsqja.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jirclldv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rcsvdenx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kbqftbzu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xshueytw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fiqgsomo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdfwxfes.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lxzokiyp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cxxkbinl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qkgqmwwc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xhsjvttq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3meyanego.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zusmwool.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vcjjwjda.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bmwbrxnv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rlyjvbil.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qivscllq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gfbhilvn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xewpchmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnabisgb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3sgidkuwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbxlqtuh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mnbumdhm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3uidsjdyc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ocovrmvl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qkzkmyxx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ckrqitax.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zayrkkxp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jdcdwpov.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fgqnrkue.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lyotnbet.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ydrvyelg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ahkjwfpx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qvoeeegt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kkwkaats.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kthwkjom.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3guejcrqs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3qdinuqhv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3twkpwajy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cytlrxjy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dscdhsfi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zfcxhnrm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bmswanlo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ozzngqiz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3uijjeulk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lmsjymux.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mepxukpd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xkzsvocl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3oznqjcrd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hdegjxmz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xkyhmloc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mpvepybi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xomkbvvn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ruibmrgi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tkcmfhxt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zcgofhmg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3injoltav.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uohzktpw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kbixijaf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ysbgzysi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bwfedzra.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3odrtdvif.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jtechhtd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ytopnruu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vxcdrbiz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ogxseyvc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3orqdndzj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tjtnytsh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sngsubru.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kqlyvxbo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ujgjeyyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mdjkkrmw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tausmgpa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3adgkaric.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ddnkujbq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fzwykkbi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3heytxtpt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qnyxjgeo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bbtllzrh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hywsmcug.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qjacnuag.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpekdkau.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cfnptpuw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3frjwgjwz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dprwkmxh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tkjfyxhb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jxfrdaza.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmdfmxrt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rwymbeyw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xtneneak.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qlwtyyuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yvfznbcz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tjhifhzy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3crkkiucd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eeljdbcs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3raolclqw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3taqvwipf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uvzqdilo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lfflirll.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wesqbphp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3umwjqfpu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gmcdslue.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qvdzplwh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jedwqmyy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qbvaptyb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cgqiefzy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ymrgbaav.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cignwylx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hoamyyib.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3eygizein.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3kbbjeint.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kepvtwhr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uqzsfkyp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gejdowaj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uovslafo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cayioyoi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3thqnyoai.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3iuqikyuq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3poipufxy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3epuphkbx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hpriwflp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jqkfdrwl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fyodrjbq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3upuzqufs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lazekqdy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uvfjjcwb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3znyoxyle.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xvydblyx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wchvvsgw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lpficeyt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cvuhfosv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zuhrvgop.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3orclkhmx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3urpcoxqu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3txoloseq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wktnqngu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3letcpgzf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gwviyzgk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ikzwmzkp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vxxhmdoq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jxztxmtq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nejnalsn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yuxryosz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdjpppjg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mqlnnskh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aotkheuo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mypltxfj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3annahsaz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ckxbimwv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fzlhgixd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rncfisfm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ufdnogpf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3szokwjov.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dvyhundg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vghetost.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tfjxjnee.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eirnokrf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iourbfrb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3bbotenpk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iumjgssx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ltnysseo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3sxecnjyy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3frvtxmnh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ypghjcxa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nfnpuotg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bfcxempm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3thhnmbug.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3onasrkzu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3plnkieyu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dbrxtimh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bbyrqwpl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3extprsla.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3oagybgqm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ojzczsnp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3obyzddfj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3apkakrtw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jseuzbrl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gyvozhxk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bfyyyzlz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3btxprvex.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fupqfcni.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3inxrumfr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rszqyysi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3maxfpbnb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vgesrjth.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3evwrsxqj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3euiobdxa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ouotgbxx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3zdpsilzh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wpnynpdf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qznddarm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cqykmoit.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3elxsihhv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wgmsfvxl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3emlsglsj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3asgwrttb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3unqivxcv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nstkmuet.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pwiybsgb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qovqwohh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bckngnsh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uwthdkil.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3icaiotot.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rnlzlqow.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jeqebffe.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vpenkqlj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qvdbbcbj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ffebtgwy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jeyvafgf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wwzlctlh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hqagtttv.html


<!-- 参考信息 -->