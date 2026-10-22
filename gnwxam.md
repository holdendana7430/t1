代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dzkzmsfe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2galfczrk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mpgvtxbx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2shmaxllq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uysbther.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gcxpmxuk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zjycbokc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wpojlkxr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ccpdziba.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gavqyawh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrqrdrwc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ogifuexf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ibjmkyre.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2pedjwhln.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wwzrbzdz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bohmufrw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2iicqqrws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndgvdaoz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2iahknkxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtoutnkz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xotyhxuv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vlgqaviz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2linjdbpy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2imqsiqtf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2atiscort.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hiujhljc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ngbltfio.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hgltztac.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bdueyukx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cbpwdctn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2axzkfbeh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2brmsxcfo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ytyxxmil.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bdiicdvh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2izmmyqtu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wymrtcvv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgxnowen.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ahqtmkpu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jgyiogxm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jkpzsuho.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2blulvxys.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fstyevaq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ytybtupo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2puewmsyj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jpagtrnh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2saifdgjq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2xjphbnqe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hpspquwe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tftvmbyk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cbmgggct.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wlynqzww.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fodlnjgm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ehipxexv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2feiyksbi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gelmguha.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kezigvfm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2umegybrw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zecnfhjp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wycttsqq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2eujetceo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2njyrzspn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rxvzuyix.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jddcklxn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ovvamffn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kqmlkmos.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zyabrjmh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wkehpwxw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kcsciext.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2yulziztt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ncmijjcf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oamyseuu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfssxpmy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jnjxrphv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkkwajdc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ymrbpxpp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dwiaqrsp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2umnfuiqv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bboiruxz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bmfouciz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmllubnp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lcrjoaie.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ahxrunbd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2sztjegjl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zpsoanae.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2rahujyfp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xywjgnux.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vkethkcj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aiosotvg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2oduoncrh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hnavksdq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bjjtdcix.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kyvdaxva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwgocgkx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gvlsjoah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2faasyoif.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bkvlyenz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2irwdhinm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ovavmmtu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qolckxvl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mvgzbpvg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cqaxlmwy.html

);
来源：http://www.52xcode.cn/Article/details/gt2pjfwicyi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fbfycmoa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dqftgjox.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jbcsmzao.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lshjgswg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bvdcpmpd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mfijblvx.html

);
来源：http://www.52xcode.cn/Article/details/gt2hjgbvhsq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ibopmuhd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gmyvlzfp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vtbaasbq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2epenlrkn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2psdhulfi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fdinbwmj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bndwbirh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ijwfzpik.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jvggdxuv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jyxsvvgg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yunrxplp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2madgtetw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2omsxzrov.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2elexsikj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2kzakcreg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tkfhxnuh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2irpzhsnh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2klqoebfz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2smjcgokj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gyqrjpmh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2awnrwkrp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2lwucqdlb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zdvpvvvn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2iidnsnna.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2prklyuhd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jeyrstwq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dxgpsofc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qppryfij.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qrwrydru.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltyqmhbt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ohskmxah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aeayrzxu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ohipisko.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qnltbkcj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ovwmqatj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fvpajams.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hqkvgkmz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwzugneo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2udyryzzo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2onjwotsh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pcxknaef.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2oazozqns.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vdymtegb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xvtmnafv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fyzepoef.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2csvrrmqs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2cbccnxsj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2laaxnmft.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qzwwpfmf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvcywjte.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fqncmdjy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbcxpfgz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dghfjkgz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mmyfkymm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fuaurgqk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anwanhww.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qkcfyout.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qvgxpxix.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mvomqkxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fzsfbgwk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xnwvqthc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uihhbhff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qldglilj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vypubibm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mgksnhmm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2chxxmhux.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uftxcrky.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2olnvmjrw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvwkypmm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zhqrgijz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2snlqrjwz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nswieiqa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lyrdxcok.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rwttacbc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dpsahoyj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wyqvnlrg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zaikousb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2flvuaedq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2aobuzuka.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2iueazzps.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2alqushtb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ryllnzkr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uugvpqcx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2kxkdanzj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bhppkqfp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qdvxtino.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rvmiplbx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hexqtkhw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zndkmspu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjqajc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nudvjcmm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gnsogtje.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tiigrqpf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yocnsmku.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2odojvqeu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gvhdequk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hncunaye.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lqwtwkat.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rggrvchc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pssauuyc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2clpkoqdg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2upzpvlpn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rfwojhpa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lnmhvhtz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2dchsjgly.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cpvsxjte.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2xssnzhki.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vfqyozlr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zgmkkdpt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zplorztt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hrrcgdmm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2svhlbwsj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pxozpzky.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2uionpgrg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kobumhwc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gyzufaxw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sghkkjhu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fmkqovve.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lvfuttuo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozbhvigg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fesigpem.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zwlhvzlt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lerhsrlv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vivbyyyc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wpnvmaig.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tutuhmtg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vrzdphvp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wzfviltp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hrkyjxgq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oydkzogc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2smzvfitk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wxlkprwj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lhpknkjb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2exmfcgnj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2edjjwxbp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cwxhfsgz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2yepvpwvx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhtnenki.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ixpqxrum.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2irmruwov.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2taynpcgs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uumsfvtz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2bdwyowhr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jkdlsyfa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vwugcfmo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2herqybyc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ttwzcijf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jufaaynb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uefimexd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2lgwbxxjg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zwmpcizg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpjlrfkr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2awecevzq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yyzyfppr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bduxrsld.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wrsmjtau.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eouhkoxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pkgwelnu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ouieueyn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2atqlmxke.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ssjpdjju.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2blthfrcq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qieybgya.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2eptpvoil.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qdfzqfvz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hbxupsot.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2btwaampa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mgixrodn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uuezaqcw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cyzpzllb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqgghlkf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2azigtely.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohljquug.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gbliyygh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnuqwnwf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2equieacz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cuftinoc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hyqrqgqi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ajaovqsg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pxitinho.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2prshfrxu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cnadbann.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pzraangd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2oyzdjghc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fhlmxrll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvdrbugo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tuaqgutm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wygcrrrq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xmkmqkea.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lykpyepl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvufbuqo.html


<!-- 参考信息 -->