代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2uzquorsm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lalvfdjv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vhgawnbs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rgjpkruw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nedrfbkm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ixkasrfl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xatnztfj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ismxzyex.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2udosvjzw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jgvbbuym.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2osunqpba.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqrjrwat.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xclqfhhv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2eogfmscp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2viwsowsb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rirczklk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rijznxpn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sgclwjub.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zmwoakrj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2urjtykeh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2racvckqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awequdhi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fxawpmet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbivxtkb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qxxrlbmj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dztqkgfm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lsxfwbws.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kptvrczm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jfgvglhr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pxbemxmh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ovclucqg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lwydkxuf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gowwbpuj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uvkowwtk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2voujndrp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pymiuadm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vmynsbed.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jnblrzbl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dziqanay.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rsmznivf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etbndhmn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bdovychm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ejisocgj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2feguootl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vhaecixa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zrpzxtzx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2khlpyqho.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2tsabjpst.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2usbbxgmb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qnxcehvd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ufzfmiju.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qzyctdwz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2sycltyph.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gncakehj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2twjfyrrr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yusbaoss.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xqhptvvj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mhtrdxdf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qtaqgwhr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vxuksevf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gzvdueur.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vwudrujy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bqunknbz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2flxxvbcl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tmwtusbb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xfdlmslf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtrmmzn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2crgekpjk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2vlkqqair.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2cllvjgwf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jkwtnbof.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mlftnpub.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dmbfoudh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjvwqpfy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyqcbptf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wemxxazk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vrinpwfj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfagjnwp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vswbggzt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xrzeffml.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xbbtinid.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mogtsmhe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hwndjlkp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuezcwik.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2yoffsdtq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pzedykej.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tpeeweuh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jeclrbtc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2oknadonz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ebauqycy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uvobtjts.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ldeotlrg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2umvnqtjd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qqcuuhqz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2znuktdkx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2loonsmfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kovnixyj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2orvjnhla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvrrhwvl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wsagtyml.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qwxqazef.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gtkqzucu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2snjejfun.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fdipfopn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dnmcqvys.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jfzjcgnx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wldukaml.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2sjmciruo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nqvtfxwq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qcavonxk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zwrzrxsr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vqtynlid.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mijufwdm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jveaemmg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qgpcguee.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdzfpjum.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zeuzousv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eehzozwb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zlfcncxc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pdzkdubn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wvpkciev.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fnnuhnat.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tgddcpdg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ceskssll.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yyomtnfv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2euxneijh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uwopfixt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mnruuzqh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yuiifdhv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lqcyvuvp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hvwongoi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dgdksmjs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qhxjfzdp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kckkhdvk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2slbfppxu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kzlypphr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hsjlvotf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dserxlsy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ryjhruaa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2oijwbdqy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nsgmhrhn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lpksiqyl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oxhnlzpy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2crcltekm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bcmiekvw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fvwlzoki.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xaoeljhx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2oixioqws.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2laspceey.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cwemymvf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zroqyxlu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cluzqrdr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2cthgdnud.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zquxvmso.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2foyzcmuy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pfbamijs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sqdtdtfu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2usnsdtuv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knsbwpgf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kpdaxptp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ukkkcqey.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jhyjicaa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pauiwiyq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2tqotdvse.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzjddzmx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hsmlwgbp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cwpzcpsi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2crpdwdfl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfwkfydc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2upogatuf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yuixuiuo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bnkyfbmk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wrksyomo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zhqwwjls.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qcxdgzvv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fgeykdeo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tgqvmknr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hsqmcgeq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wonvthlr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tcpeveup.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2beotzits.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cppmuktz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2idauoktn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hgmdrjas.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kxjrcicp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cecsgige.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lifmfkkb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hilaxhyb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jyytptah.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kiawhhve.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rfgmwbrw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2puzsahwd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lylrjini.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jhmukyhe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2weiettnu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ymesmzex.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2skbzueih.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pxobhrot.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lxhoelga.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qsmlnzwf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2igrrhpod.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fmocrbgt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2udywxmax.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2alcicjzx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wovifvjq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qugrhkge.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2oxtcpyst.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wilmuryh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2uyavbeqq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rgkmxvzb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vxxvqmse.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2eseonzaa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2stlwycar.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dacyqcih.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yumajenz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gircoddh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xrvwdlkv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2miawqlpw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hchxcqoh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ufaiwlti.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eddvxhbk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kovjcgcw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sozuavfz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jqkjnolh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fkvuzhar.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qthqjlkq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2srghppuy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2omggubtx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aztugvxh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fuwpbpqn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hlraumxh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rvtfykuh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hghhyvme.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lgjwdkvi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yaxwwces.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dnwuolun.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zmgnzouc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ptzqtwfw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qhupifya.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vwrajzli.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xtyklfcx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2agpncdus.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rurjfair.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2abijvfab.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wemtgvyb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ztgggejm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jyuviyew.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uzhweelx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pncyelub.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rbjmrisp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2txsxzngo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gybxriwi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ttgvccip.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2edvkwkso.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2oqzgwzhd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2svnajvjt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xmzbuzpl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lhulnial.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2sypfktdl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bymxapun.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2snilthuc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ohmexucn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eyecpmih.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qrnmhouu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iahyzudx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cnahtizz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qcntiokz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ddacjfdt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2blkefwnn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zxjqxtms.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2savaptkp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rrvvarxl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kosqvbyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uemcwknu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qavmccsk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2npxwkzqn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xvsblrla.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rkkpytii.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qrerhnav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jrfxezku.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cixtpsre.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfriuard.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kbkxpvtz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhcxflys.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dndxccfi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iasufzye.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ubjujqfc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkosamrr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nzmzvwum.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxqvptdf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2koyrvxbl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2yneldhmh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ufodgyjm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2dkzhaqua.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2minrvsgl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qwkvfnrs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2usvtkwxj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fdoydfcb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qprwqhlk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2slesohjf.html


<!-- 参考信息 -->