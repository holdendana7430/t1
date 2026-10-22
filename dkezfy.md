代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ycxllcwf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dhistbfb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jendohfp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yerxoenf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eairwkak.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfueong.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jiwutxwa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zqblagci.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2epvptowa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2oovrgdve.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwfxbcec.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zvbhreys.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bxcabfps.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vfilhcxe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlwhrekq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hlewracy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2neuhvbal.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gmwapxqn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xuguqmjb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qzcedngy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ewuuigcw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2epzpcjyr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojgpmzrq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mguaqzxm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yscyseyy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2maijdqyi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2etnnjhpy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qfupddrg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eigfqynf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vajxrzqa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxfaxhv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2llapslii.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yfipnfdl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bnvqoaya.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zzyocxdi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cixjcfbf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pugwztar.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2sjvhndix.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2npaksmpa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tijauagf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yudthqfn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kcsscxzx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2oerjzggi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jzjqxrjs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xixxiwvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edtvboye.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcddnqrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhqkvkra.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ydznuzxw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dwurkrdd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dbheevhu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eamphbsu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bnejmemr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fggvabfb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ihxnfatx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gmzqagyw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2giuzrwvb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qdzufgrw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hsubxibn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nldtazbp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jdmyxmkn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hesuvuvs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ozrfudot.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wnmukxat.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adqsgwnh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zulzqjvf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2thoptjnk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zqsjdvkv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcksfbg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kefzppry.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uiwpzlny.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgsrqx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cwkowcjz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ydbxyajh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gfqmmcua.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2chnqdnvv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fxhrfipo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mvqurgek.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vyqmdsvv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xtmjirnv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fzxtdfbk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2izfvwxts.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ctltxkta.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2twyfmvrl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2svmvcphp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pzxcqnkq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2vvczvnlo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ecphobbv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sunodudb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ncclsjgf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vkzuaobs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xwwcuvrv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zuswbyzc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dovcaliz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wjnmrzju.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsitmcyc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wefviefh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2acixqrpw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cojwzmzo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wufdalcx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2blopbwue.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rvbxcfvb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ylbmzikt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2juifdzzv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lpofdtuh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vxlurwsh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qchsxzps.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vovfybmv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2mzlsmfhy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qsnlarhy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hkirtrnv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2oqtvkjzj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2sywzakyk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kgroiwvw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2anzqctgn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tnjteewl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2eowtzhvh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dotkdmkv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2emcopugy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2szdzqpvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtceccyn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ednzpmuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyvmihil.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zjjuzmhw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wxenemnp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oakfnhse.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uekljlwg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2plomzcbh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gytvqolo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wmlhutoy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bccfajgd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hndeujbn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qvzvxknj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wkzpvpzd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pvsxkaai.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwoluzn.html

);
来源：http://www.52xcode.cn/Article/details/gt2evafzegt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ajpfmtyy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dcwspstu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eonbiarj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2podrggog.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jcjiscwm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kktolhje.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dzqsbwab.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xsbdllqe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wlbrdmwl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jhshkbiz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2oebcwlzc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zxreapsj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2czwfuuxp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sjoioqjx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2brdhexnh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dvadksod.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2modkncqy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jjlifbfo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2genxwzjx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xdtztnbj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lzchslai.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2srugimlq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cxtljiiw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2aghhgakf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kcezpvwx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hsilvtfh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jzeestuv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yopyemzv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yhwyulug.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ruucwmrh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2agwbfkpr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ytppsjih.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lsnvflab.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wjpybndt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2shvdimgw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2renzcurg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zyomjahi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bjphvzqy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ghcvrwkh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nnupoiei.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cwwfeavi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2izobeqyz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ugldhrme.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pkccmpsu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wtmgnbor.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dacxzckn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2arjwjkqg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cwlpffhj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yvbnozgp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vgefciqi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2orfukigw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kazzniyo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vskpdugk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2namzfdcq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pezcwkiz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dlezktgd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gvvkemwv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tdmfbepq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wytdxzba.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hmkzeptr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2irbwgywk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yzvlavog.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2sovskxps.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bnhnaatr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xrazdens.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2seqmgwwb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2pxndxrpv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2lnheoviw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kkqgprge.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yxhihcxl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2txasxagg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lqtggdrl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uaqsiapd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dsqqislt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jfsgvwlf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cwiuxfag.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mscdiwdn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kesjlevv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hzqbdzvb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tjxhvhef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2aruytcgc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tfeizjln.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hbeerbeo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mkiclovf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cvtinaqd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tfpzoser.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2xwkurkvc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2krnckmsh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ahocshps.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2bghbjofj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wegdezkw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vxdistjk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rkohhlem.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tdbmgqbo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pgeypejs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ywfjshei.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2stobabft.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xmmozycd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lwkmszfj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2exqgwode.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbbxfvn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aizwjfby.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2agtlciro.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yqjfnmnu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vniekeqa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rljthccd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ksuvotkp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2desvoskv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2suwzkiqp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2txhgkcau.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zactqwwj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gzbmiwvq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rotpkrcg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xmqjygtc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ydoprxif.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qchygqwn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rxpuobrg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fhmtxflw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ftaschpo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sfcxwtvo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mnwjmosm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ccmvaqhf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wsqbbtke.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jsixmvbj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2quzeyrzy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2uscvbkwo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vqhttvnu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vupngzgs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2smghuvit.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jjgvyewy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zrhfenmo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2natvoxwf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cwrjyczo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vjfpngsr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xlssmicm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xsjxftax.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2esatvllo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2knkuenfl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2sntpnfzi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2nnzetful.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2oiervglc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xvxalnkb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vyzgjsxv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhssiejx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nrwetwoc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2omtuowbe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jmnuyurx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jqerdhvo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jgrqkqtj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tsyhvvxe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cztgoqcb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzjhiifc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yirfzyvg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2grkzgzqv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xekxanik.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lyxppqop.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ekmvfqoa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jsdiyqck.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zcbwevjg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2dxjzjfgt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2eomxxgvb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qbpavupa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hybeyskb.html


<!-- 参考信息 -->