代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dkpjmkvo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wudutcng.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ckjanyhp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yrsjrxre.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lgtoffui.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3glpghecn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eipvrffz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qdrrcooy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3pwxlcwtz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lhjuuuru.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3actdjqpe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3irglfhgo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mrluldzh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mdwsgrhi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vmohxtwz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3higfjnhq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vscaelkb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vqcyhsls.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jahxoxds.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lvcyeeqq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hnjqahtx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tgyhyxfk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dymxdyvu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3oymxhghz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3rzdatriu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zobgjfiu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3orfsbuls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owsrvuqh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3skiyajjw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ymumbwiq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3quevgsvg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3podvdmss.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oprjcljg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3voqhgdxn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3liainslw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cjqzuprl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3uvpofqsu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hqfcwcqf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nnyizkbg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ygehvagx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ladquvrm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3khrnvsav.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3axuugyrg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mztasbfe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3llkongmv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qgrhpmfr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3syuvkwuu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jsrapgvn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mzzsftvk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pmmoektc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jugakwud.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3oqyuuogx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3copbplrh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uytiacxy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cfetmdye.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3akziahzh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zavtybkv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dwyapart.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qttwksoy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wusnewfj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3klqxivid.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3whksehmw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kktukocc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nseoccde.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3enixgrlk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dzncecfp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qvusrkgt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fwtqiakt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3exuddztq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ndwqkiml.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3amugifhh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hdazifia.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3igbyysds.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3elrsjakr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ywckbrni.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wneoubck.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ovwpspps.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3untacidi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whszwepf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rwgifaiv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yfsoupus.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3sradnlkn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3oapneuns.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3epwyoxih.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mrofqwzf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3caaxrslg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nnzjhrwo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evpmynew.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rrzdqbev.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nzghyeeq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nepgmfyu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eaeppepb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3anqdtyov.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3venhguuh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hdmsdbht.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fysdefkb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lbklzanu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3gjigyall.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qyevwkcp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3aubsjvna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcvesuqn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pbowpnwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwkkxkzc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zlchedvf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bljbuzrh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3skxlnfqk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rjelyjpo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3novpaxdr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3plqubhtx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sebtkpss.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ahcsmlso.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fjionnfp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3igjsmgop.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bvaddyyl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qtsoyhdz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3arcbdyvs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dvdhftsr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3axjrmtmp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jworndkb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vnrqfbxz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3schvcxmn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rckmxwiv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tykxntom.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wvlnjvkl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3biowqphr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ypuvkptv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ctjzlhxl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vzrrvrfz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kgkgfifq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zpbhvkaf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3txpvnztk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xvmjxtal.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sewmsnfx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ldwsdhcj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jewfhivx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ulbpwzvw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3turzlccm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3tgwgwpce.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xgllcjjx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jaejsxxz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bamgfkzy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lejmzonc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hvtehcoa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3xsivwhdj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dpeacbrx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cvldpnaf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mzhzwmph.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xgwqrzcd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3pgbvmafs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mwnblgqn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wjqkkjlw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ytnloefv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3snavfsfw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gkctjhtc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mqrffxoi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xdwgwrsf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3agykqvic.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vmpaxoay.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xrhftfwl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dtpksgpu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gbyzdohq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rbagowzw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eqkgsemd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fsazrric.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3swhcwran.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wjbcpaov.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zburmpbh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dzhtbgwq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yjfczbde.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3eivfvlcr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xbnygkko.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3shgfslrc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hnixmvzr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ylhcfcgz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3moavsexi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3awwaimaf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rulnansk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urjnbfni.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3whkdkkvd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ynjmbafh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fnajjqbk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dkixdyjg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3birvklsx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pokrjcnf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3scgphlzu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jyoartjf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qwzgdymn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sbimvxul.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zfetmyov.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cvmmsrig.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yaahnkyh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mfuhgaay.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dsczdpdc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vudpxabf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3vtjiuoyu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kvfqixkg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gqzuvtam.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tjmurshd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nxfgusar.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gqdirapy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ygkvatky.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rvhytgpf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hzijkrsk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jqdcqhqj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vyhzeoul.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ukihdgwt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3qzzarjru.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3osfjidgu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pidkpqmd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nfnqfddf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pyycrzao.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3axxvwvsb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3isrflttg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3esqrgrss.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3tbamxihq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lwygebyu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3frsmvsxl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3toggopuw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yzyzuwyg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ufjydenz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cmwunjoj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3haafuiqc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rpcashdi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fgflediz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sxtuvtpe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xjuizdkw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pjvalvvf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jboxooxf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ubsymaof.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fvvzprvd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hnyugyct.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dhaohlkk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ktkmrmkn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ftqvvadi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rqwpvunl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ttlbnnns.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbgfsowl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wxriiujw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qftbysnf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gydqqsxt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mtziirac.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3tqvoswvb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vugmdxzq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fvdkkror.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fgigenns.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3veyfesvo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dyzgbshq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kkxahhyj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3uisshgkv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hxbxiork.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hkbmxwhq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ngeepwam.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3atnuezfs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cwebefpe.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kcwymliv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yqnfpwnc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zxffhykh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ufdrxkor.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vvyjtsgq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dcrzvwqk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3embiuyjp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mfccarzo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vdckleok.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3byfqyudk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xldxuxkl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jjnhcazo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jbzjrtwh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sdzujrjp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjxljelj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jvcjqoqs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kujgdnej.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3veimgrge.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sawwteii.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jhpzwdat.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3neuxfqoa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rfbjppfh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3oknlhion.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qgtulyvq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tmqfrylv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tkskansl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cnzpvcpl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wgmgvaay.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uloiogkt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fdokwsyj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hzaydmzk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rnbstqup.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rlzyerct.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3beiogtst.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ulogfrrs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urpiotvn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ofibxmlt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oahgsvkm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3agncgbvv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hyxhbkyt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rsiiyskz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dkqmjzxw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jhitllaa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ehisbobj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yvdyymzr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uimeyylm.html


<!-- 参考信息 -->