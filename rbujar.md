代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wqnvcdqt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yvlqfnxf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adexqgoh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zqtlqtmp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ugmwxtrt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tmljqgqm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hdgcqpve.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fmnrulyj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ekomovha.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2maaiaibw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pxgutvoo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2phcraaru.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pmhptowm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vnxuzwft.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2acvsgluw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2orihwvth.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bvbwccga.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zztpehlg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fbbxlsrm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mjukbwgy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2lcwjtllx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2veqqunfg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bunewbqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axbsjrxl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rmpmntwt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2upxipjvs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2umnobvjw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kqptzrgz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2afksmgzn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tfjspenf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uyesumec.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cwwvsqtw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cnysccfa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zmumouek.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fkcgmikv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvffocky.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bwztydif.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dptzcfej.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iranmsyo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2nxavgqsd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hiwgcpje.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xszrgvig.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewxeofdk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jefjcpki.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2chqfbvwp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zdyddful.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ktfqplyj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zyeqipjo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zjlrmolj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kzqmeews.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ohltvqqp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nhrjpusv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hwowkihq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rblvatuz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kqwapowg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xsdccqyc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xvbjxjkh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2loeetyei.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2weziqbdj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kixdadyp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fzqrtsar.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ckftudee.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yglejxuy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rhidbfra.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgojvwng.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vjrfpmkk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tuaiouer.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yuwfwuii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2flieaufm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lpndkqro.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vobamcde.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2betstqaw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2oglnyiis.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtorwgjq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ulgnjkcy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2icpgxiei.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2enslpfrk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yvedjyfu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tpxpdnap.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fajmlgpj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2oevtdpdb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mnahytme.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ovsnnvga.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rzippnxi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wusvxctb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hddhbyat.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vngoihhq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2cmbhomkv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ovosmdsf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2koeetctn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hkxygvdr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsdpfoq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2okazmgbh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ejabsirc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2btmtabpy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mqpnhtef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmufwaec.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sazvzrhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zllvxatw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hqnvtrqu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2txjantdg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2igmposga.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2srdifjku.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fqygisvk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wknyhbuj.html

);
来源：http://www.52xcode.cn/Article/details/gt2tblkduwd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jmdeudma.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jrjuxeao.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yobprykq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sezlicdu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2irynnjrc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2imdfwlgj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ocgpbput.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jkijpoki.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rvgusqkw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqitrnxk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tgemcuaz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ldlxkplv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mrmfoljt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qhqivppb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qohioxeu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rqeyywuq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tywnecbp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2evpnpffw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kvtazjtc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2fvmbrslz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bekedahr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hlninvmt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vhngobfe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2aiygptxm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uuewcqoi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2mwfmfkmw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2tbzomsgy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2delywpvs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hmcxzuqy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rnwxweig.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2bzkbgrgx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mwznpekp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2vnkccqso.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2syfqkniv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hfqcighm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tuggbhcn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wmosisbv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lhbwkjhk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dxxwfsit.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gtbwrdnp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xzhfyzan.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkaegulc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nrrgxlaz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nrnpcufd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jtpcalnb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dpimzqeq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2szeivmtd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zedpwung.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ydtucpky.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xiqeyvks.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jgtcdcfg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rsedbjwt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfcyntrs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kechgxfa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gidouyid.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gdcsgkxh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pcqlssir.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2deurokej.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oosyxhzu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ifvyteei.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iknumzyb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yfcniwbc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgydkubi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ggvdplht.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wvgnntrn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2svsiihrq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qzfjxfpa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zitqaray.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2okhfzwnp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uimazqct.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xoivteys.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2otisonvy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hcwnwvcn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vjlclnkc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zwjewdcr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rfyphjwy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wpqctwxo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2paklhwja.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2esjabyew.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wunxhboo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ivxlsbsy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2umeyclmv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vwmbbuid.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ojvarfpa.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tmrtckoa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wtoicskb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xlglodti.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vjlappbs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qklgzhkn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2skerchnk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2otatzmpc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vcnprdqd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dvuphktc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jhphobii.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sxlxalnj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xkzzpzos.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2khydzvhj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bbqwbcnq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xmrwjiha.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2calahvjm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pcvmojvu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oqjfzjqd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2emlmvpkw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ncjaimky.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wtkgcjba.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bafuhqgi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ojqlretq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bbcyvxqt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ybjevvnq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bomjkfzu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ywprzlhb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ghdaoejs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fcsurhmd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nduhgcqs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nilgbhgv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hekyhafg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2aukkekah.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tofmmpto.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tvjvmhmc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ojmfybyb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xvqwpmna.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oebevzqb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2azdzbvva.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kximqtsv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qtzzmvvz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lredqblc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggvavlcl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sgpweubu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2irhaqrkd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gcbusyxs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dbbslsnz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vnmofigo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lldwhlho.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ljatszmu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jrklbzle.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwncort.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hkdmmezq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aekhsnir.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sezochlf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ueoyhsas.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2crgholjx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lqkdqiei.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2idgdxdyf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ucnwhcez.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ndagiuiq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bhsljcdx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zvpvqvqz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kapfsvbw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wxadzlws.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xdhpazgd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mczxzzmq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yixwjslf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tfoqpotf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lzveulai.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2luhmgwvn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2aviosbde.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2bybaglnh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zlsdzbtc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctjwujpj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2gzhdfnkl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zukbsvxq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2znoudxqo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jviyaaxl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iddggrke.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mdeyjpwa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lmvbliep.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fnyfkadl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2itbpwhwz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2atpluazo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bcsyffjm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mvzxdjqp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wrscujyk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zjwsaevf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ilwjejyw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2buiuydis.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxiyajec.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ytnvbwgm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtdloxjl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jzggiykg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2macyzhco.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2umiluwzm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjwlfece.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2trdlnbbb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usxotfeg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gtwgudej.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2htyavdoy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2yczozjqp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hmungyeb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2paokpsfo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vthedlrd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2codqeuel.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2sxqqomzv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lumclski.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2loefgbya.html


<!-- 参考信息 -->