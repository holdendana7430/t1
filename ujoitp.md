代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lpdcyvce.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijnaldfx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kzglkflx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gwvhvycf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fsoalukw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jewqvghg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgraokww.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lqdhiaqs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rkcuhqea.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fvylqyeb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2avkcjpew.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rzxgelwp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ffwubiml.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vxmjpbya.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vdkpucqh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dypdcayw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hxjyxqsr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sncuqovs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvcrnlm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ognerskd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2igiddkgh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2smpzmwqb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgnylafh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2placuzbe.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dikbvlei.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kvmkevin.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lchtxzeq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rxjpdpoo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mqxkocsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wertjtpv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dopvirtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlvdjadf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qehwgwvy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fakwdiop.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fbxrrijt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yaqhybvw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mhulcmil.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vuixqxor.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2txdjtnna.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wpxauqqz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mdpnpoku.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jzteuucy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qaywotnw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rynxfwrv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hbxnugdv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fhfnlwrz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oasurzsl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rasdxsun.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2pexuebzb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2puudzics.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rukgapqb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hmognlam.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ymduejxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vrqszmap.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zjacuhhn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2otwsbqdp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tmxqsuxn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zqpaukbx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fkgudhxf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2buuilxfk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2exgtzquh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tdcbbaor.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gsaptnlu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pnaaogiq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2parxqpsp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vqrkdefa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2koueemmf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yywfjsfg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2unczholm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ijzdxatn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zfpyycnw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rihcjjwe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2iyrfrvya.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fygnosta.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nebquwaz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gzihkgtg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2sznmbtvo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pudpwytb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cknyltgh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jiromduu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kfrzhwlq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzdidiwy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rumqhpkv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2noxdtzny.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lupcpard.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fdekanht.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gjuzcklk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2mvhzcckl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zsujldxf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hgujkbza.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2baxbbuip.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntjutxck.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2cvzrjtzc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zmtpkbyh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zryclzad.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2amtcdqpv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vyugxeso.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jgcnhgfo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bjgvtfaa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2njfhduvj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mexxqixs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qrxdaczf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qplsfauv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ixqrtctn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzcynqpe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2msoxzozp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyihdwoe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tuvobpqc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pgdlaouu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2byicobcs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2anidpybg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gpqtrabr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2civmjdrc.html

);
来源：http://www.52xcode.cn/Article/details/gt2gbbszupm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ilpmombm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2edlckzcg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wschuvom.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nmywyawp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dtneazya.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vdyckckg.html

);
来源：http://www.52xcode.cn/Article/details/gt2dnkkziqi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2coemnkay.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mkdcgkfe.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqeutmls.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dfksjcsa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2aodeiayl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fnrahhds.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vvsximkb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vlqfzxch.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2esehogyi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mjsvtzkr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2iiatwfvm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qybwtatc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hmuzcmvb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hypfwdiw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2eiizgfeo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dwqdieak.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2brptsflu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sgeuicrl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qzgwfspd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ecemrmcc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2twhrbrhq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wzsrdzym.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2psjjgxua.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tnwwhjpo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qvfrvzyl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jvaidwsz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ahrfvzja.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2krptruoh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pdmlpumn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfokbarm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2uiohyhur.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdumumdk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gibbklud.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2oxgkedaz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2rkksjcby.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yyrhquly.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yailstqs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tujfnkpl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qhgylkmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dvhyjbak.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mnbryigd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jxtxhfnt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kmzoplij.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pqryplhc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2opbutjyc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otknjgvq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lspuwqlu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gozszvsu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kmpeqlpz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ljufudvb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rxekhozy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nozwflin.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vwctxtel.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iputpixv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lncavmxz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cezoalxu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ldjzkjkb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xmsfittv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gxhcwgwd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dkjeeydv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rdfarutq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2waozfyta.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xkcldzde.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xtnvyxxq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iqepimrv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qzvtonsg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cgjkkijw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lpacxkgx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2egzyicqn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zbunybmh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tcueczfe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2fvmxndez.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zusbaarp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2svrzuxhh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fbtxezoj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tjeczdgk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qohaoklo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pjxhqcfx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qecpxttu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hvkaffno.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yvastwjq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jruntszy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jdkoesak.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2iddzgtpk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fdotaafo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ejjapefo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jayjzbks.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xydqgnvu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cwnvmzbl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rmaxzfda.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gsvttkqt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2aqcctcbe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hthyyrcl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tgavscxw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uzmbwezp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pcuoogzc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yaahjwoz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qzkdundr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ookqbioi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2liyhthvv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lihxcueh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2yasaqihm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kvpikfxt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2humoenbr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vvdjdjuo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ndxqgxty.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lsxxsiyw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gquujfkd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vhvemhnp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jfpyujcs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vynecjqx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tatbbrdl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ixjczxmv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ygxamukm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qjxnomtv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2aalvvmkp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xrckloqy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vlzwzsji.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2slnludba.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2megjpttt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2sdtkduqx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fmgtckzq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2owgitkyc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fxauuono.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tfavvrdi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2oywstokv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dakrorru.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qckzigfm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xoezipaa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gqfaeetq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2abclfsit.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ybontbhd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ggoiapql.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xmxwbmgt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2epcihila.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fcoopyqo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rmdjtanm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lartmbrd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mrzbamzv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bbrhrnmp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vnrtmvbm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ipzumkvd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2drbcercd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tcrceukp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rlvgitsm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2agkfhwku.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ppuqykta.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2absiohwo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gnevrdzh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fhmgzpoe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2asbhhwbm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfbygcsl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ypvgwvvi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rwmxnmbx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nwvcbbvv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ulkechiv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cbdelfnx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ikfrzzqx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fmxoxhhc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pwzcfjcl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2aaychnuj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xgzjjkdl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ztbmguvw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rbthrltx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2crqxhicx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xzqvwlbt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2nnfarlpx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rqkzlwxd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2itjuxnqw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qfxiafwo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2syehcnjm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fybodkia.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hiqmkzbc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oxjbzyql.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2huuwbbks.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qilnwkyq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnxoglcr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2senjiigj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pbyoenls.html


<!-- 参考信息 -->