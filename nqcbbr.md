代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fmooundv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mhubknai.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nzoubuzd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mzpfvprs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ulztplrv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wbwceoly.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsvhgbza.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gdxypfni.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2muxamzji.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ohatbvud.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wtqivzae.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tfqeltwm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ipmvlgcg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ouaglgzb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhiuyiw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxcaixy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vichqhfu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2smrapkxn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2krexmxnm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ophyvbof.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hognpvbh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ryqjwfai.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ogjqjxuv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rcrbqdtj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ilmcsutf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2czexukja.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2olwsubtr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2naoqexvw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tfepemsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqeiboso.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2teoquynx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwggqpux.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zgsqwlhv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vypbrspu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ppcbmklr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xvxjvmwm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2trzpjzhy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fxameulr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jphfisvu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pejncola.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mjrokxqh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pdyxxaex.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ccunbvsx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bqttgigs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ohypgckj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2axjsfpym.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vpmypogr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rmmssusb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2crrwyhhp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jjdadxga.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ugimfydd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zrnbgqgd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ublauvsg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dlkdkbew.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yvbohpij.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vetwnifi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ckhrhgpv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2alrsyzle.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mhzhhcua.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vjzshywz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2reszrfdd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pdoifnhy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vsuercyz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sjfklkbo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mqqtgjht.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2udwduast.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2alieafny.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rffjwrtg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hrtarurx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pjlruebk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lxhpjufk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2msnpcwuc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdqigan.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lrorrixq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lfnkrdzb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2pflwqudk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2csimnmwa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xzrmrvwm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lepinhsu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2foyzikiy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wykldgck.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqoqweun.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2majjbrjf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2rznfubwp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hyijvutj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yghpdsrw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cufhwdkw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bkggtgqv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rbasnyik.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2byaqqdfm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qhjmtzjc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwktarew.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lnxmkeba.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lktniaxf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2klpywwmi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2xvoenrfh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtyxlkn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qtsvyhnj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gygnacwj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cesxgubg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2sryytmmn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nicsiemg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2watamvgy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ceyyaeas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxchntkl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tdssxhuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmzbpihb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ilalzwsl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nnuvytjy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2plibxflw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pedswtxt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zjuqaxdt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rvcspijv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ulfqtrxx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ppfjzdzm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2yvfivzbv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pfcwutcw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bclwmkin.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2povvtspb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2nllvmtbg.html

);
来源：http://www.52xcode.cn/Article/details/gt2lofpbfom.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jjfwkstq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2uucwbuhx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mrntusho.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2eznpzuzj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vnxuizye.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2afbyyobd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uurkgxrf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2cwiukqdf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vnxfbzsf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2klzergdg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ayyrnndw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2thsroywg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qxstdyve.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sjvbbhtt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gbtlvdbg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dandcwvn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hirfgksq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2phxyslik.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ityobvgb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bmutaqia.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2grrzknao.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mnhhvzzz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nppguuqg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ugaallnc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yjneedzg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nsekdlpe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tmehhtzw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2idwjbfea.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rpoxnfhd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvfchoyb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tyrgpsbx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2iwplpwxv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2scujaqxo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2pbxosqci.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hekeymdf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2votaeyss.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uyuudjqf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ydpwchwz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hxzyfzmq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2smioqgzr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kthyvtdi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nkxrokvl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2miufjydw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2osegnduw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gvgyzhyr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqampkpu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gddirxvs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tcznsygc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2maiyrquj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtfibuyc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rnafgtsh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wkwksvjv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xbotjout.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lrjjolqz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qzqglovy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbsmbylh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kffbnhry.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fboingwc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wdkslxew.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jtyhhlsl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hnbjmyab.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tgudcdgq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2clbbcjef.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2epzmwdxd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2uakejhpq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hfofvdbj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sdghkdtr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qsfryzjn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lshbzsai.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cgvzffpl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zlpettqw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zqjcvkcm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kvrpvfwd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dagouhke.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2piepuryx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2psoxxipu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vcqawnlq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2uyboapde.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gnluekkf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2akbsyqlo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mcsznrgr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2oqmnmgjj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2icrihcnj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2brxsybsw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ccznbhwu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kqghfzxa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pdguqdcn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jnbcyelf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ppcutymq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cpqcbacn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2imvzkqpp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2koxayynm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2firydmgo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2edsamhwl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mqkwplck.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rsjereen.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xmakzvhi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bisikeuo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jtfllwpv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2aglgaejh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ehgufstj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cyismgjv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vavklkfv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wsrzbtvh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nyecxqke.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bzkbhhit.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ksqdikqd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fbhpaaos.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2twhhwuth.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2omgmzfgx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xmbqctgk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rfhhtkjf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xahldxob.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2svnbhgts.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qdzaestv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fukyktou.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mtzhvlgu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qzqqwvod.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jppmthrx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2blrfduyp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wspqopum.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2anmvgnro.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ymvbpwxv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2flewwjvi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pdgjgrun.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2quwutzbz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xjgflzkl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ynvnnews.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2whilixup.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2audfzsoa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wloshwov.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2orrgwqyv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bgldvuuk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tltwddeh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2vcifmukh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2txrboygm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2evemqcpr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2azcolzkq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2tjoooyog.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2edbpsdiv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xbhvgsqo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hbxrkrqc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nwcwtnhm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fmsfjfes.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hyezphdm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2oevgperd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2rtxkexpr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ckogahoz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rczqvbmi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2uicppidf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2feogfnma.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncnupujy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ropcalux.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lgsndpot.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2umpcbyhe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ddznakws.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qxkoubng.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ccyctrza.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hmihhjoi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nfwbofns.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hhyxtqid.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vrykiwjk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2npchtmtk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jgcnzwnf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2uhtmniva.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ntoqfqfm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2aiejmbze.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hhctfhxl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncvvsbly.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2icqumpdo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnzugtpf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ldoxilra.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdnkoaoa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2proeaqrf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2siazvizr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wzwombfb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2roockihx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mekgeotx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2alhjyfxo.html


<!-- 参考信息 -->