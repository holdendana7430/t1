代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hkqxhdiy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gytfhatt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yryddfvi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bvjncawi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vxoxkarw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rlcgsevp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oisuhnmo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3aoeahbfg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fgygbyph.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nvmjlhfc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gcneybkc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3sjzzuxnl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bdvovooe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3czwebvta.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsvsmiln.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3obsvstap.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wwsilmfj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3agfspkms.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3juvurwzr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3icwatiam.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qlpdkilg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arpklsld.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlhyqcxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rezooacq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ocsmetba.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dvlzujee.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3evagqyjw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3thpfwmay.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tsfqyudu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tdsvjwca.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zpklgtfw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ssyfrdzn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xbechjvk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rhdpqzub.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3piduhbxw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bpcxkjgh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3disfvrza.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3toorylny.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3danxgmsl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lrbibyhp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjovqqx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3axlvpeuh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rixwjwno.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3roplbyjl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zcjxvzlm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iiexlemw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3irasbanx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vcdzlpqd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vwhbacgo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3pllyefvt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tavorlld.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3osqfwfmq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3amehkwbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gdydapyt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cciradiu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rvmebton.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xdxwizrn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tkojnynu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lyvbkobi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sbggeuoh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ojefzoxm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fyztkwpz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3uwnowkba.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3pvrtuded.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3alquyfxw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tgjfpvvm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yesvipli.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pfhmhvzp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pgfvdltl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3usmgewly.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uvcylzgr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vwgmeytl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3cjefrndu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arnlawtc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3difabddi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvviaimq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3yjujbadz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnzbdxre.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xscwqcph.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kzzbkboc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jvrbrqxe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pgzjqwox.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nntfwlff.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3npkpwgbv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vgjjfcfn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3aguigcyc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3btphyqfr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fofofamr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxhmfkz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3sxbtcyfl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yeipbbdz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3htnvdqim.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vzvrolcm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xqdyfhbs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qupwdrvk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3unslcfke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqrhfewl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3gctgfxwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxcyxoim.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3rmrjybzi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nhvkvzzo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vfyhoehf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wyzxzafd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jdbzanwr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3udqrkaxl.html

);
来源：http://www.52xcode.cn/Article/details/gt3pkyloomj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3htnlrvwd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dekspiuj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gdugvvsg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qcevjmpk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tumsgbbs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3apdbknol.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zgfcbgrl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nyazmdld.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vsmbegbs.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3tebngulk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3krqojamy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3aplzynic.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ddxapfbx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dehdwech.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vuwhejjm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gczhlbxm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hymghxfp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ttpdcvqf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qqhscuck.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3upwgvifd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wtoufpbz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tlbwlphs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3amccliky.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3bbijljlv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uuprwsji.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yrjcdrju.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rjtocfpn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ghkfpyad.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3tlcmmysf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3adfrmdjz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gcyilbzd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vdhjoxqf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3oodhwacv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pqylfbbx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nxzoxoox.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vcbptfjd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxwrtrbr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kkheqwhi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zffsgetv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ugkszpvn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3brgixoyz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3erekuzog.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xncnkenj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mltdrefn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ctqvrbiu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kdnegcms.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3zgcckjdq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3kjiymogp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jcuhqzmv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rgbwrxgv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zpicjhfx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oavhatfi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nuwsmtct.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3syzqroqf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pyydlzci.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3arlrdlzk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhgiendj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lhewopvr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gxwqlxbj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vebuvxni.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mbgxbiob.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vkrkoqbf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3reqlnupz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kzmvjzxb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jugebjan.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kybzbuui.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ocnpfbqv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uusxkjbm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ugcliwmt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lwqymgye.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ukijpmbv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mmainmmp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vfhhldjy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gcxtuhbw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hwzttqmr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ajkenrqf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ldiewtcq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3urqzgxix.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ssufsxpt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kvfyawrn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nuzhmqlv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fsghfzlp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3aultkvrs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qmkbdxoy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rxkztapl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ombepouk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nvprxbrs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wrxiagjx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dfkxookd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cxzngvnd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xofgqbdd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lduvjlpo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sncpowxr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ydobtalt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3eiieqsyh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3woozdwjd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tmhkqsxg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qyzybeen.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3foxbodvm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3oodgscyf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mvvkukwn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dfxhhbtv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wyhuuamw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qdvogeqa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ylewupzt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vrswqnoy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hclsjfws.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3naqrrunq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ubbzrthp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ktbevajl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oibwtajn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3frmbezyf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tovriekt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3igmnqlux.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cljncitz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ewgbtvtu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zhomgwyw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3fywfkqkg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qpgkvrhy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jhtoeycm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jyzynidr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3goyhelwk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zayjkjod.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rddvwyet.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gfyplcyj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rdpzqeht.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3smpfidgw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3znlggtpq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bizdfypo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3owpsbngr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jfgottvy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3imdgfhxo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qzpeqdlp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yotpnsrw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bckyptxn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3shtyqzuj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3oqvwbtcg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3drngetdi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3myosckyo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ntyhvupv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zkpoxrfo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ykelchli.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3svyzlddy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ciigwfou.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3espoqcmb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xjnkllyu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3irtokrxq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3optbhpnm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3htavyhcz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hyfptchf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hotcogjj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cxylfcrg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ibbdewdj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xttkkwee.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzfarwuc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ekmebhhb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gzfvzscf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xgcefxdf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3thcieuql.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ofycynzf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3edrckesz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hmkpijij.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gziqqkvv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mrimonie.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gmwoislc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ehjzehxr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3yzlvflzi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jlvrkihf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ptkptwzi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yuhknmsm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wmuadmdq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3sibcmfzk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gsqdnqlj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fhfwdnoq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mtxmwirj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eiobfeeh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zvewzaoa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnseshhj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mhekpast.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3midgrabx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ppzgilte.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzefwjla.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3imhhvvvb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hrvxtbzm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3smwdxfoj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lzbssata.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tauysugp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gruzgxor.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3pslcdahb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tvzhtlsq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sqaaicob.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3upidyvwg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbphnqwe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3poehlsfa.html


<!-- 参考信息 -->