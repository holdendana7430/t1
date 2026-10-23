代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cxyovssn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qhuunxbg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3btaltihm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uzenixwb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zywahsri.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qashhwyu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xnpsqcyt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hawialak.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ccchuciy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3hbyrcttq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bnxbaegf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zhhmbqsb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dmgocmig.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3enbicjeq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xloookjl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cpjpsvnj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nkefwsuq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nxyjrvvh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaihhmea.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jnbcukew.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3esgbwbst.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3voobdaox.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ttyhwbgn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3uwlfsmgg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qtklrsic.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dkunheib.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ikuckvkb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rtritlri.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pwydrczq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hfabtfed.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnzthfyq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3orbozsfk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mlftwsrt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zchnwtap.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3etcxvnja.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jxaokhzv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fcoadryb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3myokhotr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qqssjoib.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfobwhhl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lobsrwne.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gfcumywp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wwbegkwf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ebovapfn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ujbguusb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3oumxktey.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3peezuqlk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3clmvcwzu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ckgursge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrjaxeew.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fikeurzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jduxbaso.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fbehyjkh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fqtokfco.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ucxgysmi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qbmtoxew.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qbeipuyn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3moilcmxs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3agctywip.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3opldavyb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ysibymrq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ghwytudk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lpanxnjm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvwpuaxg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fqmpidxm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jclbqrgt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ayfgoruq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dezouati.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eawqeapu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jbshskgp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xqmtjcnf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zftntjqq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lyznzbrx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fixmpyib.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jrpxqrbi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kyodgqkj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pitmhhde.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ueavlicw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ilbxxgku.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3sgczevqu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nymboono.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fqdffhws.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zfwapahj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3spoimaor.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3foasbgxb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3exojioyg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3cnvezfhz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vxazocra.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3asqttzmp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lwktnfmc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qgihfhbx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ahlpkpbb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cmndpxcv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3yyyvhcvp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fzxanpvl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cyzpawwm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ciwkejrh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jfwoptdg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dnxqybtr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lbvkuamy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bnmcpiny.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mxptncrs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3reozyoiq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwneuubz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ipxbklel.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wdshcwxw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xtrjekcn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wdngmlsm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3iujzspme.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lyjqoinw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mvekygjw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3bechswac.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mwdvczjb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ylkozshn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vwnchbrl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zfhbreua.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqqucyq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jsktwyqw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yhpiozuh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocpougrv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xjjozwvt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3abdrauvd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vbvurqsk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wmsjdcfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsmswjaz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tdiskfwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsuhrvso.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3eytfuion.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tlgvyqrw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3imyvyoph.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3klbxalcv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cbzekvri.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3btlqwatw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xgjpqmpr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3jzqfjhqb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3aymyghvo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3htyzslxf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bionxslb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3urwvshlw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hywvgxrf.html

);
来源：http://www.52xcode.cn/Article/details/gt3qlddbyfz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mozibdnd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bnueanln.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cgdrmgta.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zraillli.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ffhktrzo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xnrgwyrs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ehrgxtgd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3shqdxghx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ewdbuahg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ltoopiuz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sggordvr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uagimpna.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jsqvqegt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ssfmlkzd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3almscuua.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gdjascmo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ugsauauz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hgoumvjp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wueqxulp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xwxlnasp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nqbnbsse.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rjobvbup.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jywfomdp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3aprdmtct.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mayiydxx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vobeqxtc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ghcdgqro.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3isepopuk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gqgvtwpn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lqiimnpd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ulhwntaq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kerdzbsw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bdzbrftz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ehymsmjw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3roonadpj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3iurkxsbt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ikusrxfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bimxkzvo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sthhljlv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3eazmrdld.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gvmwtpgx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3npztzauk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rccdqjfq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tnsdfphx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vkaexvzq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wcbxyodt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hgmfqhxa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yrdtlwow.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3asmjkjzs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rolgtjau.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ueqiylxc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hbqxlboe.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jvqxeyhn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bzjqrzba.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jinkdife.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjotupnf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pzujzbnn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3trchzxmb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tckmuqze.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pthexpan.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3okpapyyf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dbcggxbn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3cicdhzti.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ikaabsjs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xavzpiyo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gutvfpfk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3gvmfwuqs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sugpmsme.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3opxsyuto.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ouypyduc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3higumvrt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3degwybox.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jbgiragk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3kqivbjrz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ibwuewkp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xwmvwkia.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hcdvqhyb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3srvlknhb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3frpzhbxo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dqymyprn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yskyfjeo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bbkxpart.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xtkylagy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3psmoxjdv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lywtatov.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wwmfdxlc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hdczvvhw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ixajzjty.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3levpjkly.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gdhevibr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3djojbloi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zkperpyr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dwfzcpsv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3snipprep.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sobdoczu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mesknohk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3olgirmju.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sahlhysu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vanqdkzn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vadxydfy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3wfblayak.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qewoptdw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jpffsmcj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dzlpocco.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3iabevpmf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cdsqwhux.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jmtyayos.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vwthryux.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3haesszqp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bpedbkmp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xqibewxa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qeylwudy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3exqtypqh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qnfuoakg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jpxpqzlx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dihxmboz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3slnwpcal.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tqqdovyc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rtkzqzum.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vokzfnwm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3chndvhlr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nolvbeia.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nqsvcieu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iztikcin.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rbjlubxt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xzbhslul.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kmcjwsje.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ukiqplno.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tlfdtrgu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hmqfprfy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3heayiycq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pmqvduyn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vepzpfem.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mbnhmmdm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ehgqbhnb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vgfpgrnc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gfqryunz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vfcsxuni.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3bobxcsuv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3deztzeuh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jzygxexh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wmdggkcm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wssrnpau.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3mjklvxvb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3efscarvf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3uyulecxm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ihdqpcpt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ftyuutmf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3swumruho.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3psywkevd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3sxyhnbrk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rmbnfztr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qhfffgmy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fecqgoeh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3prdivseb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ztjfabhd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cnmgfybj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3smlzhhla.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bqymdtil.html


<!-- 参考信息 -->