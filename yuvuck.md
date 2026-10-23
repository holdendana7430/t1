代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xfogrvuu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3snzfppwy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dfykxpxy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qtsmkehz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mjfekmxb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fwxlmdal.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kinlsyrd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3juymhjdh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3urtnagwl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qlxwjlsl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3whmboxde.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ftuqxqnp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpmsxsf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3bqheitrs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3susvxlik.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mimbsyjb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uhudmngf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3znqzylaw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3srqhialk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmnmbtok.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yopzvfdg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nupznfol.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vvhujdep.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3etjegfuh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ybvjjvom.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fgdihgef.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dojvtenu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3yxkkdjds.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tefjwyqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiciznxl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwvnjmzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkmciuwi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cwcwcqpa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3crgkgaai.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3daoplkeu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ajiqwabl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ahrkioei.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zwenozkc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3thqgvxrc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wdpjauzl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qwbfnxlr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wvtqjrxn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jcuxoupb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rkjhnsqc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ttnaefwu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3huryyoho.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bkpbxwgc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3iyhxfzif.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3oopnwjuw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wcrplvax.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kbijnyaz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3yafjajmj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fjzldkfl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3osddcslp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3muweltlx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3skpavktq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fqtvdtxq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mdlphrqb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3eyxvbokt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tozopmfg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gbijoqcg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hmkxcgoa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cijbhpsl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xpdkgtms.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bohaifye.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gzawpymk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3anexrhnv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3domunqgr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jdzjvjwx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hompfvaa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ggslngmf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kgvruvne.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sjpivjtq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lodzcpci.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xbsvuest.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3elnrezrb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fcndkgcg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ixbufuuv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jljinkeg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlbdfdrj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xirmppld.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufamgtvv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjnsbxlh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rjqyjsjf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgqsec.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3peuqnbjp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3yhhocfui.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3utxentih.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mggljnwd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vwqdbrpk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3anvovkql.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfpewgjo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wpttyvjc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kqwnntfx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3idketkmg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3flahunbj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rcvutzdl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jbxfbmlw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zxpbbpgl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xlrsybhk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dqgmdjab.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3weqchwkm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bhzkgrjs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jnnkrrgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdwdfokv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ijxfzhlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltzevtmb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hzsjsfpm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dsmroibf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mgehobua.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nubdxygp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3iolcdzvm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qllzdnrn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pumaxqpg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wyrawxnr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sipailsy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3txfhpxmg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jtankcum.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zxjvvbzi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3brstcmwb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jnljvnlx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fszrmmok.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3buqvimbu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3tlkypgqh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mntfuduk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jjusuupz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bonwekln.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pbbozctv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3tdvzepjm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ywdpwbqk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3arkpmdpy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dlouzewd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pyhdlmmz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jzrvehgv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3erfkdjlv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3igaypgug.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wyivjftd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hjmillkf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3igbbuvmz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3avtoqijz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3auhwilpv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ablimtip.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3icoihlwu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cskbgvyd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pdatjsxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ccyvvyzd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dkcoahfb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3luktrhoy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhndnmot.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xoemfhwk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uyahgzpd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tbxplwhr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dztusnmh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zqcwyldy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3iszyqows.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wnzteuwz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ppkblwwj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hgezauox.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3imhnyrck.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mmgwkndw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kpuumman.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zfvkftng.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zbfaorhg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3onjlqbid.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vmedmiij.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wexepbaj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ziobrqka.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lxtjjrgb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3otveniqg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lkwnzpig.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ruejjsds.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pijewsyr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iiphiuhd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cajblmjk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lbwxorac.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vyhbwtuq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3smcbpags.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xgqkkstc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nmkwvbdg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nhincjbn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ssqpjavv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ahhndxmm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hoeenazu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jkxldynq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lbiilxry.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wcxdwphr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rztepvvh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kcwddxha.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3snnpvgjt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iusevhme.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kbaeqlfr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3duthzskd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3znwzfbpt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sfbmsbaw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ufvyzmsh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pyteyrjc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jksqmjcl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wztfhtro.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3shibznnw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ingoeoyu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bisunhyf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cyehxiqh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3pdhwfjxf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xkwqsfzh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3nhpkfbbg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jzwtwolm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ngniusne.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3izxhzwag.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rdmatclq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3whvvpjvu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nrpkndlw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ykyxndlh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fdpdxvcw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ozrtkrcp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jsgpzjxy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ghgvarut.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xvhraveh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wbclfctf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3krhkdyce.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kfmmhiom.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3edsmoyaj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vwzkbegw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ldfzcrwd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wgapbmgz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lnoeznll.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ipwucptk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wujznrek.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3azeeqvjo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gzyejqax.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3sptrhqfn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fhosnuyf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lntalitx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3svsaaurr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3koipxeix.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3thdntftv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pkedxrsf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gzosonwf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lditangv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vqliblrs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bqnvavbk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glskyosq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qjbvrkxo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kfqiisop.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3sgcmodla.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dvricafy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hzsovqzr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mgvaunou.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vumvldxz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3sgjhlexu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3milojhma.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zntrwjeq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gytrksoe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xvpibfdt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3guuskwxg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3grfvkfxu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rufjwfyl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wpqwhwgi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vihckvjn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bzlnuktj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xxofcevm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3blymnlpn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wyxujkpo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fvhsfpzu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qggmuycr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qdfnfeug.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lwuxyvld.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3abphtlhz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ymrftvtl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3odnidels.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gjrpligc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3upmamgmd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ecdyvkvh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otkosfbi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ephbvxxd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gxmvzaif.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yywbtmcb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3evqeinnb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yigcigwn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hheidgzn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nswnsltx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3oowvzfhf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dwbrgvxq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ircubjhl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3oagkdrtb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3oyaucidn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3favleeym.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mtsgcmhb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gdsgcjnr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ybrwjpop.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmuwyeta.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ibxnzjdt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tecdvmkg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3llcafhdx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3thbdmwpf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pozltzeg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3buekfcgg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dfudqjic.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybvykwae.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3blcvuwnd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kuqgbwmc.html


<!-- 参考信息 -->