代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3epysnqqt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nvxhzhdu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fmbyxrjy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vzwbljyn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3liaeizyr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zcufvbcd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uadvleaj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jwzagkxu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fncliwwy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrqmtjzz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifzjdzfo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hxtwmsyo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hlciohlr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wmchnmdx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3eryjuecy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3eobonvxw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zzphwgzf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xccvqsxz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iusgtvom.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3koqrgmjg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3esjvfuqb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kvezqrfr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rkmzbwwe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yznkgtfu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fdjjioeg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qpxsipcm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3iqkfffzw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ieupdsbw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bwvgawcc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3muenufox.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dnaohnry.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3peycaccy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jyeaccgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iukgpkut.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lofwhshi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gofdogzd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gazrgyns.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rwfowovq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ydztajmj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3unrxkaph.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aeapoxsu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fkguyvwz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ylkzvzzh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zubqdsvh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ujnbxcpo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rzduzibd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3acflkmtw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hvbbxqkt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pssrgpep.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ipmkdzpw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3irjiubgh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jyntygul.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymbzojit.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ryiyakhv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxghqltk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nvxrqjvu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hwqsnmhd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zvwfvzlm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jgzqrxtu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ikoznwsp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uuhlxara.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ycclwgyj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3flrlwany.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cfebwkgl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kpwrjduj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kmsrwnsr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hobfwmhh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fvhmdgyc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cjqlidik.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kylecxjy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hiyjjnqj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bnztygzd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gtqigadx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wuevjgjl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bdvqicnb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3syigbqam.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3enmyjbej.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3smhwvwsp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bidztrnh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3atrlsvtx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xwqugnpa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kibycaed.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ytofmisb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ykncljef.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vnputazb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kjmfptsh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whoczzdz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mxhyepdp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3uuyewhpr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tqirxmza.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xtuhffgq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lxswfhjn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3yyddksoj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vvzscyml.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tifpdnib.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3divlvdfv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gqvyyaxx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3seahiyrk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3gvrczwkc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3frdpptfu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bwcloulz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jueastaa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fnwlapcu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hhjehxme.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3dkjposru.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bzxuymvh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3azigeikn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ecrpvedb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xroukdhb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xbsqlvon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxoukrzu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mfbulloh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tvhuvnhh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3awyjuudy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rpdzdeka.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3haggjpke.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eekehgqk.html

);
来源：http://www.52xcode.cn/Article/details/gt3vezftcvi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3btnfdjlb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jpsbqzjp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3evslsyha.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gpllmpaa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3yomunnge.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3eaxsftbz.html

);
来源：http://www.52xcode.cn/Article/details/gt3lcjkvbdx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fgjcoups.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ydajugke.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cjpzmgho.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ldykjyri.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mkddwcrc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3viuvuvgu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nurtjsem.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hqdzksdf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3btkqseno.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3buzqoylp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ngaxelnb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3clnatczq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3kxiruraa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ppkojrjr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dbipoxka.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qzzubkna.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mmgfihjs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hlbyriqn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jplupilu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3sxwpuayh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fzvirdiq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qgcqjafi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gpvumcwp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nhwyadtw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dghxmzqs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jybcqyun.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zkvykrqg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ffiyzcjo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3krcapmxm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmiquogi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3npunmxjr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rrclkjnw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ljnmeyip.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3fnthafhj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jqqixmwf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uiablhpo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bsoojpgq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ehrfmgdj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3oswtfllo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qruyvodc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3zckhlmtd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jsoofmen.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xlyqrnzt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cdffnkdu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3milaatqa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbwopuhq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iqrvlwkk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rbqjjict.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yjpltsct.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3schqqmnh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bihwgmjx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwftlyzc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rjzwojps.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lohgrcmo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wbcdmiwj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wjjbvocy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3heurgxmo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mdzlalwn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uimrdfht.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mxlbpwmy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bqxianiv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ayngzzra.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ztjheovq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jkfktnmg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ekibcnpf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vonithxa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3amtzeuuv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xarhrfgo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3neymlzpm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3chiwoqyr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3htuhejsz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pkqorshg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vqkbuxuw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hrcorzgy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ipzhlshl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uwzgxzds.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3atygobzb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qxnordyb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fskffsve.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lyretwqz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fvwzqlof.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ahbkdmkz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3pmewdktz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3blyaapxd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jcvnnenu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jmkamjnk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vvfyydhm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ehlnyyhd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dpulsfha.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rcucareg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dhgbegwm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ulqvslez.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3asmhmwji.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ywiywjpl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3glqamfud.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3txpfojqe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3klrrsywn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wcodkjjk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vbyigifc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pwrxetvy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3conxdpab.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3stenwfvk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jcznxqjp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nttkbrtc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jjwyszmf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mrehnvqu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qqsdxaqe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3guufyubc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3yjtqjibo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3npydalkp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wlcukwaf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3scbmuhmw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hlnsjkux.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3geqjxlil.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gqfzuzni.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hxflloer.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rftuuvtc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xotrorbz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bhwdcxyb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3piwnqddh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uhynwmbs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fhtdstxm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wfnothit.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmdifnpb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3eihlpioi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3hpwbaqsu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tftnxbjf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bdpyzvps.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fnzvsigf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jyuwyhqr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ykcrmrpc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ezozyeup.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3njdhhscw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hjapbnyf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gsupfkmu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qdptiyfi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3spyhhbet.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nogfiwzi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xaajatnp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3etkxhysz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3oisbvjrs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3jgkkqtmr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bvinildd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qqlqcdaa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wrpqvfca.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sjdnmjeb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ckctcidr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltxkaofm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3avvynpgh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qghnlfsl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jbhjtqxk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgwxmoqo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3moatmwnt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dszuwhhd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qihtjkow.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ygetdnnm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uoyrdmwq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dqhghfwd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zlqiyrcx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mccmzxga.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3swnyridf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yggovelc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sfbdrepo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hyravxzl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3evzqqyna.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vnqshjga.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pvayfoyi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3adrrgtpb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubmipkeo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3loajpgqh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbxkpnmn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uglqoebs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3alrdbvvs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rhwmgzat.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pctigxhc.html


<!-- 参考信息 -->