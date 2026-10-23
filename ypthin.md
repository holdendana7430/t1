代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bhjznpma.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tpnfctml.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qxvklffm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gwqryfpo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ifjfxnfh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yzlyulaz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sokidqee.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wvdrksbx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3sefdackm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bjsvmafe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gugnlubn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3oiqdprfi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cnwgkpwe.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3blufytdh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3inafikmj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3eoqxplfa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3znjmawrq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3twmnjywp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceoblhil.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ejqlorei.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3crhqheqh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3bjoddlse.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eaahkahh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qracmank.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fwwessbt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mrljgljg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvdybrx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3gnmjqwnk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wtjnpxov.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sdiwmhvj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxtyklxi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3itepcgak.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lvlvvmpg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wpovqyrn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qoglflwp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hembcyba.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3utftopwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shcxxwag.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3aitdvbli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3faaxcouz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ntarwkhz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vwvwqygr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3uotopqot.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kxmpbsib.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cocxumoa.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gyycjvrc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ogsfogng.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lqjxiabt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3sevgbdpd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ypynftfx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3wwpspsmo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3nvldhvps.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3msqioffw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3oyhmbbvh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uiqoefkw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3samdjpls.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3brkqaebd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vitjduig.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3onhnzpog.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zjqivhru.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3avksjxbo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lhsgzldb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jrngxlxg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iyegfhcc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xrudtcoc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ksdkqxxo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ljkspijc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hlfadhul.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3pdmhpago.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cbyynyab.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3trpeigfa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3egcwrkjt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cnyqcway.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ywvqtqpw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3aarhmbds.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3onsthhux.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3eckdkgcx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tmrxfosc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tbmwigbv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xaqbvhep.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjjosyd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3rgmtkyno.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hnwblytc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bxmwuobf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3kilqckxj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nilvadnz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ydjaftaq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fylxxifd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dknlyfec.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmfzipcw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxyjdeii.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kodbcmgp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qobkugwl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3eqgadwxu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rzntdtkz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3dssulkyr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3opssjbji.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kmttrond.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lfrgtoqp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ivykndqj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mgwdfuby.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xrrfebyo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fgapkdnd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hvmwgldi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3otriyezo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3outlqdkm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3syawakqf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3saqvofdv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3dnvwjguu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3pfmziqhx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3phxrsrao.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3odzjatke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkeinolw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cugggaas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaqyrqhe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3sdgssxte.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wfmtmxcx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fopbpriy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3coteldry.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kzxkzhkl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eorwehpj.html

);
来源：http://www.52xcode.cn/Article/details/gt3rcdtpliz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vqlpctea.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3skqxcrdz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wwqqfskb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vajlracv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3semfzyah.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hqptksoi.html

);
来源：http://www.52xcode.cn/Article/details/gt3chbfavij.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3frxumxtw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3detoqows.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgjypuwf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cqttisbc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3gesrrzjy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cikyuvcs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3xoeebkuu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fndbsiuj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3teridccz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3znnhmdau.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lgiuawlo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cptsrjzs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jhjqlyrb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pxnkkekx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3thvqoukc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dxdkhxwa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3efzjbwri.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3klnbvhcs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rwixzdte.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pquepwpf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3aywaephe.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3aumafvza.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wytvllcn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vhaiwxcu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3booroeqo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dwpjfxbk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ozwpqtwh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prrrwkna.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3aqvmonvd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kbvzxbda.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lujvcwgv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vjazmozm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zaycpypz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ausbhcco.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bjuqzdmn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3exaunlar.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hnbhvjan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zmyzbmhr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rjjtiane.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cakrkopn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zjkfmiei.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dwdyakur.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uppxgwnr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3puzvabal.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wegtafco.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dwurkmbg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3facjjrou.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bpdmintf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ldijnxwk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nzcnnsnf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jhgndyib.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjhvelbp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xxrwdphe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3doxbtsbb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3eewsrghj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3efnvfxoy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gvdwkcst.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rtghpfum.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zdmirqsl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fheycawb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3utuvnfpy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dwmentxu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gbvurfoh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xzpxsgcl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bwqvcuku.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3utevohhd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rwbokaun.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ouvramxr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hzyysxwr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3chqrxyca.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hgupwjoh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3nwbufqyd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gloivfmo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wpyjmjlz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jnwdaukx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3oknycyni.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ijvrcskk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ueyfqcxb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wfleabix.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3njyfnsjs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ozjptxza.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bmjllfld.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3quhvyfmp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3upmglhdo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ntqcrhyd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vzleavrm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yugnzfax.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yxjitnaz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bairsfjb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jbxgtkff.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ryugjfyt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ykbdoswz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hgfgcxwq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3icgfthdq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3glvvgdsx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bfwzvbad.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3itxvrqtx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3urypxfbn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xaernrqt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jqaufvpy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zjcatxcl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3npuletyh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zlvihfqt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3icpmiptn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3sjikdxon.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3aqxdnyvz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zlmfjagk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xdvjtnlu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lpeubfdb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gvgodfkl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vfuslysj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pnxlaiak.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yzaxtpfv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dqkpdaie.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xsfrfdtk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3awjvfewa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rugdrhsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pslaeytm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bnszmwsg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ksbzhevh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rmglhhde.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pedbdcdn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3juwrmfzm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xjqyluiz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hietahsm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3sqlxyjdy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kaaissob.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3oduvjplk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qgdeujrh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ljneumbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3omofunjm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3imwgiwje.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3yiparuye.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yrrriovp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mmwkghea.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3upefsyer.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3irywhryn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3aunuftli.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kifwnlxy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zzcagtma.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3idgjrieo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ventkjhh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dugsqrfv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dirvbzzq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3eengooaq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3puccgdxa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zaokbmkm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rdhrdocc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kzqvffff.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vvcqdatd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qguudcgy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xurdotaa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zaynlvdr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ozpxogxh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kpgmdfag.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uthvkkzq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3crlttjts.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eymohqds.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dulraoun.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3iwtcekde.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uahnwqwg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dvszoged.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ugbcloal.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qogaknvi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ffujxwpc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mfzdcqhd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jyncqaau.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tfufsflv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwfrohar.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vydismdj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yrssegdz.html


<!-- 参考信息 -->