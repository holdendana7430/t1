代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bytdenjs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jhzkdiwt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wjismtir.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cghfkigg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2drjgshxx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hmpgmidp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rotydvmx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xweudmcu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lxrztgas.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ddbmfchu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilflhcfm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ysffkaie.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2iwvmeatx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aakoqbah.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pwzdggro.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rbgafrmv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tnmacatw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axpgdmmo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bvauetlq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qnzpuhem.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wjqrbuzc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mlzqfysi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxailfzx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qblsuazb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xehuwgjp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2acbbadrq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gicxnrcz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sljlwiaq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vmhozyjh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wlmxysde.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqxgfud.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfcsjhg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mbtbghyc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kxkrwfda.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hcpbkwrp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hrnzyfcp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ptbumuki.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2exdnqzxj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zxzusuak.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mqbshwhd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2sowanjkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhovrycv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjdxmtwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbczjloq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2infowowe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nihvfvvf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2prqlhoyq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ltxrfbad.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wkkceekh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sjvdaldj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qcowksjf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vextjzga.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hjdxmxyy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bnepbffb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vwhenjpc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gvfifyik.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gucrysio.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tclspcpy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nsoymgpy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zmafbhqj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ftpqrhiu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2omxgevch.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bcqykuta.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2oshwvnge.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dwpwdpfz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2twjsyona.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2flsgfcjk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pfimiomr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yglsjnsp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2snnljrrb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ekiebpda.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tjosjuxw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2riafqzgb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yzcbkmms.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lvoglfba.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2psloxrcr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oeiiqhuo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfvutqy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nrqjlafm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qmuoyzwy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2knlhslcc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uyceullf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2raroqpyn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2nyuymrji.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmrqvzju.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2duwfnkqm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ciikjvhs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2honytftx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2goladdfd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2boyrgght.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ikghqawr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2seofkqzp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2chnbeegu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2tlepxnjp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljsusrdm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2shgbmrnr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dporqgff.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iidhjtqb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hiebypda.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kjersgiz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fxaueglf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jpfwkmxj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cfoxlmgz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atipnbll.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jgskwysr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ndrqxavk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qcycgwnf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2pdyktdxt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ppmcroej.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tqihesom.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2jkcctbuq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttduoeur.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2apspvgpq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tticcqko.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rpibkgoj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ozgmgrhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2comkduwh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lczdhuom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqvxrrat.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fojgxfdt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xsqeeibl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2myepyxec.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zcltgpce.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hztifcyx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2syldlcpg.html

);
来源：http://www.52xcode.cn/Article/details/gt2kxojrehy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vbevgapx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rjnaomqf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2upbgxihr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lrydeysr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cklpgyix.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mlwyudpy.html

);
来源：http://www.52xcode.cn/Article/details/gt2lacafcny.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2shasmkmt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kmmlyygw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2eydwopdn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zayydemb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2keepztia.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vbgmhsua.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mvhkxemf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nmfibzqk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hztvekzv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2banfeqog.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2enqledon.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yswscjct.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2dzkdbypl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ttftmfya.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2eylhvfqf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wsbqbhmc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fbcrfmrc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aqkubdlh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ogvhcvkx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2upmyxhyi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ofbjmlfm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jytzkalc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yqehumgm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ysgkupxv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xijgtdep.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2txwcbnpq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wvcicgep.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltracuhy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bevkamiy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdzshkyf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lzmrwzxn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cuaboexy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qgawyqte.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2uahfrzjg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bfgpdkhr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sbcrngnr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mfjhpcje.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2amisnswa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2svlsebqa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zlcssixq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2idwjskbo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dgztnflk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2circjlfa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fyywxvyg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vxomdhly.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wkbainox.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hjanqvih.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hjhrbsrt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rymhpzbo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntexdudl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zesbqcmk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2daugkslv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2csnyervc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lgenkmsr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bcdqfpki.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swgadsta.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ageixmjj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bxmjmkud.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uwpbehba.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dhbrwuyv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lrcuvcrj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2niiuwjcc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ravuxged.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jhlgbect.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rlxixpnx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2bwozdmup.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gbwxkiqy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sidhllcx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdabglui.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pcqdrnqe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lmvqhwsx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xflbihvn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oeusloxi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rrvigvvt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hehgkggv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rhiikohd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fmgkftju.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dzghhyjb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hydrxcjo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vmtnapgb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vbzwfoxu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vhrpzcgs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zdejzyii.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vtjtidnj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lvjqbzfi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2czlafhnl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vnaypctf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2opahuwwt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rsbkszus.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zdllsflh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nmrwvbyo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xljdlmgl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bkjkwovd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jkvqugjd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ovzbswuv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nvqnhruc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bajkgdia.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vaskbecx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zehropvk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xbixgmpm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vujgwcbt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2znossbjv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bwykwmyo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tcdohewy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2lhhptqmd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zgolhuas.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vadajxcj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bqebsqsd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wbzevxkt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ybmdlnhy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ewvblpzw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zxenfgmu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qvmawnlq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mlvabaae.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zticwsfz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2srjofpuz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pktvrvbm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xppknrgc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hzjmfpta.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmrafmmu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dvsqxenp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rgducade.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2sitegaqa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vvmkwigy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqizmp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ffieeqlg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lwnczqot.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ojgwevbh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uabiopwz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zzgycsjj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ysudzodo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sfolvtsl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kcixuklj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wjpkhgzk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yoxilerq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2objnomcx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zsikumfu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dawekmfi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rderwsmd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vtkdalsr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2dhpeyowl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lnfatgfd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2twqvgfxg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2biivttgh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hjpklrie.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yjyhpgxa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tcakacxs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2eompffaw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wyhnyjkt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eqzsnhtn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pozorrlc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekuyyefc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rptywuep.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tyeitjpj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2yxiedlfd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2amjqamyp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qzfzqmvs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fojekxvw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kgkefpow.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2onpjpblf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pixqqcwk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2pgjvzxtv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gniusncb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2apvwapjl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ihshddzh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kexmpbvc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mevijfiu.html


<!-- 参考信息 -->