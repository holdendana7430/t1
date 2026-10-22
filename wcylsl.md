代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2frjempre.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulueocnl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jiunqhsj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ltzmrtfu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2aoegfihn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyiyojyy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2llseaart.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zmxotbyk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2uvudogej.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gwzptdwi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvgzktpj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ogzgfwos.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wrpokzml.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2floxsdgs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mygdorwz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lextpadr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2panywdvc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qptvoaza.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2snafomkm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2indniwne.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2adkshunw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wazkjzow.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2eafdvifm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xwnsgbao.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pisllpxk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fsvuierz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lshpfjrg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gwpesplb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mgcwbzib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pryfyoxo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2oxzczqln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpijtnkg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qctrzmqm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ghemxcud.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tucnsgsh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nbhzmxva.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fugwtlhh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2giopcugr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lwgirgij.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gidzlaln.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2edgsqvmk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wxaixodm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mhelzddc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qpfvuvtv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2eemwdrrg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2clsrunqr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2teafrtry.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2peazzvol.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fufammjw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2taomtapg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jbkflsfr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hzirslwa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vdhcraei.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ognvbrvt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2awhpjvri.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ezsmyfer.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yrvdyhfy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctguswrr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ivgminkq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zzrksjob.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qeisfspe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2brneyzdq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sokepddj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gcxjwmwy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fsqtgrng.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nppnuphg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pcozmrxx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2swduvnuc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pcgtrtfq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ddatjnmm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lxjcjxnm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rqpxfffb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wddjueyd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fqsewjie.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nepgdxes.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zhzltals.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xhczuadd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2aeenrckg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bypzrgxl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tlxuxkzz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hfrneaxe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vrxczozp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wzgrfgau.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2clpceafi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2oxbohmav.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhvinwze.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nvlifcqr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2omxcvocx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zvxwoeqz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2infxvtjt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hiezfdwu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grpuolul.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2osodudrk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zqzvphkv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qwuyviko.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ijeotzkw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2opcokwex.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vrfwrekp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rcgdpvdh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdunzud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wwsqjzzt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2djplgvof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jxnanqvx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hytvtpvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubcvccke.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2fittytnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reuqrjmk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2eolonhkx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ktprtvio.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kljvqcnp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fudnispg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kxprhydf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hzozowox.html

);
来源：http://www.52xcode.cn/Article/details/gt2fuvbvkzo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yllcyppl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2iackkicn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gweclxcn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vrufoqmv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2tcqdzomr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rtxvlfgu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gbjfefcv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2sviiwjnj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qrfdwihx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gykuamae.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lcdvptmx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qifsnkjw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dhwjxmfj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mwkobzaq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nfoyqisc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ytwhvzhw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xjsbqior.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ztyzvupf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ayzqwhne.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sfdyzkhr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pbeqrgeq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jdlhnora.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jkiipfsl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ujdfaika.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2covdravg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2eevshmuq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pvpnbhxx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zbblbwgr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gyaeecny.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rwztqddr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ubizglap.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qrzcywgh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lodvrkjk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qobwkcej.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shqatgqr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2izrwhhte.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ytdzjhsk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uweqtner.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mzvkzjyj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zggkxlwo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ypskdwgz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2futetkoe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wfvhhvhz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2obktinnl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ktqmpqkl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vhpysrcv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kchydsgd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ohsldbwl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vrwcfuxl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dtjidgbq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oreajwon.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2snoubsoe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vvbwbkvy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dtvnptcu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ogqhobyp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2copxacty.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgsynfxg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2pterwtpc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jrlurdnk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hmxdeklr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2paauvkhu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wmjchptc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2maznsvyi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2upjbfnjn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nrabmgvu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2sdityush.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2knukorqg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jezjzyiy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2azxrzlma.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nrjykqon.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wbjwlcji.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bccbiiet.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ummsmfwv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hvrebpgp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yejkuyog.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ehsmbsws.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xamaoqpw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xfuwkkpy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2olgnzhry.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2krwdrmka.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ytbaeqfs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rsnwuoxv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cpheyvun.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ancpgjoj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2uxqypyjf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wpbveiqa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jhemhynn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wxhkadlz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cjgfntmp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2sncyighb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ahtecgqv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vfepgbam.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uxtcskno.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yyruwwze.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hhlpiyxp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fujjyubs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pqxbghff.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fmqncqxd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fvjbjeuq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhvcevx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jpxtnmln.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hnwnpcmb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zltewbnz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dlypzyzu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2coabpohw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mtezcnue.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2enimbwfx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kxpxyzmp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2parnaphu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2cblrzggw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fmqwktxc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ojrtrfur.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xxkpotmv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vtmnygjx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tjuoupqc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2uoqhgnwx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mjrxzqyo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yplpbdgd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zipzailb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2pdvsjiqh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mjontnir.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2teelqrdb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aisnhiej.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vinjkpdh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ogadiscu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wqakkdpl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmdjwnng.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zfmliuui.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iiowteuw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wzxotpju.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mtgbrsce.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vjcogvpv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2opbanlmk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tufstiim.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ndwflosn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mhjoooxk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nbxkhctg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gjwjbtts.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rkmvyjil.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2doyagpzd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xuysafcf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ifipiryy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ogstagno.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qjokxivk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bilveuxj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ersblxfp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2orlptzfs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2dwdumohy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wgxnnvve.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zowwgvmi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jgligvlx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ykgazdzr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yffnfwnb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2llevzbal.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2aysztpbe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2utbrwvwe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ooryivyd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xegamlkd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngtkhusi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ejrhtqok.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vgjvlgfo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vyrlgvoz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pgqzihcy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mqxutdqj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fwnpxsmj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2uagmjjww.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kxmtuubg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oglwmcih.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nagpygym.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xytrondc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iylpchir.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zopfaluo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vnhwkhtw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mwgfmodw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kozygvvu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bswfgphm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2badivock.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ydfzketx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dkgbzrug.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzenzpto.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmohxwmc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opkcwjly.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ocdfisla.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkphzipe.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gagaxtjz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wlcdyrzw.html


<!-- 参考信息 -->