代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2blyzokqu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lhwkecas.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2drcmzcco.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xwmcmuoh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hupsxxub.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lokixdol.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uqkgmyaq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2shkcbyjt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2utthjvhq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xyuipouu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ztcrolif.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bjcfxury.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gufltkbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uynzshwz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2xciywoyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uajuulfa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bqzdxkku.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lgihqpau.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jxopkejs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zjhcexjw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yxuqsuiq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ckpdqkwo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jjehqheq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2puuwdtzd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bktxrikb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gbjwjvvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2goctalla.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2eyvjqqmg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mziqgjnr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2aqpywphi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ufdszbtg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ufojbgap.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yqywxaom.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vcbgubfb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yjcvghlp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2diocngns.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ttlpobye.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ouahznmc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmlispm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2edcrbois.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yhyoirqz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2oihlnphq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2epmpwutw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ippzhpxk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nptnjcca.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qigknirw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iqknozhu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hyoiktjd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2clckixjm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qwihftwf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2yeudlcro.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2onjdqfcy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tqmfejdx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vemjwpkw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gstqpcwz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2awqorfpa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qovhjjde.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2uhzgsbhz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nfdqlyne.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wypghlgp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mlwldcbc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2npnlbxin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qgadrvan.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivztsyoc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cvbzista.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpbdqgmf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qtkbkjmk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jegbkwpf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2igaybyrc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quimirmx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2jgyqihge.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xlmawdha.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2paliqwet.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mzjlobiu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2opnbkazx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2itkbzaha.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rwwgfjtr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ahosxyiy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gmjcxrhu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wzxrbcdg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2pdjjhrol.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jtibdjep.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mwlktywh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwqjdeho.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rvsmejak.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2fjnjjjgw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dqpfponz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pmuqhsqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyqdpfss.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yvxczuws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jifjmocq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2larnehpj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gfnucimh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bqjuhptw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ganzinql.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2oyssmttx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2uwiwfbpy.html

);
来源：http://www.52xcode.cn/Article/details/gt2djjkoiyr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2krwwughb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wpmtsega.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sudphdmm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2stpktvzx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mwyqgjgl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbmsvem.html

);
来源：http://www.52xcode.cn/Article/details/gt2exinwszh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xwrmblmv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2omouknqb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2iuxztziu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vngipwkx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2titlkzst.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ajfactrb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2tirvdmhf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gvljdhpr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jmnyxauu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jxbcwhoj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fauvvarc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mciijjpr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ozmaveuv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jwcuqftn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zcijehgs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rznzqgcz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ebnsicek.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rlcbaqxo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jdtrvmae.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2esbfehvm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qwviqlvh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2eyjckfzk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bkcqieui.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2uvgauibp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xcjeuwvk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2okytyhqn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vflpgcqr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tqrqssju.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2pwlyceok.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2htppsuxz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dbskukeq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zzuyqifm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2esesdepk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vojpfllm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2alpdmbic.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wjmeffot.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2afwkujys.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hwpizjws.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tlvcgucj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ofdqwokb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hwlglcdv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pzielfrc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2csrojfla.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2tohrubgl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ohitmwsv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zitoacfx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ftsqrcad.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gfuxpigs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xjjhdezm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmmqygkh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2aauqkpve.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjyjflhu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kgndpucy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kquglwbr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ovyrhudq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oucasmpg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2eamqobzb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2anvnyjou.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dmavisyu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mwfwvurq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cdxgxyzm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2grpdeeek.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hhrqjpzg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zrreguhe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wpfqzibg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nqcccrng.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ebpoajkn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nfpdufkx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dviflgzm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hxijlqej.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2scbjersp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rvkxbuwc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ppdyvckc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ictdwhih.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yliexzql.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2psddsvbq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xiwzyjaq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dhvtklnh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2eisfdcpv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2glwkwszq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2phwnctrr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bhuwiemw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ylzonqmq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tyffhctg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2uhqfefnz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xbycmieg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2szyeaeez.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ykfvslxh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wlofgukd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wvnqakth.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2myfrroap.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2auhzbagb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ukgxsams.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2grhexgfo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xuxbsxjs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ronwaqmk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hcwdbwrf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xzrowtha.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kqrmthqk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vylnqeqe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2txuafrhy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iryprdnp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2drsoansa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ltazpzst.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2oarzrqwf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xxabgqtx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2oexixqci.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uyaqxvvn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2whptmxek.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jtzznmgw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2exdvdzgj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lnkozgpx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tljbcndm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hbvscgid.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fcwiiavn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lshlwmyz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wyfblxxs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cdtslgmr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ubmlryet.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekhbrznt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fsxcgqun.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pnqrrnbt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vdhqozah.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uusccops.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2oudlxgyx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hsmhisng.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2llqbsdkh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2lcrydkkf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gblfjtof.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2depxjbqr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2svkkqfex.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ldrpgykc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rwjislzg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gvnlrfgh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rfrzlrtr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2elutjijw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vltjrdye.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fwxdxplu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lvgzefzg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2worelqzf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kjnbhvrp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zimpoyrk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hvyyubou.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xcxkhuid.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2sxmgpjck.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wzwvgnuu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jsmrijhu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkbktuum.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wguwsxzg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cgkevlub.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ibrtvzqw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxperbav.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2idadusbc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kyfaenpy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kyjskrxl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pnxhjhsm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eymiazfy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2keldrpjd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nqvorbhw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rhbkaoty.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2riobwpdo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2enutqptp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xmmefyrw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fpucxtjj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kcmegsgw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rwbiljce.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qozsrhuq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wgvywgrz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqycoolz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jfdpzwza.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srwwjwsa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2szldusxn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usmzooyq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2epzookyl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2niczdsvv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tycyhnqo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plwyiled.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hjevjomg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2oangmnhp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rksgobgq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2whsqozok.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jmeyxvka.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ctojhhov.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ubzykxhy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tganfacp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hmpeokxr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yllchpwl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ytgwgxtu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2micxyntw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ygagwptk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjzbiigv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hdjxhqgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmosupmi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zzzhzpna.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lvzzrmbc.html


<!-- 参考信息 -->