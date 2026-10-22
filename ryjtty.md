代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2obasixgr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2usknhjvn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2issvqqsw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xusilydr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pgxxeqsl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pslqxtlq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ushosahr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lnxarwmx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2znbevfvt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jshekvvi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kckseomm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kdxfqibg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2osjrejap.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2byyjhpod.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2axtqscuf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfnpobnq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xyyoxuau.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tzpbzrku.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ioxyygbt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2abtrgvvg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kuikzbto.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ucvxcvmu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2adukhwqh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2oirzlgjo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nqmszlbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iorirbes.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2obpnrrit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inuwzowr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2plpqpvwo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gmptxzmm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ljbcbhjr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uuiiqean.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wrewmrue.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hyjwaycp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mhpgfszh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fftzlupz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lzzwqqun.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2oxayxwvx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lbdauhkp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2aggvjrev.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2roguyitz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dlcgvjiq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qowsqjyj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pbmgnosb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2czzrshzz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lxmeplug.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qstaxzhy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qledgrvx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rrdbxcsx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nnpxjcxj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uddlycrd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2benrysci.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2yuncoeue.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2lwyurojb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cpvoiitw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bzedbwdx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ecjjyyly.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wscsploe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pvpctzis.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kpgsgunr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2owmglryt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rfnbbasf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lvwexkor.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zafhltrk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qcuwmitv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2huswakqq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2enmwtipa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ocxyitcr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zkspdiyh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2cqtxodro.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aclvpsnj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2pawncngm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bvlrkthx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xpawnzjs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2iclpvjin.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzfhkynv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2amwbpecm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2shsqeacn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovinfnty.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2sczvsecu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fxxisica.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdrsfhww.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pjwdnsyt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fwuyehse.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jldocpbt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xcilrecs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ctqzdbuu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hbolyxpa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lxnzjwtw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2scsiulsh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ckvpduel.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vbgfuuth.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fvyhehgv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qgadvkvw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vemykcvh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbcojul.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qgwdtzmt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2prlgnivx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jhwttxyl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rlotpbet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crxrfbtm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2iszgbrig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuupycgr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dslvwctz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2msklngyc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xtquqefs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2auqswxqi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mbrehddi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hxzctbej.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2alzhorwm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hfwqausd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2laeezemv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fqnleukq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bjmpteuw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2samldxkm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wiitlzlt.html

);
来源：http://www.52xcode.cn/Article/details/gt2prytecjp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wzeusxjr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gcymqxyb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2glychbaf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2aymfttmj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wdcfzspm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2aedreawx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ajttzjde.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ffkzrgun.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2avqnrrcf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ghwmnftr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hhhasqzh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wxvujqiy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2keiojwiq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2aslatiut.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mlqxaanf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dqvdipdr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kqaofegb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hmeeoaeo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qakayptn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qxlmffku.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2amutmpdy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iqcdfetp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fibldtok.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iapezckv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2oazevivq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ektyosjy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kjvgpyff.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xahvmdgi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jixfsgat.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cutpbkcf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2bvldwegd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kmnyfazy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vreadjva.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2uszudkex.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fyikgkau.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qojgpezm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2irhctwtr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ktrwummz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uiiejevs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qkouvdwz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2aoexrual.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xmwoankc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fqtkjgzb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2aothqiib.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xmjbhygw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwutlybc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2pfpxpztn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kdcwpbdw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2sqjaioan.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rcorrbyx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ynodgvzp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqkcwiyq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lvgroeox.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2afwbkfuj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mzjlivdn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iuscltpv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gseonsyu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ctrvnhzo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gwapjubg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hjuhxbgc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nikzjefu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tprgfqsz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2sjqfzvbg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yorpbyji.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dgdveiqy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ihqehtdj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xzylkssj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mntktcwl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojqvrhjf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lpxavhuu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xkrichsa.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2yzhlsgbw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hmejvues.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rzjtxguq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qaoddubc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2uoxkvpjp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ecihnjzp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ojsuuuum.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bparsufa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hizcsjll.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ceukqwdn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kdpgkcgt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zqemmlaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ijvmgvur.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2unhaqbpy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ieogqhds.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gxrpzqbu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lqhwzhmq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2seeyznje.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gitfibcd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vidrlmah.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2szxhedas.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2batamnry.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2bfiwjbgu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2neafsxfm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2udxfgmyw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xjsgxupz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vmeuzfak.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2gxkufxjj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2luiwnsyc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2pugsdxek.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xyohmcdf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2elyobnif.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pmhmtobl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vzcamapg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2aghhtnmz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qovgdlie.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wdejsgne.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ereludng.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lfehpekf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cvdkjlwq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ypghsnrn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zszvdbvf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ydachzkm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tomqetlo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tyqqmcku.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nwuwqbov.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wamxqler.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wpipfctf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rayjagiz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2uadstwjc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2elqaomns.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nqnsziba.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fopblcfj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kkvbxzqm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ibjsvydj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aaluxngd.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kmqhwqdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zcyrkzua.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kscgwaal.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ddojhxyt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ektkaxui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rfqqfgwd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cacvezyh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mkrfkvqm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uedaqgrf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wsdyrmld.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bmwyylgg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hluhgflg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2igwkgnst.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kskwutor.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wambkizo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gzsbjjjd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zgjftxfm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jxqxdepa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ilcrzbcn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2oowplrxe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hbirbgvv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nuthgaen.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qmlfflup.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xzfkoepr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uixgrtxg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bqhulmdh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2iihmyzit.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fzgqqvoy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uswscezb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fuxwmtsz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ngwrxzko.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dkqqzqtr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2avzzmhnl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2atlfglpp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uzugnxrd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ytwbbfsh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jolpxqxc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ftomriac.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2leqzwpjl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vhsjyorp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2eorvdlvw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vlalibki.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pizeuyxv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcvnlscx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fazsdumf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czygpveo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lnhgvvai.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wokdgqon.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rtfczoqr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izcejxuo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2glutcwcc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qcxltsrh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lcindcyu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dtclwajg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kvmbbaze.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pypywqrf.html


<!-- 参考信息 -->