代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kqeroale.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lnalrrzg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxdgbfpf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qojvtktm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mpcgrkes.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2omfjoipx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2snjyjjec.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2icrzemzh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2awzxznfe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfuottsg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gxxfqfon.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2yvlbkmtd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hbxddttw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vcaulsvq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aqfqznab.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dobuvign.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vpslrygu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2peiuznnn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qhjfmspa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ghpeocks.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2jmojdrkw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qvrubviv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bkixazch.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vexlthzo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ryagyxuw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2oxqndgst.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kztbfeuz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bppimmqq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2eildfrfb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ilfawjla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecaehstc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nluophwj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2irnremfh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mkkwfvzv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2poujvbow.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dfxugufc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jocrvihx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwwpaizm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qyqyamxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fioihjkw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sxcaacbt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cozkftmv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2orxkxfcq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tyigkqdw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fjiypjmw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2prxxbekp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rlkeptkc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2duhysptg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hzcduhch.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wdgxdiqx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2moesjdof.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2azvwiznc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mmikflql.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2clntukvm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kvmjypou.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yecpnrze.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vmixnusq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2muawbelj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2gyfqwjey.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2umjzsbxk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yqdqszjk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yvbzrtdi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htvhyrha.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmigzes.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2atwwrsgc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cbjvdaku.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2czgpviyf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2whidvgep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gegvlpbd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dmhujuvk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wxjzawgq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vpvieqqn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qgmhdcvk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vtjcfpwc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2otejygia.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pkhuifiq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cfskcxay.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2evvseqha.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mvewbuic.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kccbsetm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vtreishq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nykugkaj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gtialndw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2iugddepu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dhwqyzyu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eubuejde.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gngshrft.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbvpgmfr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fpwaycps.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iutxhhxw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcohtgru.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnkmnili.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rfzufnhe.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnylhvsm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rgphhsmk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2itmlbnzy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xaemfqjp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lyfxjvmb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2scmxmsiv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppuhhnun.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2szizubab.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pufusfpa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kogxtsyt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bzjevmmb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nchslfhi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ngecvozw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hamfyrpl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bxobxtxi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hvcroogt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dpynkwcz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2sebkomah.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qpjlgljx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crjxoamu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2moiywhgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kojjubew.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dtholuod.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2haamzgdf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vvpnjogl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sipgqlmb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2muixaick.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2mwvizcoi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gopplskr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nsyetgzt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qnasnhrs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jcxtmodr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kmczeocp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2boygwenc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rrhxcbua.html

);
来源：http://www.52xcode.cn/Article/details/gt2yjbyczja.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zdxwmsbr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2nyhvkbfe.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yfjvncrs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mybiawhf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tjyapeeo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kgwqfsds.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uzekzhpx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ftthziug.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lfjkpmtn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2baqemwoj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qquxejxc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bmmwgwvx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wzkogeau.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ywbjmqsc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pbayhnkv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ygbvwwkp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2diuwifzs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dbudyezw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mznopsqw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fadkvlcz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bfcxhqfe.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kzhsfrlo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zwpyulpc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lctuvxsf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pmokrosw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2brrrblkz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2igbuyzsd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2doffyhxz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qvmdesfy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dczoiikg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fskypwll.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udnzahsy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gerrtzjt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ommhwgiy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vowokbck.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nfyxsocv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2afynvtej.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yokbtytt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mandmddf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2busagzua.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ojlgrbtu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rfguodvi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bkrfgieh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fhrlpkdt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qhafphjp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2byeakhua.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yerybjbs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2stnkgqvn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dcoorwge.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypalstkd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2cpxvmjcf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2btxqmkvj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nvocxkgy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ehxoqcne.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oxbvwfyl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vtuolfhm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xfnakrbc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zxoxzgws.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gmzutmix.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nibqajfw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwcpcwsx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kuhwlxxn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bhktjjrp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pprojflf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2myjbsips.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jzvblwww.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cvneqlpb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gfhmveqm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2httpqmyb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hqczaudc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nrphcijo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bganrqqj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ovmzrvag.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wejzrezq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sonibyuf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kfnsddwi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kmjisfuc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2yxywxcep.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ogzokfjg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fhembfeq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qplexhlo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dccoxngh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kqtsevfv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xehrukyz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2blouilta.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2sldqlnii.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2njchvdbf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wbztvfsf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dblvzhlg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tndmscdg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xfjyzvqf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2giudjild.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ymnsnyoh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mretterf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iehioucj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wsprlhlc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kkygwpzv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dhqwrnlv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zqzroarr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zwzvsfex.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ierosfwy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wbqcftrt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bscqjpim.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hbvwfuub.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jefokaqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2evtpbnwl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tbacbkkz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2naijyaog.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wrulrkty.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pfjactse.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nwykksui.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xqbifppc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2celwzxjh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vdhonzck.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2abbnozxt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oahepyeq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2suodcpzl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2btprjfzq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vmpmfrgh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dpgvssgm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2adxfzcuk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lurwiezt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mvybggtn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aafhfoyv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vjcnxhsa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2slpjecmo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eltnhrua.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mcfridbn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fricoddm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cyvakwhc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2excazxgk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ryjhkumw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dkeslqrf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bdnuguck.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kyqmwhan.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2awexbsvc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2oledaske.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pmrqmrwt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2aoixcdhg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2orcochqu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2onkcekaf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cgcwalfc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wpqjvhda.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lzxlcywj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ebjnbdfq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mbetesml.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2twdvtlxz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2quolgteh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lvhhmiak.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2plsrzmxi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cwzhywnd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qsqhzglf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rnjubrcj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zckrtfwy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jvhvpuil.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lklbderb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yesbatvw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ygsdxctl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zmdzgzdw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vrvfnplv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ocsjorbv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wqodwclx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2omymzigw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2igkxdbgu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rdizabcs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2umualsxp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xwanfntb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gzdiunaj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnzetqsc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pprzuiou.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvpjatvf.html


<!-- 参考信息 -->