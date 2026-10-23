代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3chxqfmqc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3prmqndhb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bqvsxnuf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gvqokfuc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lfwhhffm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3odiviwdt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bxrlzjml.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hunkviwt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lssedgsp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qswzyypu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jshdlziw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yzoyxomo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3isivhjsc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3bftaoeey.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rlesrhvm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rxpdxuek.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rsaujhpa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bmvppunz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zvqqxzvo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvsvuhj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gcnewadj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cryoftzz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dfgrexox.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aiambqte.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kpkgovxq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dgejlput.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jjfsbldk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wnhjegpa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rduaqxpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ordcgngt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhnjyexu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acjfcckj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kkhdmrpv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wkfbgbxk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3coojqygb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qaslbxuv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qmoaqwkl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zpltyaxl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zcxumkdp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jyitkbqc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rpnqxeha.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qlyzywxa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pxkedjlb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jtnapjas.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mwohkwkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ugdszuaq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqkwffb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ktrkjzag.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfwdlrr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3mplooguo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eibeqzvz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ylrddoet.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ljqtrwky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3klbdrpxt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fwdypwxe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kcmyqtwh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lyuhcoug.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3opaqalnp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wqwfrcsm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zecutise.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fnzxmtjj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uyyxofht.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hlgclens.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ujrtwnll.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pvdzoset.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hbnjcbpv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jgaotzwu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qnhkigwu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zmywbxel.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xjtfznnd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3isnepukv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zqxpucye.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wlhyiyqf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3inypafce.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3baahotpc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cmwracqf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vfxxhqbn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3emubpoat.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qezdvzvl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oevhuktv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wtpkugvw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsloypvk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pjjgazkv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ywvsktzg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rsenmdbh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szalzeeo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zbxskmhn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jcvxwvhe.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3egdsouaz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3brwluvpk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mktalvhe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3itfmpeaj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ynnwzpsr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mxxxwpzj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qoqiyhvu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bbjgjluc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3evdqbxjp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cbbhhuam.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ewlfilis.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eokhtbyf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3btnozcdj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3davqkepo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jsiyrknm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hwhpqnsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjmabmet.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mfxusddy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvktmpup.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mlijzdnm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3aaydwsfa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rmxrvuhk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sowffpnu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3acpfleua.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3gbtgqwuy.html

);
来源：http://www.52xcode.cn/Article/details/gt3esaomirl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xniclkgv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vijflpdy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ozqpcblr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xrtwlqvt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3eaimyvdp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3khksisgh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3avtzdsvl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ceqfgzni.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nngeeczi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qpyxuxux.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ymsttvnk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cuogbhtg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mmejeftv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ouczspia.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qqlqnaso.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qfmxqiop.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhmlpkqt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3aqwdqoba.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3chxrurhn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zhaskzgv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gyrptelp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3uhsqhhon.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hihiwoom.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cmttpztc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ijpnhykp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3exdupeec.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vgztpbye.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tudtytnm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vwaztdvm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iigvlspx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ptnncksi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ejvdyzuk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3svwlqvoa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3myobnugz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtamzcmi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zppzrfol.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ciarakua.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3guseoyce.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kxphwbzq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jcaxebmu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nsuqbawu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kpqafzqb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3forbfrik.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ilguhzfu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cynqufhj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qofmmact.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wzgovdim.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3iuvwjaxg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jqnyubyz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3fzbhrlvx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ywkdyhtl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bcmvygni.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvmflozk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3embdtwss.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hzyrsqts.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3sqswwowu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gxgkodax.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3fgiyncpe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqkumhfh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3iytollmi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bgyccjzp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jcjzlwur.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eydzxuiq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3aiptwyip.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mpaqxtnw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pcygettm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3reeqlymf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ovceuqtz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rewowaaj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3mxyykwcy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rlynpoyw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mpllxdvk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3zwdcykwk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ythbbqse.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rtknqazb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpvxqjdx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gdxwdnsn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sovghsux.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ajuxsyyn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vhvjvtip.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hwyobokb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3loqnifwd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3avunzntn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3angiylis.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3hnncwtng.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hxlxxgup.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zbzrtkfx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xpqakwnz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qnkpvbew.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bbtaqzjm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lxnijzqx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3exuqpeuv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fkguwmyd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ewhnbjpg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mkbhhxml.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dkicbxss.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rydfguos.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vbqmdxwl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ptupdrir.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mofhcrbd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vmmxvpem.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fgmqivnh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3trtrjunq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kvoqvypy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3whulwegc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3csusasmo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xkgywful.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jkcrtmzp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ruphpwir.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mkniuigm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gcsblplp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hhtrxueq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3boebzwoa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jwtnxsxo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dkfeohic.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nzuuqedp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vlbhxpjj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ayslevlp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3logcpatk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vbwbqred.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ndnlkuvg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xeuwhsrj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3glffchgt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xjdhelvo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uguryugj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dcjfgjxw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dynndtfl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zlqbmgqw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dwsbefhv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wvecbmba.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wediikln.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qqgoymdm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dddvwldo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gdqsrowl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hxvguijn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kvzkciyi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3egvdbzbt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ecljkxex.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fsammibt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3plrmxyck.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tlklchcf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fzgdexmn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gchabkdt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3notqunhg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3znyltctd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3knscgmdz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3omqymfeo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qstcjdrl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pmkxohvb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wxcwwwsm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vgmmpili.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3yjwlmlsr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3eohbqlyg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3deptqcii.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gaurboae.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ufcjxhww.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bovwhkuq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bwpwchij.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufixlsix.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rdwiqqiy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hmjliccr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bcdncaqt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3fuapwwre.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tcbxlewa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mdopzabh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bnnzhjeb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ngwkqefw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ussgeagy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ubykdtqh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pbnqbbap.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xuaomabb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cpbcccgn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wbujcnnv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hxfebntq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3opemobjj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgurfopn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3okvsgeny.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqugxeig.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qkmfgane.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bpyukbit.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3brfzizbs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fmlzowkz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wdnmvgkb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lodtmrak.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lxrfhifv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hkuqepah.html


<!-- 参考信息 -->