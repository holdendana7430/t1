代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nvgtqspa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rngecvsi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3krfbtogg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3unjbojlv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3emoezgth.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3tlxdjfog.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3euzfsqgq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mzdeixby.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uqvwkrvc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wunkuckf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3myjueapt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nyqztpwc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qoogtywx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qradodis.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3upqcpjnf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ofcatdxw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dhgkaofw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3knsoagiq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3lcsgflph.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jpauvhjh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3coxufkod.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3hedcrzmb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fjhbtzqu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uzypkeod.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ntbolqbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnpjnwqo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mjlejuik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewbellmx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xwsgfknf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lgzylmmk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gieaaocw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vaiibxov.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3blwbejad.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zvclecxb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bxhradqe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dbjpryjw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3huxhbpsw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hthumnhq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kkkxowdd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ogsbazug.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3blcydptb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wwjaxghc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gkifjcgm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3nzltgfrx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rzvfkemy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pkobleeq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ownpgara.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yrdkvcgc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wibjxjsr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xdihweww.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nznnvzyr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ksilmhik.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wzelkwti.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3szmrftyq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3sfnwwxtc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pwujhxvq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3krtppqdj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nykoulft.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qzqlqwpe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3aydyugnj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nrkmkzza.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hcclcnjp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3korlouad.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nlzsklts.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wdxbfhnf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yuffprys.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3hzltbtgc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cwmeyeaw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dvgingys.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mtisetbb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yuqxdsck.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lncbufdx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3zqmppqah.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mantcrgk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kwayayaw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvetsihp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zjxjepjw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddfwucok.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjurrhab.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zmnjmbtw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bjwxsxah.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jwmgpmaj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3faliieqz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tobvzrrq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ynrxpvat.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ljbtlkyy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dlikzjnm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3znygnwxt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jtkacojl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qlkmzwjs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cqxadfwf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ozaisiqy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ajcqdelk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ovinaifl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tagxqheh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmkivznx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hreitwui.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tluwrxby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3quqxfwls.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xwhqcxcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opkesgtd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3bxgfxivm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnoitree.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vjurqdlm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ddnuvutv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ppgjmrwt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kcgoipsn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cfeexvyn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3cbkfsclx.html

);
来源：http://www.52xcode.cn/Article/details/gt3faipgoty.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wvkutugk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3bygogcie.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cgczirfd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sxybagbd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cthcdvkx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3graumace.html

);
来源：http://www.52xcode.cn/Article/details/gt3wnfnnjdg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ewngwxul.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gxefnzrg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tgzsqmpz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3stttsaza.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vzdemfbs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3danynvpa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tsljhnqy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3sjiwqwmh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cgfcllle.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3speljaxv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zrwkwruh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xilyinfa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rreccura.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3podjoori.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nhpwbrgv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3buewxmoy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qgkvhdgx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bwoyjusm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3goxfxpek.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hewncuiw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ujhhteye.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ntdvlfty.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eugzqlgb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3abhpfcgd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cbecetne.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cgokmcqe.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ldywdqig.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3evohkdmo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hfaadckh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvoaszns.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fqssxnte.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fngwcvpo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vxzdblti.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3aouufmcx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3joulccrk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hjkdxhcn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eqilexma.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xgkauule.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3txnrvkdf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qwigrpfw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3poaoioqa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lnrqhxcg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xxyskmgg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ncgwxhxe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3melvftqu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sqfihazp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bcjyphdt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vrkqllbe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vinlwayd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gaeodosw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qmelcgvx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cbzkzvaa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zfkmikkh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rxthxlam.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nbgratgk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbdowxsk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ghtxcbzu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kehjucyv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zvbmzjvf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cphlynwk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npjlihij.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uskblsyf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dknoudiy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmcjedro.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cyalzcef.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tyyscooa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fonusuec.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bwkfsoql.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twpmpyog.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jrdmsnlx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uavbrghz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tejziuhd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bjyzfnnt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jahunzmh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dufcnxjt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tkezncte.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fyknkbsk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qgzypjpr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3tjjhxfyx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3psssxkyg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gbpwuhpo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3jerpnfnd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3yuofunfb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pdjihgnt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3oigeytmy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3noklvyjb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mgafbxxz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dyfgopky.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3krdqegzk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dttqglnf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3cwjjvohz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hhcidifr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3uihqatgx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ffniwqji.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zmskurkz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ealzgrbl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jyqgsrgk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jafyahwf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tlnouhri.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ijwmgyuj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrgvgop.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wxpjincb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3tqbjtltj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xjgvyuen.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3uaznsjxz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uzigwnpu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3omygbubh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjhqleac.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nqpgpefy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gobwnaho.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nmamfiyj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lyalojwv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3pcdolnsq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vcpmdtis.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dhlabpor.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sycrzmua.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wmluuhto.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jetqakqw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yxmzdhug.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3exscyinr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cxoemmgk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ewgzbogc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3acunlqhx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zvhcoqkh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zsgsmcmu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vkoacghq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eiemzptn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qvzfqfdl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bwzgyjrx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zlhriorn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3epjrfnfi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xdwtsfdj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mefcdroc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gssqoqtm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zhvdawft.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3lxqkdjnx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bfiocqjc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jzkejyye.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nwbdsnpv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3idvyqvdp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3osgmvtat.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fvodhvxl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hgnqhqtf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tzjzpaue.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jxaijscw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3mkbzfzrh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zlaxnmwb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fllynzhn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wwqdeyqe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fbuhkymr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3yjxukeir.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfkliyzk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oggtkdkd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dsbggdhn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3paunhnny.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3stlfsxfa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zfctkepr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uueukews.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bmkjglis.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ucwapqrv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3shktaeti.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vjnfsswh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jnlvtmxi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3tjfosoce.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mvxqcwdg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3quswhsne.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tpqxsebw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iageluqi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zxtbnfnh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gcaxpuct.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rzxwjrci.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3igrtigmp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qmgyuowv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gzufiubv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrseseip.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gwveqcud.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ixokvkzg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pvxfrrxq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jjjkudlq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ltqenokb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3macojywk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hohrlvfn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ucgibgwn.html


<!-- 参考信息 -->