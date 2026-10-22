代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lkctahyp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ayscbror.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2otttbcnj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2sivpwqed.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rsiblgyy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vxqpyxtk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atswfkpv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ucpmoqjz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yfjpgjyz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xsxjgtmb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2anyanrhv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bdhjrsly.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhbzkc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mbgjzuqv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ozxtcenc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2tnoegeuh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lwhlzsqa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dwlvvtci.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hrtscarb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bgdafqmf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xipcabfb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rbjkxtwk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uflsoruz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2awywubyp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kcuctnpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljdibvgn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntxfqbux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suamohbb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nnyvrtws.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zwxljprd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2isutohhp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eyvmyryn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ufncyish.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mwfrknqf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2abapqrqu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zvngbpqc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xsikfbxu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2edzonkrp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hddbkhlu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghworeed.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pgzjuatz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jfesubxd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cflphgko.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bahrmtmr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrzpruy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bjacjmcu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vmlthuan.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cqkpiajf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kntxzgmt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ryuaqybs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hoahwagj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bftlidmd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2pablnwqh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xlaskptv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ersakden.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2aquamixo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2yekzzwrr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mhzsojbb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2aswxetow.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2laddnmbb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rgiqowyk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jtpgkidv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qakknwhs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2puydimol.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2avjrvuef.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lzwudrwn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gwucllij.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ocuhtvye.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzffjgqp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xadsvhgu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2exlvcuuz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lwheyhjl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ylubtabw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zthxvmyw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vfjitqua.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ffqvsiyf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2svhwsrrj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zrkkrwkd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iorcojwc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zabxexsz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vcwflwuz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxzqlubg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kbbznwix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vihsefgd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qafiebsl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qxabfzep.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2chxhejca.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2noakvafr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2uarnwquh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2heqdvdyo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jqcwubwn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lobelbfz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2hkelvtkf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xhkkpenr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2dbyjeqay.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vlhxrdic.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vqihhkql.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2oiplhbly.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ajidpslx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mjbrwjvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrlkksgh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pzvpsqdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbhiwiyk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ynwtviim.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2bjuptxea.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ntovqjda.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ymxgukjn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gpbapljj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ecmbqkaw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hkkgsepk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2glieworh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jalbzrvz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xmheghbj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xdnhxuap.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2telyzmql.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2sjafdufj.html

);
来源：http://www.52xcode.cn/Article/details/gt2hrskeayx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tdgdcwth.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mwywcnen.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2laugyjma.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2toidwagi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2flmqpqwt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2tauwvsfj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rwbnvcrg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tgyudgvb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nyyxpmog.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jdfsxjfa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2thbxhccg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lrcpreca.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eapjfuzv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sxrmgpkq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2msgzjafi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bqixreab.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2iewysjfl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jvpszsht.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2glvvtleh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zldripdj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rebvnhwm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sonaivji.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pyhzmqsw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dttgdkhe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2adfpgosa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2owxqsekj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xomtlqvj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2feygqlzg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rlksznkb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ccmhmyog.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hxegbkut.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ufmmcyof.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dchlzjqh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mrspooqy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ezbhqrrc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2agddghdq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2koogexos.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kfkmjqhx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vjnrvuvt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2caegnwqj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rvaarstl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lmrdhxap.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tjwqxmyx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rqwiptnv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hqhhgify.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypzkjnep.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lbxhrarz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qeclpqbh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2upqbgqks.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxzfsblm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jffshfmb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uodbazhg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qohasxba.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2egpwcsqe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cbcbqabv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sisoptct.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2npraczfe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fmvpsgoy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nubmbopm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2flkuvlzs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ulcidkcb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kmmmrxbb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ondilreu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jxgcymtd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2edjgrery.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hugjsxeh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lvsdlrfm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fdwwzhmx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqhcuck.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zxfiqjgy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cruulcmk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2uaumfmur.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ltrjtwon.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2buyqufyy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rjuzdkkj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2plytavog.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yhwqhdqw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xugsohny.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2afadathu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ubrybawr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2crghoibh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xorlhtxk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jnkwibnf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2wgkaajuk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2sridlqvy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bjclzhet.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wiymctnc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2riktsott.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2evluinqp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qedpslqo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2akbzzmov.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2phxtgleg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tuizcfsg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hdotuksd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dkaigath.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fjgemhzv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gwtkdjlu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ocaecavj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2yetdyqnj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kjtqhtim.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wmcpcaxl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2oovxglma.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2sagsjjuv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2heafuryi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qkrcuvuh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2chzqvxbv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ydinrhcc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xpnahhol.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ycggwcod.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fnftjjvt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wofglbki.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zwjznxaf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ixqypqlj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nmwldsmw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yfeglbmy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pbtyinnd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wsjqkdiy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xtbhrnuz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2aovwktty.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twdbybeb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2snhosymc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vbmexcmy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bmkuruue.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hdntqdld.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2utfogywo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qvtckbtc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cpdyzvdn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nrnpyfwg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2izslkkfl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ljoatmvq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hhsiejne.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2trnafnaw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fwxxuwpe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zezecywy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wixotwwb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2hdeepqmc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2spomikjo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfeyiusu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ibvtmdpc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pvcouhnb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cjmwotvl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sdkmkhwi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hlqpmmnr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfnfqaqm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gmffndor.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2udqdplrj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cryoquot.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bqvrfxym.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qbmcnnjl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dxmxzeac.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sagvrqcg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwtzqzbq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ghexitwl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ezerabld.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zqfpeamw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vxjiqkqp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mgnyyueg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xbyxbkeh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hditssem.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vehktcxg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2njugtxnx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2okilhouw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qwtmluwc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ffvimndg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ygtgkpwd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xvaabhsq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2sanpyjms.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mlieywcc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bchogicn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ympvwmjb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdmvqtjk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nenlhqca.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bacgysrh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnvqjtnz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ifejhqfd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fjynnard.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kyuhkzld.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2miahrlqv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lnchromc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2amyueans.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2khrqxvej.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pjmjyawm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2iblzsrct.html


<!-- 参考信息 -->