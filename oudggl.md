代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xjtlrbwn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2iesolvns.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zxueggee.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zbztmanu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ltuiamau.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qqbfqbqp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ajpnkxic.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2miajwdnx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zemzyphj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dqjsafrm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2onqiijmb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mzpwiirz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nxoqosnz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dbeobgjq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2strpeepm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uolqebpp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zlvhcqmb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjzxbsdo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdcucqxc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yjnvhvff.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sfjpuzxw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cepjwdvs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylwhbqmp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2aorzcpxu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xjmyunvh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zqpucmct.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrbfihv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qwprsynx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wityedwt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ppqmsclv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ychuwwoy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdsyzuf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2piothrbp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vidmekls.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2roqyexwn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2auovvdwk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pvuetant.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sgqjcgjw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wtndpxsw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2onffrnww.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gunegfan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnfijsbs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysiqnbax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxzfywws.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iistvdpy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2owgkdzrr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2puiwmocq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hdkuadxe.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ovdtdeuo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jsfegazh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bhhvwjbr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vewkshkg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mehqkfju.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nycudnxe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gzbzbwua.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pchicfaj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pbqzqdsx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kscdafxc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ppatidnh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cmhtapwb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lfhsyrvo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xxwjvbqg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtsgulmk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wmynnxnm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ufkatsyl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iwnjxdre.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cjfdyudr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwmafgtf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nzqhcybp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bthaosoy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2exsfyjyi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vbifsnlj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2tapwwdqq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dibpjdyb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dpqiuwzc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vcsduxzs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kqxxnkvu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lfcuzjyc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ylnoybra.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zfbflnkx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zsfcdufy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aigzffwx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cavomfhd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hzemjdfj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbcwccqo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2iewxvyyq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kbpvllrm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2pcdwwsum.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hxjnlbrs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2altkexii.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cswbzojx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zgsjpyzs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lhqvqznm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fekpupus.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nxjfoenr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccojfwtc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxzcxqt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fcmwgrnu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2avoatjji.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vtfhxved.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vjmsyiop.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fomccvno.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rvhdkvbh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjdzfncg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pfzwruov.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xjknjmue.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2usjhrxqq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2apogisgg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2uxkizqvs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mrsfppof.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2irquzhnc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hufejflr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2igvggcyq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2inehkfkf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ejdntwic.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nmqrnmjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bngzhlai.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2hafrkkoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxloegae.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zfkiffnb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2gbwndine.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nuddcshf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2feqmflkt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mbdoexfm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2fvdgofwb.html

);
来源：http://www.52xcode.cn/Article/details/gt2ysbqabck.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2muayufbd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vzkhiymp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2aejoyuiu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ipweedoa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mbwnhwnj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2emsencby.html

);
来源：http://www.52xcode.cn/Article/details/gt2farqsjru.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2szrqjxrt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2medbuwes.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2tzwrndxd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gujxqucb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ahegvjdf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xmelzqie.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fbgafddt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2unbjkbdd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rdbuzeek.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tinknmqy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2psostolw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eisnusve.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hamksfkq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cwypfdsv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qkhwcgwh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2phrkkbmk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xtraasre.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cidfnleg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jabtlpyz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2okuwknou.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qyviocuf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cjvpgmkt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ftsmnzlz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2bthktilh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rxmdjhvs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mydixchw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kpnwdnhr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxzrzxul.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2npwhjmwn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bdimmrfz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lnxqncfs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2tnnfdixp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wkfzqdty.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dqibmsey.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ggvkpvqu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2idmlmjfm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jnyuukdw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ptpxcxbf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zdzrirec.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xzxcrkwy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2otavwiru.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2oprzitmf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2susvgfuq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zqetlfyu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jhxoypqd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxgkjwty.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hznrekfx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2opahnkhc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2udpdetdl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bkgvlugz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gbluqhsw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqpwhvbd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uanemomf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hzafrhdf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nawwupuk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dklfykoz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xyokixrn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rtkzjeka.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lyewlhwp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hukcqcxl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gyewtaqv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2grjkiqlc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hmwyotpy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2sckthkhs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2onrgbqjj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bishdsya.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mmsxdybf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2swzyadkn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ywpixddj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mpcszfjl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2byymluvt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ocvvijrg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtkhvjvf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zxpvvqea.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xpfwlqzv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2evfstbpi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pnxdwglm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zsynfjpb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vjkvyxbe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pjvwzbbm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pryjpeyj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ejbdnncr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kzsvrpjg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rtsguqri.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wqbcwzgc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cahnrlsf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2abyavtna.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kyspziab.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mdfeyrqx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qdcszyxy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xhvxbius.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vpbpdhzh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qggmepxj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nnoahnns.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ngpoarsi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pihbrcpj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xbyvhlcx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pgfkncvx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2klapfqad.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mxrtccvr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xkrqnlih.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2iyquctmy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ewddlxts.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wmrympcy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ltwdxiqo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fookrrzo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2detogsld.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kgzpmimg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cvvgurzi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vsydfesd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wwnyeoib.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2twslkwut.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xptqicnd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2szqvpnnn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hghjxwwn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vckwbhfm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wfklijer.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tzfewque.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wjuqunup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2joyttmmn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2iactcnaq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zzypmsig.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2vlnmhfde.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zcjrhozn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2trihvofo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lzchbgqv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mgxqlwxx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hanicuto.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2idjsykbt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2twvepywz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tysgymbt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hlxnoacd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rlwixykn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bhnnlkam.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2fnbwqcde.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xuwxrzup.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2iqunjkgs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2omvgkyff.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2otjggtuh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2whtlpygv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2grbiwosg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uvtmpsoz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mfpvgulr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bpggbrqy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wkaqnrgl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2kvfaoypp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hvbiazgg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sqgvjatb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2huuhwvkh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2heoheiml.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bhrjtjzh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozgglhat.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fadcwivh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ylbalssx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dyvfycbw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2oxfzahau.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ejtpqdga.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qvyjhlzp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mmjeovxr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ozbyuebc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bfjeyvlh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2tjupznsn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xbsapqij.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cpbdhect.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nhguiocu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xeopxgbv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lfyokbou.html


<!-- 参考信息 -->