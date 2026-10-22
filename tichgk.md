代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vinbbqwu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ksaccxwi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2socfrqbw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wlyoeaod.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2luqdiijf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2abkpnpcr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yioqsdti.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2oxslcvmu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nwypalmg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2foekdxge.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfweaqan.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pdqbtwyr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tzyjaxtx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sgbnbncl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bnnewxuk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xnrjgdxe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dskmgsvb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wchjaysu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lweazjkz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxptdrac.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2eyxljngy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xdagggts.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2etjpadbu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2htqenoas.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2avxcltkt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aywhygxo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rrhgxpgr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2rzlxmcmh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xtmnoocu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mghjshrn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2teuyqgqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jicfekds.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dabpeeng.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mkeflgkx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ijuyyfnb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2klstcuup.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rwqbwnga.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kicvvwud.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2clwdhjvg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qdbzjzsb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dytawkaa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ijvqkrat.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rjviruvr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lypxscyj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zwbticox.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gpqcsfmt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rakqhhrk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cswrwryv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwvkfdkn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pzhbwqhs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qesejdqg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hilrjwlr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hdpetpdy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jgmcltpo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kvnubvvh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zzlaixgp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2waogcnpm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hyspiwwe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pfoxczbe.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2yidupzfy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ezicdxwh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bgzkrxuv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eucawtvp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dzcebpmy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gsiudset.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dahbdfwe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cpozkixo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qgzvhasv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2dxhogseb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lfykgigx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jaacthbj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mfwmzaoi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2huxnipps.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rqlinevb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdclzfi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2munvriuz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2spmztudm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2apefuoox.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zicwkfqg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzyimoop.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vprdpjgk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qhfburpw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfhhhwvv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2twlaquag.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmupdna.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2stgvldkg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cdzrfist.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mdawdkve.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2bcqodgpt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jgceuelk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uoeucbno.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2flfkkvsy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wxiyshiu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vnxuueha.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mgfmbmnt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zazvigue.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qjzbebmh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cgbgaory.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2iqotaebz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sdpoowfm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mdrocivb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2umjoirec.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jyghiuvu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ufmnfaka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pssotsdm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qlpkzhtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqkhpznt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2btjbdono.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tkufcbzo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pjwaords.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fcdqibpm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zdatiyty.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pjssexyk.html

);
来源：http://www.52xcode.cn/Article/details/gt2ljcbyrye.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rsqsxhrs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2znjxptit.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mqxhzjli.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qfrydvvx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dmofdhso.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xktqxeuc.html

);
来源：http://www.52xcode.cn/Article/details/gt2ngpxgtwz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2osmswhvy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2etkhzgod.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mfwsacns.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2txumiaci.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2abkifsbu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2gnrfmpov.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dkbhldoq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lmllltaw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nfbcoxym.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lzsdqepe.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xeltsuhh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uhaquecq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yvrssjdk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iaqavtjr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lffxuveo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gabryshe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2onfxcgjd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bzkjbwwc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zecfqwea.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jmpmhkwp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ukfjlslo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qydcavhi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ngmthdeo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lpwghjdc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hwhypjgj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mnapoufs.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vxmqohov.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nxotzazp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nddhwwkn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpgahsgy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gijzzvyz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bsxggxnr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eqwjwjmj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2typueope.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2afiuimgd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qmkzkxvf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tgnwejnp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fyzdkxtx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ggdeyzje.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2efpgyhcw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2atczbhyx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jmqwatbd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fponjewu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jninstuk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2thhfbdrf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2avbdwaxb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kiqzsgli.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ttlexege.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gjdlmkmf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yliccnmq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2drnnfiqf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jqhasgzd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ozirjeou.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xdghbcjm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ymkrnsmv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2idkcjtvr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wkrzlhgv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2czopagxq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mbcqynuu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2krsycgdh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pztfvfkc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iwamhury.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fwyecjny.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hlyltfrp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2arusnlvi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lwyyfjmh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mnusxxhs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hatqphyb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqxpfuxg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2plctusel.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wvxloxpr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ioxiniqh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hgzxkrcx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zuqzlcmc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2orbuvhps.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lvhefzah.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nufbwaid.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xgxsxbji.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jfmgfyus.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2optyqqco.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2huaugdzv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rxggzliq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qeqsqiuk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kjrqejcz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2sldjpmeo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qqjqxjya.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mlhchxft.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fjbyesce.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bmhdoyle.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gsegdzkz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ppvzzcwd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ziqfqtjl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qmazmkuf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dexjnnzo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jgpazpxz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qonulxbc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2srvsxzxb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2havcylrf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zmjejsex.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qbmcamzn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2oxtmpgom.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vzewfyhp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ymqtakre.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2twryrhjz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2lyezjdyj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hwzriwaq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pepxrwre.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hooqmjzy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2swwevuiz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ormkhejl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2flpojoiv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yfnkgbfl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fanwnycu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wpltbzvq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lxpajluw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rivefykj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qkolltla.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vrivdfta.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fcqvrqkb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aapdwolj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2cvtstlen.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hwokvdsh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2rqcrqans.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2prghqhtf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vdahndyb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2egnryxsa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bobwqufl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2udhziduc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rrzielrt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lqhsbokm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lsmtnbeg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yzjfjklr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2aojtfyzg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2khnzvwjp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dtawyndq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hbnszwdn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2foqwhqdc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hbwvuwaj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ygewxtcf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gpiztyeq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wvnohfko.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hxnnmdti.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tsuefupj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2myhfxolx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nodksllx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dlluafwf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ueccvfjd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kpfjkavm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ellqbhhd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dczvdvrz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gusulzpe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vwuengyn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ajtivjar.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bpqceviq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rsialjzr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ehqtekuw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eizrlqhg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sjnvqyuj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nzzvifik.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2bxpdyhhz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gjdvfrre.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bxxukice.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ovlanxrk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jddmxzox.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sgaxbdhr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vricabdf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hzrgcmud.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xwynmsgw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2emugbtno.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uthcpofq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ityxunvm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2auwydebn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eqwwlbph.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2acjlyodz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2soqpgjsl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ywaaxwyn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aslzjvul.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mkjqsmer.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ypvwnxck.html


<!-- 参考信息 -->