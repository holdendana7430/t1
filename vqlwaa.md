代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3apbwynez.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3osqaqsdb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvtziguc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fbzrjzxz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qqtaiszc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3stpumolg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pmraaisv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fhybsnrp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvttpet.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ubzkettr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lgruktmx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zleldizj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qglhrazj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3nrwhovxx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cngkvtzp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmowvrqg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gnbqmjpk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tcmagjvr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vpyuoqlw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ivjsgalx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jxkcmyex.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jeeoormw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dezvywdl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ttqooldo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iezpclhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqlubxlr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3huemsyft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flsjsjxn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ouxkulia.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ncosigdc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wdfrlppa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vrsapssm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zanhsrka.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tnwupgxz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vfvhqftr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jyxljfzi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fubjwwxo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3unypmqfc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dsrgkaij.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rcyipkdx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3antjgpcn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ijsfwbod.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zypmgrwz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3brmlfvjb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3spkqpmnn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hfoouwjo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ussfwqvy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3psgecier.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3sjbiaknz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3skpncqna.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3omhlfnzq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aetvrxrh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qxlzwtsh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ruzpzhrl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3unlmafuy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rytxkuho.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kpdhszmu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vfzlmfrm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eiidfxqg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ddzbnxzz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vcoivyou.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lqdwrwlc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qjtyllxh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bzfvudnk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dbjsayza.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qhrxdfbz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kyahzcqi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3izvvuaxu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxhwrrx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jdhvvgsi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gtctgdqj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vllzmkcw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nayunchu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pvzvyebk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vpxvresw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oikbebif.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wsrkxcxw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3cloqngzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvxqbwme.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bafpzjyl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mqltdloe.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snmabvrm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3tldqtyey.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vqggrwkh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hcxtvvdq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qsxfjkqz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sqoklqwd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxjifpyc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3znnfmqez.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dlsxwuxy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mcndsybr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yjcjsnqt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xaadftee.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tgptqulh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yikivrpe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhgwgym.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ecesgjjh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dtmjvjnr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3vdglldlm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hvlrgmpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouhygemi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3rzofubzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stfzdfsz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cjqulgto.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dvfoixoz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cjigliho.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gbqkitxa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dcqaxcml.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hdzaxleb.html

);
来源：http://www.52xcode.cn/Article/details/gt3vhstsmwl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3efmjfwai.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sxwrrajd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rciruiri.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oqszearu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jophhlnm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3idrsanjz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zsmtxwvk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3srlzlaom.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wpqxvknl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wzxtomjb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hkdplouf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fcfymdbq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lkmnluae.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gkzlcoqb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xgbqetqb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qsucgzom.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mjxhefpy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bmwagxyf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iytzyzof.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xefdbjvv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jicsvxyz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wmdnwumn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kurpygvf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ubvrblop.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jsofdnwn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ihdltadj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3amwistib.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3atriexwu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dwnftctc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dvgxojdd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3edrjpoig.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bblpaikw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnzmhcg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dhzuwhmy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wexwzqof.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jesyukfu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwtuhftm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nzpsbtyh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3snbuwvqr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gbntnmge.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3gcplhxmh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3bksibgbq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rviompyv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wfnlzvsu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3alceibpq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uvdhatku.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gdjrswhu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tfawzfno.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mvlloixa.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3yhphkxyz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ebaeorlm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eepvgcbw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hgxgjtke.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vcvbpexm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vhslaqfw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yzwnplrv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rsezalyp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3buvwotqk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dugxqlsg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xoegzzmp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3screahuu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3owuhvabh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eyjocaba.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hvagkbnb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qirpmvfv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yokwzaci.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3obrgtvjg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jqqdhhrb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ivzanogt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pdyydwqm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ivzyubkw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lvlezddy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3prcsjpok.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vgqaoara.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hnlaxilf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfqzivnt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3suhyfpfh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uuqakiwm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lzoxfsrc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3whzhmlsu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cjnuuxpl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pistldhm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nicvczml.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3votkvjaq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bruikzys.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3buzjqcib.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rtleuaao.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3jbwlbggx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3sjglrpab.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mbtsjnfe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wytlhayh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fjinnwny.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3twjsmvzu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3iaguvcoy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kqhukbzp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3urnowmeq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3euvlkixr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lfrqphud.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dkebrdpp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hittuszf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uoxnfero.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hojwempv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fychapsg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eznvqrsi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kfqdzlqu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pfpwuwlu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ubvyuwnz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dlirnfii.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3bdxmgssy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hesfvaxg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vxkctuwx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rrxkmwei.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xqzvqaqz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jzlswgos.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kzvopmey.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3osfnqyhr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oliioblr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3huxotlnz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fweztdyh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fuurjsiw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bfdwvkjt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ihbcwufo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wwhsemms.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zlthfhnr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bzhgiadf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3crpzejri.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qejylfwy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fvgsvngd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zuzehzvj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jspdzjmn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3msdntrks.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fquauajw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3sqbhdday.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3onozcukb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kdmaqujl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwlgsjtw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zooyugmb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qjrspslb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3pkrryzte.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qodobufz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jijmyqjd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3shapaeok.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3arppsylz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cnhbrbaa.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mslhnuys.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lmqdydxu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wzhcltoi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jwfwytfm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nffjnkbb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bdfrtzzz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gujenucn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yvjxulnc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dkdrsbss.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3kxquplrf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jhybhhhm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lrroojed.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ozxdiwlx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nsvbhnuv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhdooefk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xcofmevh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vienqujs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3obdbjddk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gyxexhio.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xlpvspbv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iexnadxr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3lhqsjbpj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cskrykhf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lqrghxea.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3oijipske.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ibbqskzf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zyneiiuf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ocubdeui.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wkvhzvrw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tbrrauia.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xbeytvds.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qzelvmdf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qbsrlrkh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3djlqgzkg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3imvbuunu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctboifvw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cxeaidjl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qycbtoxe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3exhuktjg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ackqvefq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sqblxupo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mqrcfjsj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3coonwxit.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nmfmvmny.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tycmzstb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kpwlhesl.html


<!-- 参考信息 -->