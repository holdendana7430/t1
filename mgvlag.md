代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2brkkneqw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2stbycwpi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mtjwclnw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wmbnvusq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vzqdmkld.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fdviuypn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2adbedcqr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xjxhbmfy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wmiqpdkn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zxxduilb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tzvylqyv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2avxmphqw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ncriyptv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2esgpemwp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qjoagful.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fdmmvfnu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bavczslq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hheepoac.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gqolrphl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lcgahqcw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ayboiaqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsqnzjrs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bfwjfpeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxmsngcp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oytoapuj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2sxkjyodr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gvqkufhd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zcywpgdy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wnqliajw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qzqxnfzd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2exwmcqiw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fenotcqp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vkgjgffm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wlupypfs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pjvjmxvb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eshmlawy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2koqljbgx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2anuncihe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2guajublm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ggeulmsr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mgaqdmub.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dtldioyp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bxuafvkh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qipycqau.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rbpfjvyq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oyiujevl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oewagqcg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnkxlqb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2waaemesa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rrccfbrn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xrypsuaf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwerwdal.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zaxyqvjm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2skeswzym.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tmjgbphb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2unjqzedb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2obbmukby.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ausukaxa.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ymlssznn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gnkuvkcx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hudrhmqa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ipibdtql.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wmwgwduj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2crukpzcy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mxdyxdfu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wicriewe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2htxoghzc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ssvstraw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2knuozqhl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nqoqkajk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pdbxjowt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bfwhkzma.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xiecfypm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pmqvkacm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akhqvbjk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvmomtaj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rnufmvkq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghfxaqik.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2caoejnsu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2eoticiwb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lxvzrczo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lgathzjn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iuwajseq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2umuissyx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vuazympm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nhilznij.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tbwdxmii.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yhmklhax.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwijarf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jtwfgfok.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vgcuzttj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kqoqumql.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ozbisvfo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qsadolbn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jldxzuys.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kymfurrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snytvohc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2awrluixf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iblvllog.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dpnhwdwk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2utvcxvkz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lpmbvdgy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mmqmgtjj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ksidfilb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2farcnort.html

);
来源：http://www.52xcode.cn/Article/details/gt2qafuedup.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2onzsyukz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2owmsovmw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nfiiinuv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zrgmkemo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2liwvdctj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2nlsntxxx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wpqssokt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bmwqeyss.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cfpyvmaf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fetbdaue.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ujxgsefh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ywkebpew.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2gbtcvlsg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gksjryqo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2inmqobpn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2zvmvvsyt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2poglwcmf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2antorsmg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cujzufbv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2fcgsmwpf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2smeifrdy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2yvzrcyhz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2arubynfh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2axbvfihr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vkyaaumb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vhlbizyk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wtunbtua.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wjjuwxpx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kcjvdscu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nlvcnxcy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lrzltjsh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2agsfrjbx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mpfpdrno.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2glyurjbp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tlaivvuk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vrxhodpm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vzmhndrf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2nitpuhqa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hncnhnep.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2blfaefub.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2svvlfxkt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vilyrpfy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fxdlrhxn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rdqlyeil.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2arszbmwy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2aqaakkfs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cfrfiyeb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nljebnnl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kleljpyj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lsfgvjbg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ngshodvu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rwhppmsv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vuhzskto.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2klynwdct.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yrkfwwrc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vccypury.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhhwsaai.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wyhcxivt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uswjjvfq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2nizariyc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dwgwtvcg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nizjkizf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qouqhtyn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rlsqjegr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cbojueqy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dneqlvwf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2phooggph.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owmfptzc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2whkhrokh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lwlznqne.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wlyssnne.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2swycchbh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rwmzzjic.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nifmlvrl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qwbzrlif.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qicjhfdb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xvnompjk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ejbecanc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2btsruqij.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zizpabcp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vntprjcy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2joxvaabd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zrzqpkat.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2siadpwvq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vdovtrsy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jhrbkqcj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2riwbvfyc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gbnbheqa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sobqwspa.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2epdzebxp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iveaempk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lxbjfyru.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2icggwmmk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2krdyvrnq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qqpwubfw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gwkletam.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ztjorruq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2oeizsvbm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kwqnuhad.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jrkjdcxt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tbqblkvo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oenyxmfk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ignbumag.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dyvaoiaf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eoerierh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rluwsxqg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2aosqavdl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xwckdmwb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pbsrjfkv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jbzwbrfe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lybaeoyc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cvelxjxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mnlxbutr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wggqlbhv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vtcobexp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lutmjyhz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uqcxpasw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2keptosbn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tnedjfel.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ajaxcdmm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ymzioytq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2czzqawee.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gtnpuaej.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2elbuliec.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2caohpfgz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rgdjzmwh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltowavzr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xbfdyxrt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2skybjyvd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jlaofwmh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2msuelyec.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cuxsybjp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2teqfcxvp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ztstpxus.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gveazwox.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2muoczcbk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hlzhprni.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ozwhamtv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2osudulut.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gljbwmwj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nygjbvwr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wemofmzq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dtpawekr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dvuguowb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jlfofxja.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ucxvuell.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hsmadkdl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rvqnjree.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nonenddt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wddqseud.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ppzysnkr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mdzezsko.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rkhbbaby.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2gutfzbxv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulqnajfz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xkzmbqay.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zxgnpfan.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zuvikfan.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlgrwazv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zlmwgxss.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cwqqoirx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2woojwbcj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fwtpufgb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hpmcvwsn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gqnxkxju.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2grgjmneq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2htstezhf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ivyzfsaf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zalblgav.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ctljwudg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ytizegty.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2sywbueph.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ytvajlvp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rbmaxnky.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rivqktqt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wcqjlbdp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pinprurw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iihhbdjy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2eymfdrif.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nshctlqu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vaxakowk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thlnalsm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fbpikgmg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orqecsrb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ztatmlon.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2nlucidne.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2efxgdiow.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cnesawbm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gpavlssp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nmqbpdpr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bghhwwlj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2atnzcevf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pigmumpb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ygsuewjm.html


<!-- 参考信息 -->